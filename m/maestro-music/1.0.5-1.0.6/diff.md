# Comparing `tmp/maestro-music-1.0.5.tar.gz` & `tmp/maestro-music-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maestro-music-1.0.5.tar", last modified: Tue Jun 13 05:40:21 2023, max compression
+gzip compressed data, was "maestro-music-1.0.6.tar", last modified: Tue Jul 18 06:06:04 2023, max compression
```

## Comparing `maestro-music-1.0.5.tar` & `maestro-music-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-06-13 05:40:21.330181 maestro-music-1.0.5/
--rw-r--r--   0 sysadmin   (501) staff       (20)     1067 2023-06-06 05:56:48.000000 maestro-music-1.0.5/LICENSE
--rw-r--r--   0 sysadmin   (501) staff       (20)    11718 2023-06-13 05:40:21.329937 maestro-music-1.0.5/PKG-INFO
--rw-r--r--   0 sysadmin   (501) staff       (20)    40840 2023-06-13 05:39:50.000000 maestro-music-1.0.5/helpers.py
--rw-r--r--   0 sysadmin   (501) staff       (20)   146639 2023-03-25 20:23:16.000000 maestro-music-1.0.5/icon.py
--rw-r--r--   0 sysadmin   (501) staff       (20)     8837 2023-06-08 00:47:48.000000 maestro-music-1.0.5/mac_presence.py
--rw-r--r--   0 sysadmin   (501) staff       (20)   111717 2023-06-08 06:29:07.000000 maestro-music-1.0.5/maestro.py
-drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-06-13 05:40:21.329698 maestro-music-1.0.5/maestro_music.egg-info/
--rw-r--r--   0 sysadmin   (501) staff       (20)    11718 2023-06-13 05:40:21.000000 maestro-music-1.0.5/maestro_music.egg-info/PKG-INFO
--rw-r--r--   0 sysadmin   (501) staff       (20)      286 2023-06-13 05:40:21.000000 maestro-music-1.0.5/maestro_music.egg-info/SOURCES.txt
--rw-r--r--   0 sysadmin   (501) staff       (20)        1 2023-06-13 05:40:21.000000 maestro-music-1.0.5/maestro_music.egg-info/dependency_links.txt
--rw-r--r--   0 sysadmin   (501) staff       (20)       40 2023-06-13 05:40:21.000000 maestro-music-1.0.5/maestro_music.egg-info/entry_points.txt
--rw-r--r--   0 sysadmin   (501) staff       (20)      367 2023-06-13 05:40:21.000000 maestro-music-1.0.5/maestro_music.egg-info/requires.txt
--rw-r--r--   0 sysadmin   (501) staff       (20)       34 2023-06-13 05:40:21.000000 maestro-music-1.0.5/maestro_music.egg-info/top_level.txt
--rw-r--r--   0 sysadmin   (501) staff       (20)       38 2023-06-13 05:40:21.330245 maestro-music-1.0.5/setup.cfg
--rw-r--r--   0 sysadmin   (501) staff       (20)     1646 2023-06-13 05:40:20.000000 maestro-music-1.0.5/setup.py
+drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-07-18 06:06:04.417618 maestro-music-1.0.6/
+-rw-r--r--   0 sysadmin   (501) staff       (20)     1067 2023-06-06 05:56:48.000000 maestro-music-1.0.6/LICENSE
+-rw-r--r--   0 sysadmin   (501) staff       (20)    11718 2023-07-18 06:06:04.416723 maestro-music-1.0.6/PKG-INFO
+-rw-r--r--   0 sysadmin   (501) staff       (20)    39637 2023-07-18 05:38:37.000000 maestro-music-1.0.6/helpers.py
+-rw-r--r--   0 sysadmin   (501) staff       (20)   146639 2023-03-25 20:23:16.000000 maestro-music-1.0.6/icon.py
+-rw-r--r--   0 sysadmin   (501) staff       (20)     8837 2023-06-08 00:47:48.000000 maestro-music-1.0.6/mac_presence.py
+-rw-r--r--   0 sysadmin   (501) staff       (20)   115701 2023-07-18 06:06:00.000000 maestro-music-1.0.6/maestro.py
+drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-07-18 06:06:04.416414 maestro-music-1.0.6/maestro_music.egg-info/
+-rw-r--r--   0 sysadmin   (501) staff       (20)    11718 2023-07-18 06:06:04.000000 maestro-music-1.0.6/maestro_music.egg-info/PKG-INFO
+-rw-r--r--   0 sysadmin   (501) staff       (20)      286 2023-07-18 06:06:04.000000 maestro-music-1.0.6/maestro_music.egg-info/SOURCES.txt
+-rw-r--r--   0 sysadmin   (501) staff       (20)        1 2023-07-18 06:06:04.000000 maestro-music-1.0.6/maestro_music.egg-info/dependency_links.txt
+-rw-r--r--   0 sysadmin   (501) staff       (20)       40 2023-07-18 06:06:04.000000 maestro-music-1.0.6/maestro_music.egg-info/entry_points.txt
+-rw-r--r--   0 sysadmin   (501) staff       (20)      367 2023-07-18 06:06:04.000000 maestro-music-1.0.6/maestro_music.egg-info/requires.txt
+-rw-r--r--   0 sysadmin   (501) staff       (20)       34 2023-07-18 06:06:04.000000 maestro-music-1.0.6/maestro_music.egg-info/top_level.txt
+-rw-r--r--   0 sysadmin   (501) staff       (20)       38 2023-07-18 06:06:04.418157 maestro-music-1.0.6/setup.cfg
+-rw-r--r--   0 sysadmin   (501) staff       (20)     1532 2023-07-14 03:24:42.000000 maestro-music-1.0.6/setup.py
```

### Comparing `maestro-music-1.0.5/LICENSE` & `maestro-music-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `maestro-music-1.0.5/PKG-INFO` & `maestro-music-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maestro-music
-Version: 1.0.5
+Version: 1.0.6
 Summary: A simple command line tool to play songs (or any audio files, really).
 Home-page: https://github.com/PrajwalVandana/maestro-cli
 Author: Prajwal Vandana
 License: MIT
 Keywords: music,sound,audio,music-player,cli,ogg,flac,mp3,wav,spotify,youtube,audio-visualization,audio-visualizer
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `maestro-music-1.0.5/helpers.py` & `maestro-music-1.0.6/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,17 @@
     "#bitspersample",
     "#samplerate",
 )
 
 # region paths
 MAESTRO_DIR = os.path.join(os.path.expanduser("~"), ".maestro-files/")
 
-SONGS_DIR = os.path.join(MAESTRO_DIR, "songs/")
+SETTINGS_FILE = os.path.join(MAESTRO_DIR, "settings.json")
+DEFAULT_SONGS_DIR = os.path.join(MAESTRO_DIR, "songs/")
+SONGS_DIR = None
 
 SONGS_INFO_PATH = os.path.join(MAESTRO_DIR, "songs.txt")
 
 STATS_DIR = os.path.join(MAESTRO_DIR, "stats/")
 CUR_YEAR_STATS_PATH = os.path.join(STATS_DIR, f"{CUR_YEAR}.txt")
 TOTAL_STATS_PATH = os.path.join(STATS_DIR, "total.txt")
 # endregion
@@ -210,15 +212,15 @@
     return avg_head
 
 
 # @jit
 def render(
     num_bins,
     freqs,
-    t,
+    frame,
     visualizer_height,
     mono=None,
     include_remainder=None,
     func=np.max,
 ):
     """
     mono:
@@ -230,20 +232,20 @@
         mono = np.array_equal(freqs[0], freqs[1])
 
     if not mono:
         gap_bins = 1 if num_bins % 2 else 2
         num_bins = (num_bins - 1) // 2
     else:
         gap_bins = 0
-        freqs[0, :, t] = (freqs[0, :, t] + freqs[1, :, t]) / 2
+        freqs[0, :, frame] = (freqs[0, :, frame] + freqs[1, :, frame]) / 2
 
     num_vertical_block_sizes = len(VERTICAL_BLOCKS) - 1
     freqs = np.round(
         bin_average(
-            freqs[:, :, t],
+            freqs[:, :, frame],
             num_bins,
             (freqs.shape[-2] % num_bins) > num_bins / 2
             if include_remainder is None
             else include_remainder,
             func=func,
         )
         / 80
@@ -883,33 +885,14 @@
     )
 
 
 def clip_editor(stdscr, details):
     song_name = details[1]
     song_path = os.path.join(SONGS_DIR, song_name)
 
-    show_waveform = True
-    if LIBROSA is None:
-        show_waveform = False
-    else:
-        audio_data = LIBROSA.load(song_path, sr=SAMPLE_RATE)[0]
-
-        if len(audio_data.shape) == 1:  # mono -> stereo
-            audio_data = np.repeat([audio_data], 2, axis=0)
-        elif audio_data.shape[0] == 1:  # mono -> stereo
-            audio_data = np.repeat(audio_data, 2, axis=0)
-        elif audio_data.shape[0] == 6:  # 5.1 surround -> stereo
-            audio_data = np.delete(audio_data, (1, 3, 4, 5), axis=0)
-
-        audio_data /= np.max(np.abs(audio_data))
-        audio_data = (
-            80
-            * ((np.reshape(audio_data, audio_data.shape + (1,)) + 1) / 2) ** 80
-        )
-
     playback = Playback()
     playback.load_file(song_path)
 
     init_curses(stdscr)
 
     if details[3]:
         clip_start, clip_end = [float(x) for x in details[3].split()]
@@ -929,23 +912,21 @@
             (playback.curr_pos - last_timestamp)
             >= (playback.duration / (8 * (stdscr.getmaxyx()[1] - 2)))
         )
 
         if change_output:
             clip_editor_output(
                 stdscr,
-                audio_data,
                 details,
                 playback.curr_pos,
                 playback.paused,
                 playback.duration,
                 clip_start,
                 clip_end,
                 editing_start,
-                show_waveform,
             )
 
         c = stdscr.getch()
         next_c = stdscr.getch()
         while next_c != -1:
             c, next_c = next_c, stdscr.getch()
 
@@ -1035,64 +1016,44 @@
                     break
 
     return clip_start, clip_end
 
 
 def clip_editor_output(
     stdscr,
-    audio_data,
     details,
     pos,
     paused,
     duration,
     clip_start,
     clip_end,
     editing_start,
-    show_waveform,
 ):
     stdscr.erase()
 
     if stdscr.getmaxyx()[0] < 3:
         stdscr.addstr("Window too small.", curses.color_pair(4))
         stdscr.refresh()
         return
 
     screen_width = stdscr.getmaxyx()[1]
 
-    show_waveform = (
-        show_waveform and stdscr.getmaxyx()[0] >= 4 + WAVEFORM_HEIGHT
-    )
-    if show_waveform:
-        rendered_lines = render(
-            screen_width - 2,
-            audio_data,
-            0,
-            WAVEFORM_HEIGHT,
-            mono=True,
-            include_remainder=True,
-            func=np.max,
-        )
-
     stdscr.insstr(
         f"{format_seconds(clip_start, show_decimal=True)}"
         + (" <" if editing_start else ""),
         curses.color_pair(7),
     )
 
     end_str = (
         "> " if not editing_start else ""
     ) + f"{format_seconds(clip_end, show_decimal=True)}"
     stdscr.move(0, screen_width - len(end_str))
     stdscr.insstr(end_str, curses.color_pair(7))
 
     stdscr.move(1, 0)
-    if show_waveform:
-        for i in range(len(rendered_lines)):
-            stdscr.addstr(" " + rendered_lines[i])
-            stdscr.move(stdscr.getyx()[0] + 1, 0)
 
     clip_bar_width = screen_width - 2
     if clip_bar_width > 0:
         bar = "|"
         before_clip_block_width = round(
             (clip_bar_width * 8 * clip_start) / duration
         )
```

### Comparing `maestro-music-1.0.5/icon.py` & `maestro-music-1.0.6/icon.py`

 * *Files identical despite different names*

### Comparing `maestro-music-1.0.5/mac_presence.py` & `maestro-music-1.0.6/mac_presence.py`

 * *Files identical despite different names*

### Comparing `maestro-music-1.0.5/maestro.py` & `maestro-music-1.0.6/maestro.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,6983 +1,7232 @@
 00000000: 2320 7265 6769 6f6e 2069 6d70 6f72 7473  # region imports
 00000010: 0a69 6d70 6f72 7420 6375 7273 6573 0a69  .import curses.i
-00000020: 6d70 6f72 7420 6d75 6c74 6970 726f 6365  mport multiproce
-00000030: 7373 696e 670a 696d 706f 7274 206f 730a  ssing.import os.
-00000040: 6672 6f6d 2073 6875 7469 6c20 696d 706f  from shutil impo
-00000050: 7274 206d 6f76 650a 696d 706f 7274 2073  rt move.import s
-00000060: 7562 7072 6f63 6573 730a 696d 706f 7274  ubprocess.import
-00000070: 2073 7973 0a0a 696d 706f 7274 2063 6c69   sys..import cli
-00000080: 636b 0a69 6d70 6f72 7420 6d75 7369 635f  ck.import music_
-00000090: 7461 670a 0a66 726f 6d20 636f 6c6c 6563  tag..from collec
-000000a0: 7469 6f6e 7320 696d 706f 7274 2064 6566  tions import def
-000000b0: 6175 6c74 6469 6374 0a66 726f 6d20 7175  aultdict.from qu
-000000c0: 6575 6520 696d 706f 7274 2051 7565 7565  eue import Queue
-000000d0: 0a66 726f 6d20 7261 6e64 6f6d 2069 6d70  .from random imp
-000000e0: 6f72 7420 7368 7566 666c 652c 2072 616e  ort shuffle, ran
-000000f0: 6469 6e74 0a66 726f 6d20 7469 6d65 2069  dint.from time i
-00000100: 6d70 6f72 7420 736c 6565 702c 2074 696d  mport sleep, tim
-00000110: 650a 0a66 726f 6d20 6963 6f6e 2069 6d70  e..from icon imp
-00000120: 6f72 7420 696d 670a 0a66 726f 6d20 6a75  ort img..from ju
-00000130: 7374 5f70 6c61 7962 6163 6b20 696d 706f  st_playback impo
-00000140: 7274 2050 6c61 7962 6163 6b0a 0a63 616e  rt Playback..can
-00000150: 5f75 7064 6174 655f 6469 7363 6f72 6420  _update_discord 
-00000160: 3d20 5472 7565 0a74 7279 3a0a 2020 2020  = True.try:.    
-00000170: 696d 706f 7274 2070 7970 7265 7365 6e63  import pypresenc
-00000180: 650a 6578 6365 7074 2049 6d70 6f72 7445  e.except ImportE
-00000190: 7272 6f72 3a0a 2020 2020 6361 6e5f 7570  rror:.    can_up
-000001a0: 6461 7465 5f64 6973 636f 7264 203d 2046  date_discord = F
-000001b0: 616c 7365 0a0a 6672 6f6d 2068 656c 7065  alse..from helpe
-000001c0: 7273 2069 6d70 6f72 7420 2a20 2023 2070  rs import *  # p
-000001d0: 796c 696e 743a 2064 6973 6162 6c65 3d77  ylint: disable=w
-000001e0: 696c 6463 6172 642d 696d 706f 7274 2c75  ildcard-import,u
-000001f0: 6e75 7365 642d 7769 6c64 6361 7264 2d69  nused-wildcard-i
-00000200: 6d70 6f72 740a 0a69 6620 7379 732e 706c  mport..if sys.pl
-00000210: 6174 666f 726d 203d 3d20 2264 6172 7769  atform == "darwi
-00000220: 6e22 3a0a 2020 2020 7472 793a 0a20 2020  n":.    try:.   
-00000230: 2020 2020 2023 2070 796c 696e 743a 2064       # pylint: d
-00000240: 6973 6162 6c65 3d6e 6f2d 6e61 6d65 2d69  isable=no-name-i
-00000250: 6e2d 6d6f 6475 6c65 2c69 6d70 6f72 742d  n-module,import-
-00000260: 6572 726f 720a 2020 2020 2020 2020 6672  error.        fr
-00000270: 6f6d 2041 7070 4b69 7420 696d 706f 7274  om AppKit import
-00000280: 2028 0a20 2020 2020 2020 2020 2020 204e   (.            N
-00000290: 5341 7070 2c0a 2020 2020 2020 2020 2020  SApp,.          
-000002a0: 2020 4e53 4170 706c 6963 6174 696f 6e2c    NSApplication,
-000002b0: 0a20 2020 2020 2020 2020 2020 204e 5341  .            NSA
-000002c0: 7070 6c69 6361 7469 6f6e 4163 7469 7661  pplicationActiva
-000002d0: 7469 6f6e 506f 6c69 6379 5072 6f68 6962  tionPolicyProhib
-000002e0: 6974 6564 2c0a 2020 2020 2020 2020 2020  ited,.          
-000002f0: 2020 4e53 4461 7465 2c0a 2020 2020 2020    NSDate,.      
-00000300: 2020 2020 2020 4e53 4f62 6a65 6374 2c0a        NSObject,.
-00000310: 2020 2020 2020 2020 2020 2020 4e53 5275              NSRu
-00000320: 6e4c 6f6f 702c 0a20 2020 2020 2020 2029  nLoop,.        )
-00000330: 0a0a 2020 2020 2020 2020 2320 6672 6f6d  ..        # from
-00000340: 204d 6564 6961 506c 6179 6572 2069 6d70   MediaPlayer imp
-00000350: 6f72 7420 4d50 4e6f 7750 6c61 7969 6e67  ort MPNowPlaying
-00000360: 496e 666f 5072 6f70 6572 7479 456c 6170  InfoPropertyElap
-00000370: 7365 6450 6c61 7962 6163 6b54 696d 650a  sedPlaybackTime.
-00000380: 2020 2020 2020 2020 6672 6f6d 2050 794f          from PyO
-00000390: 626a 4354 6f6f 6c73 2069 6d70 6f72 7420  bjCTools import 
-000003a0: 4170 7048 656c 7065 720a 0a20 2020 2020  AppHelper..     
-000003b0: 2020 2066 726f 6d20 6d61 635f 7072 6573     from mac_pres
-000003c0: 656e 6365 2069 6d70 6f72 7420 4d61 634e  ence import MacN
-000003d0: 6f77 506c 6179 696e 670a 0a20 2020 2020  owPlaying..     
-000003e0: 2020 2023 2067 6c6f 6261 6c73 0a20 2020     # globals.   
-000003f0: 2020 2020 206d 6163 5f6e 6f77 5f70 6c61       mac_now_pla
-00000400: 7969 6e67 203d 204d 6163 4e6f 7750 6c61  ying = MacNowPla
-00000410: 7969 6e67 2829 0a20 2020 2020 2020 2063  ying().        c
-00000420: 6f76 6572 5f69 6d67 203d 2069 6d67 0a0a  over_img = img..
-00000430: 2020 2020 2020 2020 6361 6e5f 6d61 635f          can_mac_
-00000440: 6e6f 775f 706c 6179 696e 6720 3d20 5472  now_playing = Tr
-00000450: 7565 0a20 2020 2065 7863 6570 7420 4578  ue.    except Ex
-00000460: 6365 7074 696f 6e20 6173 2065 3a20 2023  ception as e:  #
-00000470: 2070 796c 696e 743a 2064 6973 6162 6c65   pylint: disable
-00000480: 3d62 6172 652d 6578 6365 7074 2c62 726f  =bare-except,bro
-00000490: 6164 2d65 7863 6570 740a 2020 2020 2020  ad-except.      
-000004a0: 2020 2320 7072 696e 7428 652c 2066 696c    # print(e, fil
-000004b0: 653d 6f70 656e 2822 6c6f 672e 7478 7422  e=open("log.txt"
-000004c0: 2c20 2261 2229 290a 2020 2020 2020 2020  , "a")).        
-000004d0: 6361 6e5f 6d61 635f 6e6f 775f 706c 6179  can_mac_now_play
-000004e0: 696e 6720 3d20 4661 6c73 650a 0a23 2065  ing = False..# e
-000004f0: 6e64 7265 6769 6f6e 0a0a 2320 7265 6769  ndregion..# regi
-00000500: 6f6e 2075 7469 6c69 7479 2066 756e 6374  on utility funct
-00000510: 696f 6e73 2f63 6c61 7373 6573 0a0a 6966  ions/classes..if
-00000520: 2073 7973 2e70 6c61 7466 6f72 6d20 3d3d   sys.platform ==
-00000530: 2022 6461 7277 696e 2220 616e 6420 6361   "darwin" and ca
-00000540: 6e5f 6d61 635f 6e6f 775f 706c 6179 696e  n_mac_now_playin
-00000550: 673a 0a0a 2020 2020 636c 6173 7320 4170  g:..    class Ap
-00000560: 7044 656c 6567 6174 6528 4e53 4f62 6a65  pDelegate(NSObje
-00000570: 6374 293a 2020 2320 736f 2050 7974 686f  ct):  # so Pytho
-00000580: 6e20 646f 6573 6e27 7420 626f 756e 6365  n doesn't bounce
-00000590: 2069 6e20 7468 6520 646f 636b 0a20 2020   in the dock.   
-000005a0: 2020 2020 2064 6566 2061 7070 6c69 6361       def applica
-000005b0: 7469 6f6e 4469 6446 696e 6973 684c 6175  tionDidFinishLau
-000005c0: 6e63 6869 6e67 5f28 7365 6c66 2c20 5f61  nching_(self, _a
-000005d0: 4e6f 7469 6669 6361 7469 6f6e 293a 0a20  Notification):. 
-000005e0: 2020 2020 2020 2020 2020 2070 6173 730a             pass.
-000005f0: 0a20 2020 2020 2020 2064 6566 2073 6179  .        def say
-00000600: 4865 6c6c 6f5f 2873 656c 662c 205f 7365  Hello_(self, _se
-00000610: 6e64 6572 293a 0a20 2020 2020 2020 2020  nder):.         
-00000620: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
-00000630: 2061 7070 5f68 656c 7065 725f 6c6f 6f70   app_helper_loop
-00000640: 2829 3a0a 2020 2020 2020 2020 2320 6e73  ():.        # ns
-00000650: 5f61 7070 6c69 6361 7469 6f6e 203d 204e  _application = N
-00000660: 5341 7070 6c69 6361 7469 6f6e 2e73 6861  SApplication.sha
-00000670: 7265 6441 7070 6c69 6361 7469 6f6e 2829  redApplication()
-00000680: 0a20 2020 2020 2020 2023 206c 6f67 6f5f  .        # logo_
-00000690: 6e73 5f69 6d61 6765 203d 204e 5349 6d61  ns_image = NSIma
-000006a0: 6765 2e61 6c6c 6f63 2829 2e69 6e69 7442  ge.alloc().initB
-000006b0: 7952 6566 6572 656e 6369 6e67 4669 6c65  yReferencingFile
-000006c0: 5f28 0a20 2020 2020 2020 2023 2020 2020  _(.        #    
-000006d0: 2022 2e2f 6d61 6573 7472 6f5f 6963 6f6e   "./maestro_icon
-000006e0: 2e70 6e67 220a 2020 2020 2020 2020 2320  .png".        # 
-000006f0: 290a 2020 2020 2020 2020 2320 6e73 5f61  ).        # ns_a
-00000700: 7070 6c69 6361 7469 6f6e 2e73 6574 4170  pplication.setAp
-00000710: 706c 6963 6174 696f 6e49 636f 6e49 6d61  plicationIconIma
-00000720: 6765 5f28 6c6f 676f 5f6e 735f 696d 6167  ge_(logo_ns_imag
-00000730: 6529 0a0a 2020 2020 2020 2020 2320 2320  e)..        # # 
-00000740: 7765 206d 7573 7420 6b65 6570 2061 2072  we must keep a r
-00000750: 6566 6572 656e 6365 2074 6f20 7468 6520  eference to the 
-00000760: 6465 6c65 6761 7465 206f 626a 6563 7420  delegate object 
-00000770: 6f75 7273 656c 7665 732c 0a20 2020 2020  ourselves,.     
-00000780: 2020 2023 2023 204e 5341 7070 2e73 6574     # # NSApp.set
-00000790: 4465 6c65 6761 7465 5f28 2920 646f 6573  Delegate_() does
-000007a0: 6e27 7420 7265 7461 696e 2069 742e 2041  n't retain it. A
-000007b0: 206c 6f63 616c 2076 6172 6961 626c 6520   local variable 
-000007c0: 6973 0a20 2020 2020 2020 2023 2023 2065  is.        # # e
-000007d0: 6e6f 7567 6820 6865 7265 2e0a 2020 2020  nough here..    
-000007e0: 2020 2020 2320 6465 6c65 6761 7465 203d      # delegate =
-000007f0: 2041 7070 4465 6c65 6761 7465 2e61 6c6c   AppDelegate.all
-00000800: 6f63 2829 2e69 6e69 7428 290a 2020 2020  oc().init().    
-00000810: 2020 2020 2320 4e53 4170 7028 292e 7365      # NSApp().se
-00000820: 7444 656c 6567 6174 655f 2864 656c 6567  tDelegate_(deleg
-00000830: 6174 6529 0a0a 2020 2020 2020 2020 4170  ate)..        Ap
-00000840: 7048 656c 7065 722e 7275 6e45 7665 6e74  pHelper.runEvent
-00000850: 4c6f 6f70 2829 0a0a 0a64 6566 2064 6973  Loop()...def dis
-00000860: 636f 7264 5f70 7265 7365 6e63 655f 6c6f  cord_presence_lo
-00000870: 6f70 2873 6f6e 675f 6e61 6d65 5f71 7565  op(song_name_que
-00000880: 7565 2c20 6172 7469 7374 5f71 7565 7565  ue, artist_queue
-00000890: 2c20 6469 7363 6f72 645f 636f 6e6e 6563  , discord_connec
-000008a0: 7465 6429 3a0a 2020 2020 7472 793a 0a20  ted):.    try:. 
-000008b0: 2020 2020 2020 2064 6973 636f 7264 5f72         discord_r
-000008c0: 7063 203d 2070 7970 7265 7365 6e63 652e  pc = pypresence.
-000008d0: 5072 6573 656e 6365 2863 6c69 656e 745f  Presence(client_
-000008e0: 6964 3d44 4953 434f 5244 5f49 4429 0a20  id=DISCORD_ID). 
-000008f0: 2020 2020 2020 2064 6973 636f 7264 5f72         discord_r
-00000900: 7063 2e63 6f6e 6e65 6374 2829 0a20 2020  pc.connect().   
-00000910: 2020 2020 2064 6973 636f 7264 5f63 6f6e       discord_con
-00000920: 6e65 6374 6564 2e76 616c 7565 203d 2031  nected.value = 1
-00000930: 0a20 2020 2065 7863 6570 743a 2020 2320  .    except:  # 
-00000940: 7079 6c69 6e74 3a20 6469 7361 626c 653d  pylint: disable=
-00000950: 6261 7265 2d65 7863 6570 740a 2020 2020  bare-except.    
-00000960: 2020 2020 6469 7363 6f72 645f 636f 6e6e      discord_conn
-00000970: 6563 7465 642e 7661 6c75 6520 3d20 300a  ected.value = 0.
-00000980: 0a20 2020 2077 6869 6c65 2054 7275 653a  .    while True:
-00000990: 0a20 2020 2020 2020 2073 6f6e 675f 6e61  .        song_na
-000009a0: 6d65 203d 2022 220a 2020 2020 2020 2020  me = "".        
-000009b0: 6966 206e 6f74 2073 6f6e 675f 6e61 6d65  if not song_name
-000009c0: 5f71 7565 7565 2e65 6d70 7479 2829 206f  _queue.empty() o
-000009d0: 7220 736f 6e67 5f6e 616d 653a 0a20 2020  r song_name:.   
-000009e0: 2020 2020 2020 2020 2077 6869 6c65 206e           while n
-000009f0: 6f74 2073 6f6e 675f 6e61 6d65 5f71 7565  ot song_name_que
-00000a00: 7565 2e65 6d70 7479 2829 3a0a 2020 2020  ue.empty():.    
-00000a10: 2020 2020 2020 2020 2020 2020 736f 6e67              song
-00000a20: 5f6e 616d 6520 3d20 2222 0a20 2020 2020  _name = "".     
-00000a30: 2020 2020 2020 2020 2020 2063 203d 2073             c = s
-00000a40: 6f6e 675f 6e61 6d65 5f71 7565 7565 2e67  ong_name_queue.g
-00000a50: 6574 2829 0a20 2020 2020 2020 2020 2020  et().           
-00000a60: 2020 2020 2077 6869 6c65 2063 2021 3d20       while c != 
-00000a70: 225c 6e22 3a0a 2020 2020 2020 2020 2020  "\n":.          
-00000a80: 2020 2020 2020 2020 2020 736f 6e67 5f6e            song_n
-00000a90: 616d 6520 2b3d 2063 0a20 2020 2020 2020  ame += c.       
-00000aa0: 2020 2020 2020 2020 2020 2020 2063 203d               c =
-00000ab0: 2073 6f6e 675f 6e61 6d65 5f71 7565 7565   song_name_queue
-00000ac0: 2e67 6574 2829 0a0a 2020 2020 2020 2020  .get()..        
-00000ad0: 2020 2020 6172 7469 7374 5f6e 616d 6520      artist_name 
-00000ae0: 3d20 2222 0a20 2020 2020 2020 2020 2020  = "".           
-00000af0: 2077 6869 6c65 206e 6f74 2061 7274 6973   while not artis
-00000b00: 745f 7175 6575 652e 656d 7074 7928 293a  t_queue.empty():
-00000b10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000b20: 2061 7274 6973 745f 6e61 6d65 203d 2022   artist_name = "
-00000b30: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00000b40: 2020 6320 3d20 6172 7469 7374 5f71 7565    c = artist_que
-00000b50: 7565 2e67 6574 2829 0a20 2020 2020 2020  ue.get().       
-00000b60: 2020 2020 2020 2020 2077 6869 6c65 2063           while c
-00000b70: 2021 3d20 225c 6e22 3a0a 2020 2020 2020   != "\n":.      
-00000b80: 2020 2020 2020 2020 2020 2020 2020 6172                ar
-00000b90: 7469 7374 5f6e 616d 6520 2b3d 2063 0a20  tist_name += c. 
-00000ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000bb0: 2020 2063 203d 2061 7274 6973 745f 7175     c = artist_qu
-00000bc0: 6575 652e 6765 7428 290a 0a20 2020 2020  eue.get()..     
-00000bd0: 2020 2020 2020 2061 7274 6973 745f 6e61         artist_na
-00000be0: 6d65 203d 2022 6279 2022 202b 2061 7274  me = "by " + art
-00000bf0: 6973 745f 6e61 6d65 0a0a 2020 2020 2020  ist_name..      
-00000c00: 2020 2020 2020 6966 2064 6973 636f 7264        if discord
-00000c10: 5f63 6f6e 6e65 6374 6564 2e76 616c 7565  _connected.value
-00000c20: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00000c30: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-00000c40: 2020 2020 2020 2020 2020 2064 6973 636f             disco
-00000c50: 7264 5f72 7063 2e75 7064 6174 6528 0a20  rd_rpc.update(. 
-00000c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c70: 2020 2020 2020 2064 6574 6169 6c73 3d73         details=s
-00000c80: 6f6e 675f 6e61 6d65 2c0a 2020 2020 2020  ong_name,.      
-00000c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ca0: 2020 7374 6174 653d 6172 7469 7374 5f6e    state=artist_n
-00000cb0: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
-00000cc0: 2020 2020 2020 2020 2020 2020 206c 6172               lar
-00000cd0: 6765 5f69 6d61 6765 3d22 6d61 6573 7472  ge_image="maestr
-00000ce0: 6f2d 6963 6f6e 222c 0a20 2020 2020 2020  o-icon",.       
-00000cf0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-00000d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d10: 2020 2073 6f6e 675f 6e61 6d65 203d 2022     song_name = "
-00000d20: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00000d30: 2020 2020 2020 6172 7469 7374 5f6e 616d        artist_nam
-00000d40: 6520 3d20 2222 0a20 2020 2020 2020 2020  e = "".         
-00000d50: 2020 2020 2020 2020 2020 2073 6c65 6570             sleep
-00000d60: 2831 3529 0a20 2020 2020 2020 2020 2020  (15).           
-00000d70: 2020 2020 2065 7863 6570 743a 2020 2320       except:  # 
-00000d80: 7079 6c69 6e74 3a20 6469 7361 626c 653d  pylint: disable=
-00000d90: 6261 7265 2d65 7863 6570 740a 2020 2020  bare-except.    
-00000da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000db0: 6469 7363 6f72 645f 636f 6e6e 6563 7465  discord_connecte
-00000dc0: 642e 7661 6c75 6520 3d20 300a 2020 2020  d.value = 0.    
-00000dd0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00000de0: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-00000df0: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
-00000e00: 2020 2020 2020 2064 6973 636f 7264 5f72         discord_r
-00000e10: 7063 203d 2070 7970 7265 7365 6e63 652e  pc = pypresence.
-00000e20: 5072 6573 656e 6365 2863 6c69 656e 745f  Presence(client_
-00000e30: 6964 3d44 4953 434f 5244 5f49 4429 0a20  id=DISCORD_ID). 
-00000e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e50: 2020 2064 6973 636f 7264 5f72 7063 2e63     discord_rpc.c
-00000e60: 6f6e 6e65 6374 2829 0a20 2020 2020 2020  onnect().       
-00000e70: 2020 2020 2020 2020 2020 2020 2064 6973               dis
-00000e80: 636f 7264 5f63 6f6e 6e65 6374 6564 2e76  cord_connected.v
-00000e90: 616c 7565 203d 2031 0a20 2020 2020 2020  alue = 1.       
-00000ea0: 2020 2020 2020 2020 2065 7863 6570 743a           except:
-00000eb0: 2020 2320 7079 6c69 6e74 3a20 6469 7361    # pylint: disa
-00000ec0: 626c 653d 6261 7265 2d65 7863 6570 740a  ble=bare-except.
-00000ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ee0: 2020 2020 7061 7373 0a0a 2020 2020 2020      pass..      
-00000ef0: 2020 2020 2020 2020 2020 6966 2064 6973            if dis
-00000f00: 636f 7264 5f63 6f6e 6e65 6374 6564 2e76  cord_connected.v
-00000f10: 616c 7565 3a0a 2020 2020 2020 2020 2020  alue:.          
-00000f20: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
-00000f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f40: 2020 2020 2020 2064 6973 636f 7264 5f72         discord_r
-00000f50: 7063 2e75 7064 6174 6528 0a20 2020 2020  pc.update(.     
-00000f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f70: 2020 2020 2020 2064 6574 6169 6c73 3d73         details=s
-00000f80: 6f6e 675f 6e61 6d65 2c0a 2020 2020 2020  ong_name,.      
-00000f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000fa0: 2020 2020 2020 7374 6174 653d 6172 7469        state=arti
-00000fb0: 7374 5f6e 616d 652c 0a20 2020 2020 2020  st_name,.       
-00000fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000fd0: 2020 2020 206c 6172 6765 5f69 6d61 6765       large_image
-00000fe0: 3d22 6d61 6573 7472 6f2d 6963 6f6e 222c  ="maestro-icon",
-00000ff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001000: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00001010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001020: 2020 2073 6f6e 675f 6e61 6d65 203d 2022     song_name = "
-00001030: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00001040: 2020 2020 2020 2020 2020 6172 7469 7374            artist
-00001050: 5f6e 616d 6520 3d20 2222 0a20 2020 2020  _name = "".     
-00001060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001070: 2020 2073 6c65 6570 2831 3529 0a20 2020     sleep(15).   
-00001080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001090: 2065 7863 6570 743a 2020 2320 7079 6c69   except:  # pyli
-000010a0: 6e74 3a20 6469 7361 626c 653d 6261 7265  nt: disable=bare
-000010b0: 2d65 7863 6570 740a 2020 2020 2020 2020  -except.        
-000010c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010d0: 6469 7363 6f72 645f 636f 6e6e 6563 7465  discord_connecte
-000010e0: 642e 7661 6c75 6520 3d20 300a 2020 2020  d.value = 0.    
-000010f0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00001100: 2020 2020 2020 6966 206e 6f74 2064 6973        if not dis
-00001110: 636f 7264 5f63 6f6e 6e65 6374 6564 2e76  cord_connected.v
-00001120: 616c 7565 3a0a 2020 2020 2020 2020 2020  alue:.          
-00001130: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-00001140: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00001150: 6973 636f 7264 5f72 7063 203d 2070 7970  iscord_rpc = pyp
-00001160: 7265 7365 6e63 652e 5072 6573 656e 6365  resence.Presence
-00001170: 2863 6c69 656e 745f 6964 3d44 4953 434f  (client_id=DISCO
-00001180: 5244 5f49 4429 0a20 2020 2020 2020 2020  RD_ID).         
-00001190: 2020 2020 2020 2020 2020 2064 6973 636f             disco
-000011a0: 7264 5f72 7063 2e63 6f6e 6e65 6374 2829  rd_rpc.connect()
-000011b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000011c0: 2020 2020 2064 6973 636f 7264 5f63 6f6e       discord_con
-000011d0: 6e65 6374 6564 2e76 616c 7565 203d 2031  nected.value = 1
-000011e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000011f0: 2065 7863 6570 743a 2020 2320 7079 6c69   except:  # pyli
-00001200: 6e74 3a20 6469 7361 626c 653d 6261 7265  nt: disable=bare
-00001210: 2d65 7863 6570 740a 2020 2020 2020 2020  -except.        
-00001220: 2020 2020 2020 2020 2020 2020 7061 7373              pass
-00001230: 0a0a 0a64 6566 205f 706c 6179 280a 2020  ...def _play(.  
-00001240: 2020 7374 6473 6372 2c0a 2020 2020 706c    stdscr,.    pl
-00001250: 6179 6c69 7374 2c0a 2020 2020 766f 6c75  aylist,.    volu
-00001260: 6d65 2c0a 2020 2020 6c6f 6f70 2c0a 2020  me,.    loop,.  
-00001270: 2020 636c 6970 5f6d 6f64 652c 0a20 2020    clip_mode,.   
-00001280: 2072 6573 6875 6666 6c65 2c0a 2020 2020   reshuffle,.    
-00001290: 7570 6461 7465 5f64 6973 636f 7264 2c0a  update_discord,.
-000012a0: 2020 2020 7669 7375 616c 697a 652c 0a29      visualize,.)
-000012b0: 3a0a 2020 2020 676c 6f62 616c 2063 616e  :.    global can
-000012c0: 5f6d 6163 5f6e 6f77 5f70 6c61 7969 6e67  _mac_now_playing
-000012d0: 2020 2320 7079 6c69 6e74 3a20 6469 7361    # pylint: disa
-000012e0: 626c 653d 676c 6f62 616c 2d73 7461 7465  ble=global-state
-000012f0: 6d65 6e74 0a0a 2020 2020 696e 6974 5f63  ment..    init_c
-00001300: 7572 7365 7328 7374 6473 6372 290a 0a20  urses(stdscr).. 
-00001310: 2020 2069 6620 6c6f 6f70 3a0a 2020 2020     if loop:.    
-00001320: 2020 2020 6e65 7874 5f70 6c61 796c 6973      next_playlis
-00001330: 7420 3d20 706c 6179 6c69 7374 5b3a 5d0a  t = playlist[:].
-00001340: 2020 2020 2020 2020 6966 2072 6573 6875          if reshu
-00001350: 6666 6c65 3a0a 2020 2020 2020 2020 2020  ffle:.          
-00001360: 2020 7368 7566 666c 6528 6e65 7874 5f70    shuffle(next_p
-00001370: 6c61 796c 6973 7429 0a20 2020 2065 6c73  laylist).    els
-00001380: 653a 0a20 2020 2020 2020 206e 6578 745f  e:.        next_
-00001390: 706c 6179 6c69 7374 203d 204e 6f6e 650a  playlist = None.
-000013a0: 0a20 2020 2070 6c61 7965 725f 6f75 7470  .    player_outp
-000013b0: 7574 203d 2050 6c61 7965 724f 7574 7075  ut = PlayerOutpu
-000013c0: 7428 0a20 2020 2020 2020 2073 7464 7363  t(.        stdsc
-000013d0: 722c 2070 6c61 796c 6973 742c 2076 6f6c  r, playlist, vol
-000013e0: 756d 652c 2063 6c69 705f 6d6f 6465 2c20  ume, clip_mode, 
-000013f0: 7570 6461 7465 5f64 6973 636f 7264 2c20  update_discord, 
-00001400: 7669 7375 616c 697a 650a 2020 2020 290a  visualize.    ).
-00001410: 0a20 2020 2069 6620 706c 6179 6572 5f6f  .    if player_o
-00001420: 7574 7075 742e 7570 6461 7465 5f64 6973  utput.update_dis
-00001430: 636f 7264 3a0a 2020 2020 2020 2020 6469  cord:.        di
-00001440: 7363 6f72 645f 7469 746c 655f 7175 6575  scord_title_queu
-00001450: 6520 3d20 6d75 6c74 6970 726f 6365 7373  e = multiprocess
-00001460: 696e 672e 5369 6d70 6c65 5175 6575 6528  ing.SimpleQueue(
-00001470: 290a 2020 2020 2020 2020 6469 7363 6f72  ).        discor
-00001480: 645f 6172 7469 7374 5f71 7565 7565 203d  d_artist_queue =
-00001490: 206d 756c 7469 7072 6f63 6573 7369 6e67   multiprocessing
-000014a0: 2e53 696d 706c 6551 7565 7565 2829 0a20  .SimpleQueue(). 
-000014b0: 2020 2020 2020 2064 6973 636f 7264 5f70         discord_p
-000014c0: 7265 7365 6e63 655f 7072 6f63 6573 7320  resence_process 
-000014d0: 3d20 6d75 6c74 6970 726f 6365 7373 696e  = multiprocessin
-000014e0: 672e 5072 6f63 6573 7328 0a20 2020 2020  g.Process(.     
-000014f0: 2020 2020 2020 2064 6165 6d6f 6e3d 5472         daemon=Tr
-00001500: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-00001510: 7461 7267 6574 3d64 6973 636f 7264 5f70  target=discord_p
-00001520: 7265 7365 6e63 655f 6c6f 6f70 2c0a 2020  resence_loop,.  
-00001530: 2020 2020 2020 2020 2020 6172 6773 3d28            args=(
-00001540: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001550: 2064 6973 636f 7264 5f74 6974 6c65 5f71   discord_title_q
-00001560: 7565 7565 2c0a 2020 2020 2020 2020 2020  ueue,.          
-00001570: 2020 2020 2020 6469 7363 6f72 645f 6172        discord_ar
-00001580: 7469 7374 5f71 7565 7565 2c0a 2020 2020  tist_queue,.    
-00001590: 2020 2020 2020 2020 2020 2020 706c 6179              play
-000015a0: 6572 5f6f 7574 7075 742e 6469 7363 6f72  er_output.discor
-000015b0: 645f 636f 6e6e 6563 7465 642c 0a20 2020  d_connected,.   
-000015c0: 2020 2020 2020 2020 2029 2c0a 2020 2020           ),.    
-000015d0: 2020 2020 290a 2020 2020 2020 2020 6469      ).        di
-000015e0: 7363 6f72 645f 7072 6573 656e 6365 5f70  scord_presence_p
-000015f0: 726f 6365 7373 2e73 7461 7274 2829 0a0a  rocess.start()..
-00001600: 2020 2020 6966 2073 7973 2e70 6c61 7466      if sys.platf
-00001610: 6f72 6d20 3d3d 2022 6461 7277 696e 2220  orm == "darwin" 
-00001620: 616e 6420 6361 6e5f 6d61 635f 6e6f 775f  and can_mac_now_
-00001630: 706c 6179 696e 673a 0a20 2020 2020 2020  playing:.       
-00001640: 206d 6163 5f6e 6f77 5f70 6c61 7969 6e67   mac_now_playing
-00001650: 2e74 6974 6c65 5f71 7565 7565 203d 2051  .title_queue = Q
-00001660: 7565 7565 2829 0a20 2020 2020 2020 206d  ueue().        m
-00001670: 6163 5f6e 6f77 5f70 6c61 7969 6e67 2e61  ac_now_playing.a
-00001680: 7274 6973 745f 7175 6575 6520 3d20 5175  rtist_queue = Qu
-00001690: 6575 6528 290a 2020 2020 2020 2020 6d61  eue().        ma
-000016a0: 635f 6e6f 775f 706c 6179 696e 672e 7120  c_now_playing.q 
-000016b0: 3d20 5175 6575 6528 290a 2020 2020 2020  = Queue().      
-000016c0: 2020 6d61 635f 6e6f 775f 706c 6179 696e    mac_now_playin
-000016d0: 672e 636f 7665 7220 3d20 636f 7665 725f  g.cover = cover_
-000016e0: 696d 670a 0a20 2020 2020 2020 206e 735f  img..        ns_
-000016f0: 6170 706c 6963 6174 696f 6e20 3d20 4e53  application = NS
-00001700: 4170 706c 6963 6174 696f 6e2e 7368 6172  Application.shar
-00001710: 6564 4170 706c 6963 6174 696f 6e28 290a  edApplication().
-00001720: 2020 2020 2020 2020 2320 6c6f 676f 5f6e          # logo_n
-00001730: 735f 696d 6167 6520 3d20 4e53 496d 6167  s_image = NSImag
-00001740: 652e 616c 6c6f 6328 292e 696e 6974 4279  e.alloc().initBy
-00001750: 5265 6665 7265 6e63 696e 6746 696c 655f  ReferencingFile_
-00001760: 280a 2020 2020 2020 2020 2320 2020 2020  (.        #     
-00001770: 222e 2f6d 6165 7374 726f 5f69 636f 6e2e  "./maestro_icon.
-00001780: 706e 6722 0a20 2020 2020 2020 2023 2029  png".        # )
-00001790: 0a20 2020 2020 2020 2023 206e 735f 6170  .        # ns_ap
-000017a0: 706c 6963 6174 696f 6e2e 7365 7441 7070  plication.setApp
-000017b0: 6c69 6361 7469 6f6e 4963 6f6e 496d 6167  licationIconImag
-000017c0: 655f 286c 6f67 6f5f 6e73 5f69 6d61 6765  e_(logo_ns_image
-000017d0: 290a 2020 2020 2020 2020 6e73 5f61 7070  ).        ns_app
-000017e0: 6c69 6361 7469 6f6e 2e73 6574 4163 7469  lication.setActi
-000017f0: 7661 7469 6f6e 506f 6c69 6379 5f28 0a20  vationPolicy_(. 
-00001800: 2020 2020 2020 2020 2020 204e 5341 7070             NSApp
-00001810: 6c69 6361 7469 6f6e 4163 7469 7661 7469  licationActivati
-00001820: 6f6e 506f 6c69 6379 5072 6f68 6962 6974  onPolicyProhibit
-00001830: 6564 0a20 2020 2020 2020 2029 0a0a 2020  ed.        )..  
-00001840: 2020 2020 2020 2320 4e4f 5445 3a20 6b65        # NOTE: ke
-00001850: 6570 2072 6566 2074 6f20 6465 6c65 6761  ep ref to delega
-00001860: 7465 206f 626a 6563 742c 2073 6574 4465  te object, setDe
-00001870: 6c65 6761 7465 5f20 646f 6573 6e27 7420  legate_ doesn't 
-00001880: 7265 7461 696e 0a20 2020 2020 2020 2064  retain.        d
-00001890: 656c 6567 6174 6520 3d20 4170 7044 656c  elegate = AppDel
-000018a0: 6567 6174 652e 616c 6c6f 6328 292e 696e  egate.alloc().in
-000018b0: 6974 2829 0a20 2020 2020 2020 204e 5341  it().        NSA
-000018c0: 7070 2829 2e73 6574 4465 6c65 6761 7465  pp().setDelegate
-000018d0: 5f28 6465 6c65 6761 7465 290a 0a20 2020  _(delegate)..   
-000018e0: 2020 2020 2061 7070 5f68 656c 7065 725f       app_helper_
-000018f0: 7072 6f63 6573 7320 3d20 6d75 6c74 6970  process = multip
-00001900: 726f 6365 7373 696e 672e 5072 6f63 6573  rocessing.Proces
-00001910: 7328 0a20 2020 2020 2020 2020 2020 2064  s(.            d
-00001920: 6165 6d6f 6e3d 5472 7565 2c0a 2020 2020  aemon=True,.    
-00001930: 2020 2020 2020 2020 7461 7267 6574 3d61          target=a
-00001940: 7070 5f68 656c 7065 725f 6c6f 6f70 2c0a  pp_helper_loop,.
-00001950: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00001960: 2020 6170 705f 6865 6c70 6572 5f70 726f    app_helper_pro
-00001970: 6365 7373 2e73 7461 7274 2829 0a0a 2020  cess.start()..  
-00001980: 2020 7072 6576 5f76 6f6c 756d 6520 3d20    prev_volume = 
-00001990: 766f 6c75 6d65 0a20 2020 2077 6869 6c65  volume.    while
-000019a0: 2070 6c61 7965 725f 6f75 7470 7574 2e69   player_output.i
-000019b0: 2069 6e20 7261 6e67 6528 6c65 6e28 706c   in range(len(pl
-000019c0: 6179 6572 5f6f 7574 7075 742e 706c 6179  ayer_output.play
-000019d0: 6c69 7374 2929 3a0a 2020 2020 2020 2020  list)):.        
-000019e0: 736f 6e67 5f70 6174 6820 3d20 6f73 2e70  song_path = os.p
-000019f0: 6174 682e 6a6f 696e 280a 2020 2020 2020  ath.join(.      
-00001a00: 2020 2020 2020 534f 4e47 535f 4449 522c        SONGS_DIR,
-00001a10: 2070 6c61 7965 725f 6f75 7470 7574 2e70   player_output.p
-00001a20: 6c61 796c 6973 745b 706c 6179 6572 5f6f  laylist[player_o
-00001a30: 7574 7075 742e 695d 5b31 5d0a 2020 2020  utput.i][1].    
-00001a40: 2020 2020 290a 0a20 2020 2020 2020 2070      )..        p
-00001a50: 6c61 7962 6163 6b20 3d20 506c 6179 6261  layback = Playba
-00001a60: 636b 2829 0a20 2020 2020 2020 2070 6c61  ck().        pla
-00001a70: 7962 6163 6b2e 6c6f 6164 5f66 696c 6528  yback.load_file(
-00001a80: 736f 6e67 5f70 6174 6829 0a0a 2020 2020  song_path)..    
-00001a90: 2020 2020 636c 6970 5f73 7472 696e 6720      clip_string 
-00001aa0: 3d20 706c 6179 6572 5f6f 7574 7075 742e  = player_output.
-00001ab0: 706c 6179 6c69 7374 5b70 6c61 7965 725f  playlist[player_
-00001ac0: 6f75 7470 7574 2e69 5d5b 335d 0a20 2020  output.i][3].   
-00001ad0: 2020 2020 2069 6620 636c 6970 5f73 7472       if clip_str
-00001ae0: 696e 673a 0a20 2020 2020 2020 2020 2020  ing:.           
-00001af0: 2070 6c61 7965 725f 6f75 7470 7574 2e63   player_output.c
-00001b00: 6c69 7020 3d20 7475 706c 6528 0a20 2020  lip = tuple(.   
-00001b10: 2020 2020 2020 2020 2020 2020 206d 6170               map
-00001b20: 2866 6c6f 6174 2c20 706c 6179 6572 5f6f  (float, player_o
-00001b30: 7574 7075 742e 706c 6179 6c69 7374 5b70  utput.playlist[p
-00001b40: 6c61 7965 725f 6f75 7470 7574 2e69 5d5b  layer_output.i][
-00001b50: 335d 2e73 706c 6974 2829 290a 2020 2020  3].split()).    
-00001b60: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00001b70: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00001b80: 2020 2020 706c 6179 6572 5f6f 7574 7075      player_outpu
-00001b90: 742e 636c 6970 203d 2030 2c20 706c 6179  t.clip = 0, play
-00001ba0: 6261 636b 2e64 7572 6174 696f 6e0a 0a20  back.duration.. 
-00001bb0: 2020 2020 2020 2070 6c61 7965 725f 6f75         player_ou
-00001bc0: 7470 7574 2e70 6175 7365 6420 3d20 4661  tput.paused = Fa
-00001bd0: 6c73 650a 2020 2020 2020 2020 706c 6179  lse.        play
-00001be0: 6572 5f6f 7574 7075 742e 6475 7261 7469  er_output.durati
-00001bf0: 6f6e 203d 2066 756c 6c5f 6475 7261 7469  on = full_durati
-00001c00: 6f6e 203d 2070 6c61 7962 6163 6b2e 6475  on = playback.du
-00001c10: 7261 7469 6f6e 0a0a 2020 2020 2020 2020  ration..        
-00001c20: 6966 2073 7973 2e70 6c61 7466 6f72 6d20  if sys.platform 
-00001c30: 3d3d 2022 6461 7277 696e 2220 616e 6420  == "darwin" and 
-00001c40: 6361 6e5f 6d61 635f 6e6f 775f 706c 6179  can_mac_now_play
-00001c50: 696e 673a 0a20 2020 2020 2020 2020 2020  ing:.           
-00001c60: 206d 6163 5f6e 6f77 5f70 6c61 7969 6e67   mac_now_playing
-00001c70: 2e70 6175 7365 6420 3d20 4661 6c73 650a  .paused = False.
-00001c80: 2020 2020 2020 2020 2020 2020 6d61 635f              mac_
-00001c90: 6e6f 775f 706c 6179 696e 672e 706f 7320  now_playing.pos 
-00001ca0: 3d20 300a 2020 2020 2020 2020 2020 2020  = 0.            
-00001cb0: 6d61 635f 6e6f 775f 706c 6179 696e 672e  mac_now_playing.
-00001cc0: 6c65 6e67 7468 203d 2070 6c61 7965 725f  length = player_
-00001cd0: 6f75 7470 7574 2e64 7572 6174 696f 6e0a  output.duration.
-00001ce0: 0a20 2020 2020 2020 2020 2020 206d 756c  .            mul
-00001cf0: 7469 7072 6f63 6573 7369 6e67 5f70 7574  tiprocessing_put
-00001d00: 5f77 6f72 6428 0a20 2020 2020 2020 2020  _word(.         
-00001d10: 2020 2020 2020 206d 6163 5f6e 6f77 5f70         mac_now_p
-00001d20: 6c61 7969 6e67 2e74 6974 6c65 5f71 7565  laying.title_que
-00001d30: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-00001d40: 2020 2020 706c 6179 6572 5f6f 7574 7075      player_outpu
-00001d50: 742e 706c 6179 6c69 7374 5b70 6c61 7965  t.playlist[playe
-00001d60: 725f 6f75 7470 7574 2e69 5d5b 315d 2c0a  r_output.i][1],.
-00001d70: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00001d80: 2020 2020 2020 2020 2020 6d75 6c74 6970            multip
-00001d90: 726f 6365 7373 696e 675f 7075 745f 776f  rocessing_put_wo
-00001da0: 7264 280a 2020 2020 2020 2020 2020 2020  rd(.            
-00001db0: 2020 2020 6d61 635f 6e6f 775f 706c 6179      mac_now_play
-00001dc0: 696e 672e 6172 7469 7374 5f71 7565 7565  ing.artist_queue
-00001dd0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001de0: 2020 706c 6179 6572 5f6f 7574 7075 742e    player_output.
-00001df0: 706c 6179 6c69 7374 5b70 6c61 7965 725f  playlist[player_
-00001e00: 6f75 7470 7574 2e69 5d5b 2d33 5d2c 0a20  output.i][-3],. 
-00001e10: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-00001e20: 2020 2020 2020 2020 2020 7570 6461 7465            update
-00001e30: 5f6e 6f77 5f70 6c61 7969 6e67 203d 2054  _now_playing = T
-00001e40: 7275 650a 0a20 2020 2020 2020 2069 6620  rue..        if 
-00001e50: 706c 6179 6572 5f6f 7574 7075 742e 7570  player_output.up
-00001e60: 6461 7465 5f64 6973 636f 7264 3a0a 2020  date_discord:.  
-00001e70: 2020 2020 2020 2020 2020 6d75 6c74 6970            multip
-00001e80: 726f 6365 7373 696e 675f 7075 745f 776f  rocessing_put_wo
-00001e90: 7264 280a 2020 2020 2020 2020 2020 2020  rd(.            
-00001ea0: 2020 2020 6469 7363 6f72 645f 7469 746c      discord_titl
-00001eb0: 655f 7175 6575 652c 2070 6c61 7965 725f  e_queue, player_
-00001ec0: 6f75 7470 7574 2e70 6c61 796c 6973 745b  output.playlist[
-00001ed0: 706c 6179 6572 5f6f 7574 7075 742e 695d  player_output.i]
-00001ee0: 5b31 5d0a 2020 2020 2020 2020 2020 2020  [1].            
-00001ef0: 290a 2020 2020 2020 2020 2020 2020 6d75  ).            mu
-00001f00: 6c74 6970 726f 6365 7373 696e 675f 7075  ltiprocessing_pu
-00001f10: 745f 776f 7264 280a 2020 2020 2020 2020  t_word(.        
-00001f20: 2020 2020 2020 2020 6469 7363 6f72 645f          discord_
-00001f30: 6172 7469 7374 5f71 7565 7565 2c0a 2020  artist_queue,.  
-00001f40: 2020 2020 2020 2020 2020 2020 2020 706c                pl
-00001f50: 6179 6572 5f6f 7574 7075 742e 706c 6179  ayer_output.play
-00001f60: 6c69 7374 5b70 6c61 7965 725f 6f75 7470  list[player_outp
-00001f70: 7574 2e69 5d5b 2d33 5d2c 0a20 2020 2020  ut.i][-3],.     
-00001f80: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-00001f90: 2020 706c 6179 6261 636b 2e70 6c61 7928    playback.play(
-00001fa0: 290a 0a20 2020 2020 2020 2069 6620 706c  )..        if pl
-00001fb0: 6179 6572 5f6f 7574 7075 742e 636c 6970  ayer_output.clip
-00001fc0: 5f6d 6f64 653a 0a20 2020 2020 2020 2020  _mode:.         
-00001fd0: 2020 2063 6c69 705f 7374 6172 742c 2063     clip_start, c
-00001fe0: 6c69 705f 656e 6420 3d20 706c 6179 6572  lip_end = player
-00001ff0: 5f6f 7574 7075 742e 636c 6970 0a20 2020  _output.clip.   
-00002000: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
-00002010: 6f75 7470 7574 2e64 7572 6174 696f 6e20  output.duration 
-00002020: 3d20 636c 6970 5f65 6e64 202d 2063 6c69  = clip_end - cli
-00002030: 705f 7374 6172 740a 2020 2020 2020 2020  p_start.        
-00002040: 2020 2020 706c 6179 6261 636b 2e73 6565      playback.see
-00002050: 6b28 636c 6970 5f73 7461 7274 290a 2020  k(clip_start).  
-00002060: 2020 2020 2020 2020 2020 6966 2073 7973            if sys
-00002070: 2e70 6c61 7466 6f72 6d20 3d3d 2022 6461  .platform == "da
-00002080: 7277 696e 2220 616e 6420 6361 6e5f 6d61  rwin" and can_ma
-00002090: 635f 6e6f 775f 706c 6179 696e 673a 0a20  c_now_playing:. 
-000020a0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-000020b0: 6163 5f6e 6f77 5f70 6c61 7969 6e67 2e70  ac_now_playing.p
-000020c0: 6f73 203d 2072 6f75 6e64 2870 6c61 7962  os = round(playb
-000020d0: 6163 6b2e 6375 7272 5f70 6f73 290a 2020  ack.curr_pos).  
-000020e0: 2020 2020 2020 2020 2020 6c61 7374 5f74            last_t
-000020f0: 696d 6573 7461 6d70 203d 2070 6c61 7962  imestamp = playb
-00002100: 6163 6b2e 6375 7272 5f70 6f73 0a0a 2020  ack.curr_pos..  
-00002110: 2020 2020 2020 7374 6172 745f 7469 6d65        start_time
-00002120: 203d 2070 6175 7365 5f73 7461 7274 203d   = pause_start =
-00002130: 2074 696d 6528 290a 2020 2020 2020 2020   time().        
-00002140: 706c 6179 6261 636b 2e73 6574 5f76 6f6c  playback.set_vol
-00002150: 756d 6528 706c 6179 6572 5f6f 7574 7075  ume(player_outpu
-00002160: 742e 766f 6c75 6d65 290a 0a20 2020 2020  t.volume)..     
-00002170: 2020 206c 6173 745f 7469 6d65 7374 616d     last_timestam
-00002180: 7020 3d20 706c 6179 6261 636b 2e63 7572  p = playback.cur
-00002190: 725f 706f 730a 2020 2020 2020 2020 6e65  r_pos.        ne
-000021a0: 7874 5f73 6f6e 6720 3d20 3120 2023 202d  xt_song = 1  # -
-000021b0: 3120 6966 2067 6f69 6e67 2062 6163 6b2c  1 if going back,
-000021c0: 2030 2069 6620 7265 7374 6172 7469 6e67   0 if restarting
-000021d0: 2c20 2b31 2069 6620 6e65 7874 2073 6f6e  , +1 if next son
-000021e0: 670a 2020 2020 2020 2020 706c 6179 6572  g.        player
-000021f0: 5f6f 7574 7075 742e 656e 6469 6e67 203d  _output.ending =
-00002200: 2046 616c 7365 0a20 2020 2020 2020 2077   False.        w
-00002210: 6869 6c65 2054 7275 653a 0a20 2020 2020  hile True:.     
-00002220: 2020 2020 2020 2069 6620 6e6f 7420 706c         if not pl
-00002230: 6179 6261 636b 2e61 6374 6976 6520 6f72  ayback.active or
-00002240: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
-00002250: 2020 2070 6c61 7965 725f 6f75 7470 7574     player_output
-00002260: 2e63 6c69 705f 6d6f 6465 0a20 2020 2020  .clip_mode.     
-00002270: 2020 2020 2020 2020 2020 2061 6e64 2070             and p
-00002280: 6c61 7962 6163 6b2e 6375 7272 5f70 6f73  layback.curr_pos
-00002290: 203e 2070 6c61 7965 725f 6f75 7470 7574   > player_output
-000022a0: 2e63 6c69 705b 315d 0a20 2020 2020 2020  .clip[1].       
-000022b0: 2020 2020 2029 3a0a 2020 2020 2020 2020       ):.        
-000022c0: 2020 2020 2020 2020 6e65 7874 5f73 6f6e          next_son
-000022d0: 6720 3d20 6e6f 7420 706c 6179 6572 5f6f  g = not player_o
-000022e0: 7574 7075 742e 6c6f 6f70 696e 675f 6375  utput.looping_cu
-000022f0: 7272 656e 745f 736f 6e67 0a20 2020 2020  rrent_song.     
-00002300: 2020 2020 2020 2020 2020 2062 7265 616b             break
-00002310: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-00002320: 6661 6465 2069 6e20 6669 7273 7420 3220  fade in first 2 
-00002330: 7365 636f 6e64 7320 6f66 2063 6c69 700a  seconds of clip.
-00002340: 2020 2020 2020 2020 2020 2020 6966 2028              if (
-00002350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002360: 2070 6c61 7965 725f 6f75 7470 7574 2e63   player_output.c
-00002370: 6c69 705f 6d6f 6465 0a20 2020 2020 2020  lip_mode.       
-00002380: 2020 2020 2020 2020 2061 6e64 2063 6c69           and cli
-00002390: 705f 7374 6172 7420 213d 2030 2020 2320  p_start != 0  # 
-000023a0: 6966 2063 6c69 7020 646f 6573 6e27 7420  if clip doesn't 
-000023b0: 7374 6172 7420 6174 2062 6567 696e 6e69  start at beginni
-000023c0: 6e67 0a20 2020 2020 2020 2020 2020 2020  ng.             
-000023d0: 2020 2061 6e64 2063 6c69 705f 656e 6420     and clip_end 
-000023e0: 2d20 636c 6970 5f73 7461 7274 203e 2035  - clip_start > 5
-000023f0: 2020 2320 6966 2063 6c69 7020 6973 206c    # if clip is l
-00002400: 6f6e 6765 7220 7468 616e 2035 2073 6563  onger than 5 sec
-00002410: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-00002420: 2020 616e 6420 706c 6179 6261 636b 2e63    and playback.c
-00002430: 7572 725f 706f 7320 3c20 636c 6970 5f73  urr_pos < clip_s
-00002440: 7461 7274 202b 2032 0a20 2020 2020 2020  tart + 2.       
-00002450: 2020 2020 2029 3a0a 2020 2020 2020 2020       ):.        
-00002460: 2020 2020 2020 2020 706c 6179 6261 636b          playback
-00002470: 2e73 6574 5f76 6f6c 756d 6528 0a20 2020  .set_volume(.   
-00002480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002490: 2070 6c61 7965 725f 6f75 7470 7574 2e76   player_output.v
-000024a0: 6f6c 756d 6520 2a20 2870 6c61 7962 6163  olume * (playbac
-000024b0: 6b2e 6375 7272 5f70 6f73 202d 2063 6c69  k.curr_pos - cli
-000024c0: 705f 7374 6172 7429 202f 2032 0a20 2020  p_start) / 2.   
-000024d0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-000024e0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-000024f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002500: 2070 6c61 7962 6163 6b2e 7365 745f 766f   playback.set_vo
-00002510: 6c75 6d65 2870 6c61 7965 725f 6f75 7470  lume(player_outp
-00002520: 7574 2e76 6f6c 756d 6529 0a0a 2020 2020  ut.volume)..    
-00002530: 2020 2020 2020 2020 6966 2073 7973 2e70          if sys.p
-00002540: 6c61 7466 6f72 6d20 3d3d 2022 6461 7277  latform == "darw
-00002550: 696e 2220 616e 6420 6361 6e5f 6d61 635f  in" and can_mac_
-00002560: 6e6f 775f 706c 6179 696e 673a 0a20 2020  now_playing:.   
-00002570: 2020 2020 2020 2020 2020 2020 2074 7279               try
-00002580: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00002590: 2020 2020 2020 6966 2075 7064 6174 655f        if update_
-000025a0: 6e6f 775f 706c 6179 696e 673a 0a20 2020  now_playing:.   
-000025b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025c0: 2020 2020 206d 6163 5f6e 6f77 5f70 6c61       mac_now_pla
-000025d0: 7969 6e67 2e75 7064 6174 6528 290a 2020  ying.update().  
-000025e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025f0: 2020 2020 2020 7570 6461 7465 5f6e 6f77        update_now
-00002600: 5f70 6c61 7969 6e67 203d 2046 616c 7365  _playing = False
-00002610: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002620: 2020 2020 204e 5352 756e 4c6f 6f70 2e63       NSRunLoop.c
-00002630: 7572 7265 6e74 5275 6e4c 6f6f 7028 292e  urrentRunLoop().
-00002640: 7275 6e55 6e74 696c 4461 7465 5f28 0a20  runUntilDate_(. 
-00002650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002660: 2020 2020 2020 204e 5344 6174 652e 6461         NSDate.da
-00002670: 7465 5769 7468 5469 6d65 496e 7465 7276  teWithTimeInterv
-00002680: 616c 5369 6e63 654e 6f77 5f28 302e 3035  alSinceNow_(0.05
-00002690: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000026a0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-000026b0: 2020 2020 2020 2020 6578 6365 7074 3a20          except: 
-000026c0: 2023 2070 796c 696e 743a 2064 6973 6162   # pylint: disab
-000026d0: 6c65 3d62 6172 652d 6578 6365 7074 0a20  le=bare-except. 
-000026e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026f0: 2020 2063 616e 5f6d 6163 5f6e 6f77 5f70     can_mac_now_p
-00002700: 6c61 7969 6e67 203d 2046 616c 7365 0a0a  laying = False..
-00002710: 2020 2020 2020 2020 2020 2020 6966 2028              if (
-00002720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002730: 2073 7973 2e70 6c61 7466 6f72 6d20 3d3d   sys.platform ==
-00002740: 2022 6461 7277 696e 220a 2020 2020 2020   "darwin".      
-00002750: 2020 2020 2020 2020 2020 616e 6420 6361            and ca
-00002760: 6e5f 6d61 635f 6e6f 775f 706c 6179 696e  n_mac_now_playin
-00002770: 670a 2020 2020 2020 2020 2020 2020 2020  g.              
-00002780: 2020 616e 6420 6e6f 7420 6d61 635f 6e6f    and not mac_no
-00002790: 775f 706c 6179 696e 672e 712e 656d 7074  w_playing.q.empt
-000027a0: 7928 290a 2020 2020 2020 2020 2020 2020  y().            
-000027b0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000027c0: 2020 2063 203d 206d 6163 5f6e 6f77 5f70     c = mac_now_p
-000027d0: 6c61 7969 6e67 2e71 2e67 6574 2829 0a20  laying.q.get(). 
-000027e0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000027f0: 6620 6320 696e 2022 6e4e 223a 0a20 2020  f c in "nN":.   
-00002800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002810: 2069 6620 280a 2020 2020 2020 2020 2020   if (.          
-00002820: 2020 2020 2020 2020 2020 2020 2020 706c                pl
-00002830: 6179 6572 5f6f 7574 7075 742e 6920 3d3d  ayer_output.i ==
-00002840: 206c 656e 2870 6c61 7965 725f 6f75 7470   len(player_outp
-00002850: 7574 2e70 6c61 796c 6973 7429 202d 2031  ut.playlist) - 1
-00002860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002870: 2020 2020 2020 2020 2061 6e64 206e 6f74           and not
-00002880: 206c 6f6f 700a 2020 2020 2020 2020 2020   loop.          
-00002890: 2020 2020 2020 2020 2020 293a 0a20 2020            ):.   
-000028a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028b0: 2020 2020 2070 6173 730a 2020 2020 2020       pass.      
-000028c0: 2020 2020 2020 2020 2020 2020 2020 656c                el
-000028d0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-000028e0: 2020 2020 2020 2020 2020 2020 6e65 7874              next
-000028f0: 5f73 6f6e 6720 3d20 310a 2020 2020 2020  _song = 1.      
-00002900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002910: 2020 706c 6179 6261 636b 2e73 746f 7028    playback.stop(
-00002920: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00002930: 2020 2020 2020 2020 2020 6272 6561 6b0a            break.
-00002940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002950: 656c 6966 2063 2069 6e20 2262 4222 3a0a  elif c in "bB":.
-00002960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002970: 2020 2020 6966 2070 6c61 7965 725f 6f75      if player_ou
-00002980: 7470 7574 2e69 203d 3d20 303a 0a20 2020  tput.i == 0:.   
-00002990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029a0: 2020 2020 2070 6173 730a 2020 2020 2020       pass.      
-000029b0: 2020 2020 2020 2020 2020 2020 2020 656c                el
-000029c0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-000029d0: 2020 2020 2020 2020 2020 2020 6e65 7874              next
-000029e0: 5f73 6f6e 6720 3d20 2d31 0a20 2020 2020  _song = -1.     
-000029f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a00: 2020 2070 6c61 7962 6163 6b2e 7374 6f70     playback.stop
-00002a10: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00002a20: 2020 2020 2020 2020 2020 2062 7265 616b             break
-00002a30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002a40: 2065 6c69 6620 6320 696e 2022 7252 223a   elif c in "rR":
-00002a50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002a60: 2020 2020 2070 6c61 7962 6163 6b2e 7374       playback.st
-00002a70: 6f70 2829 0a20 2020 2020 2020 2020 2020  op().           
-00002a80: 2020 2020 2020 2020 206e 6578 745f 736f           next_so
-00002a90: 6e67 203d 2030 0a20 2020 2020 2020 2020  ng = 0.         
-00002aa0: 2020 2020 2020 2020 2020 2062 7265 616b             break
-00002ab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002ac0: 2065 6c69 6620 6320 696e 2022 7151 223a   elif c in "qQ":
-00002ad0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002ae0: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
-00002af0: 7574 2e65 6e64 696e 6720 3d20 5472 7565  ut.ending = True
-00002b00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002b10: 2020 2020 2062 7265 616b 0a20 2020 2020       break.     
-00002b20: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00002b30: 6320 3d3d 2022 2022 3a0a 2020 2020 2020  c == " ":.      
-00002b40: 2020 2020 2020 2020 2020 2020 2020 706c                pl
-00002b50: 6179 6572 5f6f 7574 7075 742e 7061 7573  ayer_output.paus
-00002b60: 6564 203d 206e 6f74 2070 6c61 7965 725f  ed = not player_
-00002b70: 6f75 7470 7574 2e70 6175 7365 640a 0a20  output.paused.. 
-00002b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b90: 2020 2069 6620 706c 6179 6572 5f6f 7574     if player_out
-00002ba0: 7075 742e 7061 7573 6564 3a0a 2020 2020  put.paused:.    
-00002bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002bc0: 2020 2020 706c 6179 6261 636b 2e70 6175      playback.pau
-00002bd0: 7365 2829 0a20 2020 2020 2020 2020 2020  se().           
-00002be0: 2020 2020 2020 2020 2020 2020 2070 6175               pau
-00002bf0: 7365 5f73 7461 7274 203d 2074 696d 6528  se_start = time(
-00002c00: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00002c10: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00002c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c30: 2020 2020 706c 6179 6261 636b 2e72 6573      playback.res
-00002c40: 756d 6528 290a 2020 2020 2020 2020 2020  ume().          
-00002c50: 2020 2020 2020 2020 2020 2020 2020 7374                st
-00002c60: 6172 745f 7469 6d65 202b 3d20 7469 6d65  art_time += time
-00002c70: 2829 202d 2070 6175 7365 5f73 7461 7274  () - pause_start
-00002c80: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002c90: 2020 2020 2020 6966 2073 7973 2e70 6c61        if sys.pla
-00002ca0: 7466 6f72 6d20 3d3d 2022 6461 7277 696e  tform == "darwin
-00002cb0: 2220 616e 6420 6361 6e5f 6d61 635f 6e6f  " and can_mac_no
-00002cc0: 775f 706c 6179 696e 673a 0a20 2020 2020  w_playing:.     
-00002cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ce0: 2020 206d 6163 5f6e 6f77 5f70 6c61 7969     mac_now_playi
-00002cf0: 6e67 2e70 6175 7365 6420 3d20 706c 6179  ng.paused = play
-00002d00: 6572 5f6f 7574 7075 742e 7061 7573 6564  er_output.paused
-00002d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002d20: 2020 2020 2020 2020 2069 6620 706c 6179           if play
-00002d30: 6572 5f6f 7574 7075 742e 7061 7573 6564  er_output.paused
-00002d40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00002d50: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
-00002d60: 635f 6e6f 775f 706c 6179 696e 672e 7061  c_now_playing.pa
-00002d70: 7573 6528 290a 2020 2020 2020 2020 2020  use().          
-00002d80: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00002d90: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00000020: 6d70 6f72 7420 6a73 6f6e 0a69 6d70 6f72  mport json.impor
+00000030: 7420 6d75 6c74 6970 726f 6365 7373 696e  t multiprocessin
+00000040: 670a 696d 706f 7274 206f 730a 696d 706f  g.import os.impo
+00000050: 7274 2073 7562 7072 6f63 6573 730a 696d  rt subprocess.im
+00000060: 706f 7274 2073 7973 0a0a 696d 706f 7274  port sys..import
+00000070: 2063 6c69 636b 0a69 6d70 6f72 7420 6d75   click.import mu
+00000080: 7369 635f 7461 670a 0a66 726f 6d20 636f  sic_tag..from co
+00000090: 6c6c 6563 7469 6f6e 7320 696d 706f 7274  llections import
+000000a0: 2064 6566 6175 6c74 6469 6374 0a66 726f   defaultdict.fro
+000000b0: 6d20 7175 6575 6520 696d 706f 7274 2051  m queue import Q
+000000c0: 7565 7565 0a66 726f 6d20 7261 6e64 6f6d  ueue.from random
+000000d0: 2069 6d70 6f72 7420 7368 7566 666c 652c   import shuffle,
+000000e0: 2072 616e 6469 6e74 0a66 726f 6d20 7368   randint.from sh
+000000f0: 7574 696c 2069 6d70 6f72 7420 6d6f 7665  util import move
+00000100: 0a66 726f 6d20 7469 6d65 2069 6d70 6f72  .from time impor
+00000110: 7420 736c 6565 702c 2074 696d 650a 0a66  t sleep, time..f
+00000120: 726f 6d20 6963 6f6e 2069 6d70 6f72 7420  rom icon import 
+00000130: 696d 670a 0a66 726f 6d20 6a75 7374 5f70  img..from just_p
+00000140: 6c61 7962 6163 6b20 696d 706f 7274 2050  layback import P
+00000150: 6c61 7962 6163 6b0a 0a63 616e 5f75 7064  layback..can_upd
+00000160: 6174 655f 6469 7363 6f72 6420 3d20 5472  ate_discord = Tr
+00000170: 7565 0a74 7279 3a0a 2020 2020 696d 706f  ue.try:.    impo
+00000180: 7274 2070 7970 7265 7365 6e63 650a 6578  rt pypresence.ex
+00000190: 6365 7074 2049 6d70 6f72 7445 7272 6f72  cept ImportError
+000001a0: 3a0a 2020 2020 6361 6e5f 7570 6461 7465  :.    can_update
+000001b0: 5f64 6973 636f 7264 203d 2046 616c 7365  _discord = False
+000001c0: 0a0a 6672 6f6d 2068 656c 7065 7273 2069  ..from helpers i
+000001d0: 6d70 6f72 7420 2a20 2023 2070 796c 696e  mport *  # pylin
+000001e0: 743a 2064 6973 6162 6c65 3d77 696c 6463  t: disable=wildc
+000001f0: 6172 642d 696d 706f 7274 2c75 6e75 7365  ard-import,unuse
+00000200: 642d 7769 6c64 6361 7264 2d69 6d70 6f72  d-wildcard-impor
+00000210: 740a 0a69 6620 7379 732e 706c 6174 666f  t..if sys.platfo
+00000220: 726d 203d 3d20 2264 6172 7769 6e22 3a0a  rm == "darwin":.
+00000230: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+00000240: 2023 2070 796c 696e 743a 2064 6973 6162   # pylint: disab
+00000250: 6c65 3d6e 6f2d 6e61 6d65 2d69 6e2d 6d6f  le=no-name-in-mo
+00000260: 6475 6c65 2c69 6d70 6f72 742d 6572 726f  dule,import-erro
+00000270: 720a 2020 2020 2020 2020 6672 6f6d 2041  r.        from A
+00000280: 7070 4b69 7420 696d 706f 7274 2028 0a20  ppKit import (. 
+00000290: 2020 2020 2020 2020 2020 204e 5341 7070             NSApp
+000002a0: 2c0a 2020 2020 2020 2020 2020 2020 4e53  ,.            NS
+000002b0: 4170 706c 6963 6174 696f 6e2c 0a20 2020  Application,.   
+000002c0: 2020 2020 2020 2020 204e 5341 7070 6c69           NSAppli
+000002d0: 6361 7469 6f6e 4163 7469 7661 7469 6f6e  cationActivation
+000002e0: 506f 6c69 6379 5072 6f68 6962 6974 6564  PolicyProhibited
+000002f0: 2c0a 2020 2020 2020 2020 2020 2020 4e53  ,.            NS
+00000300: 4461 7465 2c0a 2020 2020 2020 2020 2020  Date,.          
+00000310: 2020 4e53 4f62 6a65 6374 2c0a 2020 2020    NSObject,.    
+00000320: 2020 2020 2020 2020 4e53 5275 6e4c 6f6f          NSRunLoo
+00000330: 702c 0a20 2020 2020 2020 2029 0a0a 2020  p,.        )..  
+00000340: 2020 2020 2020 2320 6672 6f6d 204d 6564        # from Med
+00000350: 6961 506c 6179 6572 2069 6d70 6f72 7420  iaPlayer import 
+00000360: 4d50 4e6f 7750 6c61 7969 6e67 496e 666f  MPNowPlayingInfo
+00000370: 5072 6f70 6572 7479 456c 6170 7365 6450  PropertyElapsedP
+00000380: 6c61 7962 6163 6b54 696d 650a 2020 2020  laybackTime.    
+00000390: 2020 2020 6672 6f6d 2050 794f 626a 4354      from PyObjCT
+000003a0: 6f6f 6c73 2069 6d70 6f72 7420 4170 7048  ools import AppH
+000003b0: 656c 7065 720a 0a20 2020 2020 2020 2066  elper..        f
+000003c0: 726f 6d20 6d61 635f 7072 6573 656e 6365  rom mac_presence
+000003d0: 2069 6d70 6f72 7420 4d61 634e 6f77 506c   import MacNowPl
+000003e0: 6179 696e 670a 0a20 2020 2020 2020 2023  aying..        #
+000003f0: 2067 6c6f 6261 6c73 0a20 2020 2020 2020   globals.       
+00000400: 206d 6163 5f6e 6f77 5f70 6c61 7969 6e67   mac_now_playing
+00000410: 203d 204d 6163 4e6f 7750 6c61 7969 6e67   = MacNowPlaying
+00000420: 2829 0a20 2020 2020 2020 2063 6f76 6572  ().        cover
+00000430: 5f69 6d67 203d 2069 6d67 0a0a 2020 2020  _img = img..    
+00000440: 2020 2020 6361 6e5f 6d61 635f 6e6f 775f      can_mac_now_
+00000450: 706c 6179 696e 6720 3d20 5472 7565 0a20  playing = True. 
+00000460: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
+00000470: 696f 6e20 6173 2065 3a20 2023 2070 796c  ion as e:  # pyl
+00000480: 696e 743a 2064 6973 6162 6c65 3d62 6172  int: disable=bar
+00000490: 652d 6578 6365 7074 2c62 726f 6164 2d65  e-except,broad-e
+000004a0: 7863 6570 740a 2020 2020 2020 2020 2320  xcept.        # 
+000004b0: 7072 696e 7428 652c 2066 696c 653d 6f70  print(e, file=op
+000004c0: 656e 2822 6c6f 672e 7478 7422 2c20 2261  en("log.txt", "a
+000004d0: 2229 290a 2020 2020 2020 2020 6361 6e5f  ")).        can_
+000004e0: 6d61 635f 6e6f 775f 706c 6179 696e 6720  mac_now_playing 
+000004f0: 3d20 4661 6c73 650a 0a23 2065 6e64 7265  = False..# endre
+00000500: 6769 6f6e 0a0a 2320 7265 6769 6f6e 2075  gion..# region u
+00000510: 7469 6c69 7479 2066 756e 6374 696f 6e73  tility functions
+00000520: 2f63 6c61 7373 6573 0a0a 6966 2073 7973  /classes..if sys
+00000530: 2e70 6c61 7466 6f72 6d20 3d3d 2022 6461  .platform == "da
+00000540: 7277 696e 2220 616e 6420 6361 6e5f 6d61  rwin" and can_ma
+00000550: 635f 6e6f 775f 706c 6179 696e 673a 0a0a  c_now_playing:..
+00000560: 2020 2020 636c 6173 7320 4170 7044 656c      class AppDel
+00000570: 6567 6174 6528 4e53 4f62 6a65 6374 293a  egate(NSObject):
+00000580: 2020 2320 736f 2050 7974 686f 6e20 646f    # so Python do
+00000590: 6573 6e27 7420 626f 756e 6365 2069 6e20  esn't bounce in 
+000005a0: 7468 6520 646f 636b 0a20 2020 2020 2020  the dock.       
+000005b0: 2064 6566 2061 7070 6c69 6361 7469 6f6e   def application
+000005c0: 4469 6446 696e 6973 684c 6175 6e63 6869  DidFinishLaunchi
+000005d0: 6e67 5f28 7365 6c66 2c20 5f61 4e6f 7469  ng_(self, _aNoti
+000005e0: 6669 6361 7469 6f6e 293a 0a20 2020 2020  fication):.     
+000005f0: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
+00000600: 2020 2020 2064 6566 2073 6179 4865 6c6c       def sayHell
+00000610: 6f5f 2873 656c 662c 205f 7365 6e64 6572  o_(self, _sender
+00000620: 293a 0a20 2020 2020 2020 2020 2020 2070  ):.            p
+00000630: 6173 730a 0a20 2020 2064 6566 2061 7070  ass..    def app
+00000640: 5f68 656c 7065 725f 6c6f 6f70 2829 3a0a  _helper_loop():.
+00000650: 2020 2020 2020 2020 2320 6e73 5f61 7070          # ns_app
+00000660: 6c69 6361 7469 6f6e 203d 204e 5341 7070  lication = NSApp
+00000670: 6c69 6361 7469 6f6e 2e73 6861 7265 6441  lication.sharedA
+00000680: 7070 6c69 6361 7469 6f6e 2829 0a20 2020  pplication().   
+00000690: 2020 2020 2023 206c 6f67 6f5f 6e73 5f69       # logo_ns_i
+000006a0: 6d61 6765 203d 204e 5349 6d61 6765 2e61  mage = NSImage.a
+000006b0: 6c6c 6f63 2829 2e69 6e69 7442 7952 6566  lloc().initByRef
+000006c0: 6572 656e 6369 6e67 4669 6c65 5f28 0a20  erencingFile_(. 
+000006d0: 2020 2020 2020 2023 2020 2020 2022 2e2f         #     "./
+000006e0: 6d61 6573 7472 6f5f 6963 6f6e 2e70 6e67  maestro_icon.png
+000006f0: 220a 2020 2020 2020 2020 2320 290a 2020  ".        # ).  
+00000700: 2020 2020 2020 2320 6e73 5f61 7070 6c69        # ns_appli
+00000710: 6361 7469 6f6e 2e73 6574 4170 706c 6963  cation.setApplic
+00000720: 6174 696f 6e49 636f 6e49 6d61 6765 5f28  ationIconImage_(
+00000730: 6c6f 676f 5f6e 735f 696d 6167 6529 0a0a  logo_ns_image)..
+00000740: 2020 2020 2020 2020 2320 2320 7765 206d          # # we m
+00000750: 7573 7420 6b65 6570 2061 2072 6566 6572  ust keep a refer
+00000760: 656e 6365 2074 6f20 7468 6520 6465 6c65  ence to the dele
+00000770: 6761 7465 206f 626a 6563 7420 6f75 7273  gate object ours
+00000780: 656c 7665 732c 0a20 2020 2020 2020 2023  elves,.        #
+00000790: 2023 204e 5341 7070 2e73 6574 4465 6c65   # NSApp.setDele
+000007a0: 6761 7465 5f28 2920 646f 6573 6e27 7420  gate_() doesn't 
+000007b0: 7265 7461 696e 2069 742e 2041 206c 6f63  retain it. A loc
+000007c0: 616c 2076 6172 6961 626c 6520 6973 0a20  al variable is. 
+000007d0: 2020 2020 2020 2023 2023 2065 6e6f 7567         # # enoug
+000007e0: 6820 6865 7265 2e0a 2020 2020 2020 2020  h here..        
+000007f0: 2320 6465 6c65 6761 7465 203d 2041 7070  # delegate = App
+00000800: 4465 6c65 6761 7465 2e61 6c6c 6f63 2829  Delegate.alloc()
+00000810: 2e69 6e69 7428 290a 2020 2020 2020 2020  .init().        
+00000820: 2320 4e53 4170 7028 292e 7365 7444 656c  # NSApp().setDel
+00000830: 6567 6174 655f 2864 656c 6567 6174 6529  egate_(delegate)
+00000840: 0a0a 2020 2020 2020 2020 4170 7048 656c  ..        AppHel
+00000850: 7065 722e 7275 6e45 7665 6e74 4c6f 6f70  per.runEventLoop
+00000860: 2829 0a0a 0a64 6566 2064 6973 636f 7264  ()...def discord
+00000870: 5f70 7265 7365 6e63 655f 6c6f 6f70 2873  _presence_loop(s
+00000880: 6f6e 675f 6e61 6d65 5f71 7565 7565 2c20  ong_name_queue, 
+00000890: 6172 7469 7374 5f71 7565 7565 2c20 6469  artist_queue, di
+000008a0: 7363 6f72 645f 636f 6e6e 6563 7465 6429  scord_connected)
+000008b0: 3a0a 2020 2020 7472 793a 0a20 2020 2020  :.    try:.     
+000008c0: 2020 2064 6973 636f 7264 5f72 7063 203d     discord_rpc =
+000008d0: 2070 7970 7265 7365 6e63 652e 5072 6573   pypresence.Pres
+000008e0: 656e 6365 2863 6c69 656e 745f 6964 3d44  ence(client_id=D
+000008f0: 4953 434f 5244 5f49 4429 0a20 2020 2020  ISCORD_ID).     
+00000900: 2020 2064 6973 636f 7264 5f72 7063 2e63     discord_rpc.c
+00000910: 6f6e 6e65 6374 2829 0a20 2020 2020 2020  onnect().       
+00000920: 2064 6973 636f 7264 5f63 6f6e 6e65 6374   discord_connect
+00000930: 6564 2e76 616c 7565 203d 2031 0a20 2020  ed.value = 1.   
+00000940: 2065 7863 6570 743a 2020 2320 7079 6c69   except:  # pyli
+00000950: 6e74 3a20 6469 7361 626c 653d 6261 7265  nt: disable=bare
+00000960: 2d65 7863 6570 740a 2020 2020 2020 2020  -except.        
+00000970: 6469 7363 6f72 645f 636f 6e6e 6563 7465  discord_connecte
+00000980: 642e 7661 6c75 6520 3d20 300a 0a20 2020  d.value = 0..   
+00000990: 2077 6869 6c65 2054 7275 653a 0a20 2020   while True:.   
+000009a0: 2020 2020 2073 6f6e 675f 6e61 6d65 203d       song_name =
+000009b0: 2022 220a 2020 2020 2020 2020 6966 206e   "".        if n
+000009c0: 6f74 2073 6f6e 675f 6e61 6d65 5f71 7565  ot song_name_que
+000009d0: 7565 2e65 6d70 7479 2829 206f 7220 736f  ue.empty() or so
+000009e0: 6e67 5f6e 616d 653a 0a20 2020 2020 2020  ng_name:.       
+000009f0: 2020 2020 2077 6869 6c65 206e 6f74 2073       while not s
+00000a00: 6f6e 675f 6e61 6d65 5f71 7565 7565 2e65  ong_name_queue.e
+00000a10: 6d70 7479 2829 3a0a 2020 2020 2020 2020  mpty():.        
+00000a20: 2020 2020 2020 2020 736f 6e67 5f6e 616d          song_nam
+00000a30: 6520 3d20 2222 0a20 2020 2020 2020 2020  e = "".         
+00000a40: 2020 2020 2020 2063 203d 2073 6f6e 675f         c = song_
+00000a50: 6e61 6d65 5f71 7565 7565 2e67 6574 2829  name_queue.get()
+00000a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000a70: 2077 6869 6c65 2063 2021 3d20 225c 6e22   while c != "\n"
+00000a80: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00000a90: 2020 2020 2020 736f 6e67 5f6e 616d 6520        song_name 
+00000aa0: 2b3d 2063 0a20 2020 2020 2020 2020 2020  += c.           
+00000ab0: 2020 2020 2020 2020 2063 203d 2073 6f6e           c = son
+00000ac0: 675f 6e61 6d65 5f71 7565 7565 2e67 6574  g_name_queue.get
+00000ad0: 2829 0a0a 2020 2020 2020 2020 2020 2020  ()..            
+00000ae0: 6172 7469 7374 5f6e 616d 6520 3d20 2222  artist_name = ""
+00000af0: 0a20 2020 2020 2020 2020 2020 2077 6869  .            whi
+00000b00: 6c65 206e 6f74 2061 7274 6973 745f 7175  le not artist_qu
+00000b10: 6575 652e 656d 7074 7928 293a 0a20 2020  eue.empty():.   
+00000b20: 2020 2020 2020 2020 2020 2020 2061 7274               art
+00000b30: 6973 745f 6e61 6d65 203d 2022 220a 2020  ist_name = "".  
+00000b40: 2020 2020 2020 2020 2020 2020 2020 6320                c 
+00000b50: 3d20 6172 7469 7374 5f71 7565 7565 2e67  = artist_queue.g
+00000b60: 6574 2829 0a20 2020 2020 2020 2020 2020  et().           
+00000b70: 2020 2020 2077 6869 6c65 2063 2021 3d20       while c != 
+00000b80: 225c 6e22 3a0a 2020 2020 2020 2020 2020  "\n":.          
+00000b90: 2020 2020 2020 2020 2020 6172 7469 7374            artist
+00000ba0: 5f6e 616d 6520 2b3d 2063 0a20 2020 2020  _name += c.     
+00000bb0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00000bc0: 203d 2061 7274 6973 745f 7175 6575 652e   = artist_queue.
+00000bd0: 6765 7428 290a 0a20 2020 2020 2020 2020  get()..         
+00000be0: 2020 2061 7274 6973 745f 6e61 6d65 203d     artist_name =
+00000bf0: 2022 6279 2022 202b 2061 7274 6973 745f   "by " + artist_
+00000c00: 6e61 6d65 0a0a 2020 2020 2020 2020 2020  name..          
+00000c10: 2020 6966 2064 6973 636f 7264 5f63 6f6e    if discord_con
+00000c20: 6e65 6374 6564 2e76 616c 7565 3a0a 2020  nected.value:.  
+00000c30: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+00000c40: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
+00000c50: 2020 2020 2020 2064 6973 636f 7264 5f72         discord_r
+00000c60: 7063 2e75 7064 6174 6528 0a20 2020 2020  pc.update(.     
+00000c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c80: 2020 2064 6574 6169 6c73 3d73 6f6e 675f     details=song_
+00000c90: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
+00000ca0: 2020 2020 2020 2020 2020 2020 2020 7374                st
+00000cb0: 6174 653d 6172 7469 7374 5f6e 616d 652c  ate=artist_name,
+00000cc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000cd0: 2020 2020 2020 2020 206c 6172 6765 5f69           large_i
+00000ce0: 6d61 6765 3d22 6d61 6573 7472 6f2d 6963  mage="maestro-ic
+00000cf0: 6f6e 222c 0a20 2020 2020 2020 2020 2020  on",.           
+00000d00: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00000d10: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00000d20: 6f6e 675f 6e61 6d65 203d 2022 220a 2020  ong_name = "".  
+00000d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d40: 2020 6172 7469 7374 5f6e 616d 6520 3d20    artist_name = 
+00000d50: 2222 0a20 2020 2020 2020 2020 2020 2020  "".             
+00000d60: 2020 2020 2020 2073 6c65 6570 2831 3529         sleep(15)
+00000d70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000d80: 2065 7863 6570 743a 2020 2320 7079 6c69   except:  # pyli
+00000d90: 6e74 3a20 6469 7361 626c 653d 6261 7265  nt: disable=bare
+00000da0: 2d65 7863 6570 740a 2020 2020 2020 2020  -except.        
+00000db0: 2020 2020 2020 2020 2020 2020 6469 7363              disc
+00000dc0: 6f72 645f 636f 6e6e 6563 7465 642e 7661  ord_connected.va
+00000dd0: 6c75 6520 3d20 300a 2020 2020 2020 2020  lue = 0.        
+00000de0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00000df0: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
+00000e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e10: 2020 2064 6973 636f 7264 5f72 7063 203d     discord_rpc =
+00000e20: 2070 7970 7265 7365 6e63 652e 5072 6573   pypresence.Pres
+00000e30: 656e 6365 2863 6c69 656e 745f 6964 3d44  ence(client_id=D
+00000e40: 4953 434f 5244 5f49 4429 0a20 2020 2020  ISCORD_ID).     
+00000e50: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00000e60: 6973 636f 7264 5f72 7063 2e63 6f6e 6e65  iscord_rpc.conne
+00000e70: 6374 2829 0a20 2020 2020 2020 2020 2020  ct().           
+00000e80: 2020 2020 2020 2020 2064 6973 636f 7264           discord
+00000e90: 5f63 6f6e 6e65 6374 6564 2e76 616c 7565  _connected.value
+00000ea0: 203d 2031 0a20 2020 2020 2020 2020 2020   = 1.           
+00000eb0: 2020 2020 2065 7863 6570 743a 2020 2320       except:  # 
+00000ec0: 7079 6c69 6e74 3a20 6469 7361 626c 653d  pylint: disable=
+00000ed0: 6261 7265 2d65 7863 6570 740a 2020 2020  bare-except.    
+00000ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ef0: 7061 7373 0a0a 2020 2020 2020 2020 2020  pass..          
+00000f00: 2020 2020 2020 6966 2064 6973 636f 7264        if discord
+00000f10: 5f63 6f6e 6e65 6374 6564 2e76 616c 7565  _connected.value
+00000f20: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00000f30: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+00000f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f50: 2020 2064 6973 636f 7264 5f72 7063 2e75     discord_rpc.u
+00000f60: 7064 6174 6528 0a20 2020 2020 2020 2020  pdate(.         
+00000f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f80: 2020 2064 6574 6169 6c73 3d73 6f6e 675f     details=song_
+00000f90: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
+00000fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000fb0: 2020 7374 6174 653d 6172 7469 7374 5f6e    state=artist_n
+00000fc0: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
+00000fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000fe0: 206c 6172 6765 5f69 6d61 6765 3d22 6d61   large_image="ma
+00000ff0: 6573 7472 6f2d 6963 6f6e 222c 0a20 2020  estro-icon",.   
+00001000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001010: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00001020: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00001030: 6f6e 675f 6e61 6d65 203d 2022 220a 2020  ong_name = "".  
+00001040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001050: 2020 2020 2020 6172 7469 7374 5f6e 616d        artist_nam
+00001060: 6520 3d20 2222 0a20 2020 2020 2020 2020  e = "".         
+00001070: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00001080: 6c65 6570 2831 3529 0a20 2020 2020 2020  leep(15).       
+00001090: 2020 2020 2020 2020 2020 2020 2065 7863               exc
+000010a0: 6570 743a 2020 2320 7079 6c69 6e74 3a20  ept:  # pylint: 
+000010b0: 6469 7361 626c 653d 6261 7265 2d65 7863  disable=bare-exc
+000010c0: 6570 740a 2020 2020 2020 2020 2020 2020  ept.            
+000010d0: 2020 2020 2020 2020 2020 2020 6469 7363              disc
+000010e0: 6f72 645f 636f 6e6e 6563 7465 642e 7661  ord_connected.va
+000010f0: 6c75 6520 3d20 300a 2020 2020 2020 2020  lue = 0.        
+00001100: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00001110: 2020 6966 206e 6f74 2064 6973 636f 7264    if not discord
+00001120: 5f63 6f6e 6e65 6374 6564 2e76 616c 7565  _connected.value
+00001130: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00001140: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+00001150: 2020 2020 2020 2020 2020 2064 6973 636f             disco
+00001160: 7264 5f72 7063 203d 2070 7970 7265 7365  rd_rpc = pyprese
+00001170: 6e63 652e 5072 6573 656e 6365 2863 6c69  nce.Presence(cli
+00001180: 656e 745f 6964 3d44 4953 434f 5244 5f49  ent_id=DISCORD_I
+00001190: 4429 0a20 2020 2020 2020 2020 2020 2020  D).             
+000011a0: 2020 2020 2020 2064 6973 636f 7264 5f72         discord_r
+000011b0: 7063 2e63 6f6e 6e65 6374 2829 0a20 2020  pc.connect().   
+000011c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000011d0: 2064 6973 636f 7264 5f63 6f6e 6e65 6374   discord_connect
+000011e0: 6564 2e76 616c 7565 203d 2031 0a20 2020  ed.value = 1.   
+000011f0: 2020 2020 2020 2020 2020 2020 2065 7863               exc
+00001200: 6570 743a 2020 2320 7079 6c69 6e74 3a20  ept:  # pylint: 
+00001210: 6469 7361 626c 653d 6261 7265 2d65 7863  disable=bare-exc
+00001220: 6570 740a 2020 2020 2020 2020 2020 2020  ept.            
+00001230: 2020 2020 2020 2020 7061 7373 0a0a 0a64          pass...d
+00001240: 6566 205f 706c 6179 280a 2020 2020 7374  ef _play(.    st
+00001250: 6473 6372 2c0a 2020 2020 706c 6179 6c69  dscr,.    playli
+00001260: 7374 2c0a 2020 2020 766f 6c75 6d65 2c0a  st,.    volume,.
+00001270: 2020 2020 6c6f 6f70 2c0a 2020 2020 636c      loop,.    cl
+00001280: 6970 5f6d 6f64 652c 0a20 2020 2072 6573  ip_mode,.    res
+00001290: 6875 6666 6c65 2c0a 2020 2020 7570 6461  huffle,.    upda
+000012a0: 7465 5f64 6973 636f 7264 2c0a 2020 2020  te_discord,.    
+000012b0: 7669 7375 616c 697a 652c 0a29 3a0a 2020  visualize,.):.  
+000012c0: 2020 676c 6f62 616c 2063 616e 5f6d 6163    global can_mac
+000012d0: 5f6e 6f77 5f70 6c61 7969 6e67 2020 2320  _now_playing  # 
+000012e0: 7079 6c69 6e74 3a20 6469 7361 626c 653d  pylint: disable=
+000012f0: 676c 6f62 616c 2d73 7461 7465 6d65 6e74  global-statement
+00001300: 0a0a 2020 2020 696e 6974 5f63 7572 7365  ..    init_curse
+00001310: 7328 7374 6473 6372 290a 0a20 2020 2069  s(stdscr)..    i
+00001320: 6620 6c6f 6f70 3a0a 2020 2020 2020 2020  f loop:.        
+00001330: 6e65 7874 5f70 6c61 796c 6973 7420 3d20  next_playlist = 
+00001340: 706c 6179 6c69 7374 5b3a 5d0a 2020 2020  playlist[:].    
+00001350: 2020 2020 6966 2072 6573 6875 6666 6c65      if reshuffle
+00001360: 3a0a 2020 2020 2020 2020 2020 2020 7368  :.            sh
+00001370: 7566 666c 6528 6e65 7874 5f70 6c61 796c  uffle(next_playl
+00001380: 6973 7429 0a20 2020 2065 6c73 653a 0a20  ist).    else:. 
+00001390: 2020 2020 2020 206e 6578 745f 706c 6179         next_play
+000013a0: 6c69 7374 203d 204e 6f6e 650a 0a20 2020  list = None..   
+000013b0: 2070 6c61 7965 725f 6f75 7470 7574 203d   player_output =
+000013c0: 2050 6c61 7965 724f 7574 7075 7428 0a20   PlayerOutput(. 
+000013d0: 2020 2020 2020 2073 7464 7363 722c 2070         stdscr, p
+000013e0: 6c61 796c 6973 742c 2076 6f6c 756d 652c  laylist, volume,
+000013f0: 2063 6c69 705f 6d6f 6465 2c20 7570 6461   clip_mode, upda
+00001400: 7465 5f64 6973 636f 7264 2c20 7669 7375  te_discord, visu
+00001410: 616c 697a 650a 2020 2020 290a 0a20 2020  alize.    )..   
+00001420: 2069 6620 706c 6179 6572 5f6f 7574 7075   if player_outpu
+00001430: 742e 7570 6461 7465 5f64 6973 636f 7264  t.update_discord
+00001440: 3a0a 2020 2020 2020 2020 6469 7363 6f72  :.        discor
+00001450: 645f 7469 746c 655f 7175 6575 6520 3d20  d_title_queue = 
+00001460: 6d75 6c74 6970 726f 6365 7373 696e 672e  multiprocessing.
+00001470: 5369 6d70 6c65 5175 6575 6528 290a 2020  SimpleQueue().  
+00001480: 2020 2020 2020 6469 7363 6f72 645f 6172        discord_ar
+00001490: 7469 7374 5f71 7565 7565 203d 206d 756c  tist_queue = mul
+000014a0: 7469 7072 6f63 6573 7369 6e67 2e53 696d  tiprocessing.Sim
+000014b0: 706c 6551 7565 7565 2829 0a20 2020 2020  pleQueue().     
+000014c0: 2020 2064 6973 636f 7264 5f70 7265 7365     discord_prese
+000014d0: 6e63 655f 7072 6f63 6573 7320 3d20 6d75  nce_process = mu
+000014e0: 6c74 6970 726f 6365 7373 696e 672e 5072  ltiprocessing.Pr
+000014f0: 6f63 6573 7328 0a20 2020 2020 2020 2020  ocess(.         
+00001500: 2020 2064 6165 6d6f 6e3d 5472 7565 2c0a     daemon=True,.
+00001510: 2020 2020 2020 2020 2020 2020 7461 7267              targ
+00001520: 6574 3d64 6973 636f 7264 5f70 7265 7365  et=discord_prese
+00001530: 6e63 655f 6c6f 6f70 2c0a 2020 2020 2020  nce_loop,.      
+00001540: 2020 2020 2020 6172 6773 3d28 0a20 2020        args=(.   
+00001550: 2020 2020 2020 2020 2020 2020 2064 6973               dis
+00001560: 636f 7264 5f74 6974 6c65 5f71 7565 7565  cord_title_queue
+00001570: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001580: 2020 6469 7363 6f72 645f 6172 7469 7374    discord_artist
+00001590: 5f71 7565 7565 2c0a 2020 2020 2020 2020  _queue,.        
+000015a0: 2020 2020 2020 2020 706c 6179 6572 5f6f          player_o
+000015b0: 7574 7075 742e 6469 7363 6f72 645f 636f  utput.discord_co
+000015c0: 6e6e 6563 7465 642c 0a20 2020 2020 2020  nnected,.       
+000015d0: 2020 2020 2029 2c0a 2020 2020 2020 2020       ),.        
+000015e0: 290a 2020 2020 2020 2020 6469 7363 6f72  ).        discor
+000015f0: 645f 7072 6573 656e 6365 5f70 726f 6365  d_presence_proce
+00001600: 7373 2e73 7461 7274 2829 0a0a 2020 2020  ss.start()..    
+00001610: 6966 2073 7973 2e70 6c61 7466 6f72 6d20  if sys.platform 
+00001620: 3d3d 2022 6461 7277 696e 2220 616e 6420  == "darwin" and 
+00001630: 6361 6e5f 6d61 635f 6e6f 775f 706c 6179  can_mac_now_play
+00001640: 696e 673a 0a20 2020 2020 2020 206d 6163  ing:.        mac
+00001650: 5f6e 6f77 5f70 6c61 7969 6e67 2e74 6974  _now_playing.tit
+00001660: 6c65 5f71 7565 7565 203d 2051 7565 7565  le_queue = Queue
+00001670: 2829 0a20 2020 2020 2020 206d 6163 5f6e  ().        mac_n
+00001680: 6f77 5f70 6c61 7969 6e67 2e61 7274 6973  ow_playing.artis
+00001690: 745f 7175 6575 6520 3d20 5175 6575 6528  t_queue = Queue(
+000016a0: 290a 2020 2020 2020 2020 6d61 635f 6e6f  ).        mac_no
+000016b0: 775f 706c 6179 696e 672e 7120 3d20 5175  w_playing.q = Qu
+000016c0: 6575 6528 290a 2020 2020 2020 2020 6d61  eue().        ma
+000016d0: 635f 6e6f 775f 706c 6179 696e 672e 636f  c_now_playing.co
+000016e0: 7665 7220 3d20 636f 7665 725f 696d 670a  ver = cover_img.
+000016f0: 0a20 2020 2020 2020 206e 735f 6170 706c  .        ns_appl
+00001700: 6963 6174 696f 6e20 3d20 4e53 4170 706c  ication = NSAppl
+00001710: 6963 6174 696f 6e2e 7368 6172 6564 4170  ication.sharedAp
+00001720: 706c 6963 6174 696f 6e28 290a 2020 2020  plication().    
+00001730: 2020 2020 2320 6c6f 676f 5f6e 735f 696d      # logo_ns_im
+00001740: 6167 6520 3d20 4e53 496d 6167 652e 616c  age = NSImage.al
+00001750: 6c6f 6328 292e 696e 6974 4279 5265 6665  loc().initByRefe
+00001760: 7265 6e63 696e 6746 696c 655f 280a 2020  rencingFile_(.  
+00001770: 2020 2020 2020 2320 2020 2020 222e 2f6d        #     "./m
+00001780: 6165 7374 726f 5f69 636f 6e2e 706e 6722  aestro_icon.png"
+00001790: 0a20 2020 2020 2020 2023 2029 0a20 2020  .        # ).   
+000017a0: 2020 2020 2023 206e 735f 6170 706c 6963       # ns_applic
+000017b0: 6174 696f 6e2e 7365 7441 7070 6c69 6361  ation.setApplica
+000017c0: 7469 6f6e 4963 6f6e 496d 6167 655f 286c  tionIconImage_(l
+000017d0: 6f67 6f5f 6e73 5f69 6d61 6765 290a 2020  ogo_ns_image).  
+000017e0: 2020 2020 2020 6e73 5f61 7070 6c69 6361        ns_applica
+000017f0: 7469 6f6e 2e73 6574 4163 7469 7661 7469  tion.setActivati
+00001800: 6f6e 506f 6c69 6379 5f28 0a20 2020 2020  onPolicy_(.     
+00001810: 2020 2020 2020 204e 5341 7070 6c69 6361         NSApplica
+00001820: 7469 6f6e 4163 7469 7661 7469 6f6e 506f  tionActivationPo
+00001830: 6c69 6379 5072 6f68 6962 6974 6564 0a20  licyProhibited. 
+00001840: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+00001850: 2020 2320 4e4f 5445 3a20 6b65 6570 2072    # NOTE: keep r
+00001860: 6566 2074 6f20 6465 6c65 6761 7465 206f  ef to delegate o
+00001870: 626a 6563 742c 2073 6574 4465 6c65 6761  bject, setDelega
+00001880: 7465 5f20 646f 6573 6e27 7420 7265 7461  te_ doesn't reta
+00001890: 696e 0a20 2020 2020 2020 2064 656c 6567  in.        deleg
+000018a0: 6174 6520 3d20 4170 7044 656c 6567 6174  ate = AppDelegat
+000018b0: 652e 616c 6c6f 6328 292e 696e 6974 2829  e.alloc().init()
+000018c0: 0a20 2020 2020 2020 204e 5341 7070 2829  .        NSApp()
+000018d0: 2e73 6574 4465 6c65 6761 7465 5f28 6465  .setDelegate_(de
+000018e0: 6c65 6761 7465 290a 0a20 2020 2020 2020  legate)..       
+000018f0: 2061 7070 5f68 656c 7065 725f 7072 6f63   app_helper_proc
+00001900: 6573 7320 3d20 6d75 6c74 6970 726f 6365  ess = multiproce
+00001910: 7373 696e 672e 5072 6f63 6573 7328 0a20  ssing.Process(. 
+00001920: 2020 2020 2020 2020 2020 2064 6165 6d6f             daemo
+00001930: 6e3d 5472 7565 2c0a 2020 2020 2020 2020  n=True,.        
+00001940: 2020 2020 7461 7267 6574 3d61 7070 5f68      target=app_h
+00001950: 656c 7065 725f 6c6f 6f70 2c0a 2020 2020  elper_loop,.    
+00001960: 2020 2020 290a 2020 2020 2020 2020 6170      ).        ap
+00001970: 705f 6865 6c70 6572 5f70 726f 6365 7373  p_helper_process
+00001980: 2e73 7461 7274 2829 0a0a 2020 2020 7072  .start()..    pr
+00001990: 6576 5f76 6f6c 756d 6520 3d20 766f 6c75  ev_volume = volu
+000019a0: 6d65 0a20 2020 2077 6869 6c65 2070 6c61  me.    while pla
+000019b0: 7965 725f 6f75 7470 7574 2e69 2069 6e20  yer_output.i in 
+000019c0: 7261 6e67 6528 6c65 6e28 706c 6179 6572  range(len(player
+000019d0: 5f6f 7574 7075 742e 706c 6179 6c69 7374  _output.playlist
+000019e0: 2929 3a0a 2020 2020 2020 2020 736f 6e67  )):.        song
+000019f0: 5f70 6174 6820 3d20 6f73 2e70 6174 682e  _path = os.path.
+00001a00: 6a6f 696e 280a 2020 2020 2020 2020 2020  join(.          
+00001a10: 2020 534f 4e47 535f 4449 522c 2070 6c61    SONGS_DIR, pla
+00001a20: 7965 725f 6f75 7470 7574 2e70 6c61 796c  yer_output.playl
+00001a30: 6973 745b 706c 6179 6572 5f6f 7574 7075  ist[player_outpu
+00001a40: 742e 695d 5b31 5d0a 2020 2020 2020 2020  t.i][1].        
+00001a50: 290a 0a20 2020 2020 2020 2070 6c61 7962  )..        playb
+00001a60: 6163 6b20 3d20 506c 6179 6261 636b 2829  ack = Playback()
+00001a70: 0a20 2020 2020 2020 2070 6c61 7962 6163  .        playbac
+00001a80: 6b2e 6c6f 6164 5f66 696c 6528 736f 6e67  k.load_file(song
+00001a90: 5f70 6174 6829 0a0a 2020 2020 2020 2020  _path)..        
+00001aa0: 636c 6970 5f73 7472 696e 6720 3d20 706c  clip_string = pl
+00001ab0: 6179 6572 5f6f 7574 7075 742e 706c 6179  ayer_output.play
+00001ac0: 6c69 7374 5b70 6c61 7965 725f 6f75 7470  list[player_outp
+00001ad0: 7574 2e69 5d5b 335d 0a20 2020 2020 2020  ut.i][3].       
+00001ae0: 2069 6620 636c 6970 5f73 7472 696e 673a   if clip_string:
+00001af0: 0a20 2020 2020 2020 2020 2020 2070 6c61  .            pla
+00001b00: 7965 725f 6f75 7470 7574 2e63 6c69 7020  yer_output.clip 
+00001b10: 3d20 7475 706c 6528 0a20 2020 2020 2020  = tuple(.       
+00001b20: 2020 2020 2020 2020 206d 6170 2866 6c6f           map(flo
+00001b30: 6174 2c20 706c 6179 6572 5f6f 7574 7075  at, player_outpu
+00001b40: 742e 706c 6179 6c69 7374 5b70 6c61 7965  t.playlist[playe
+00001b50: 725f 6f75 7470 7574 2e69 5d5b 335d 2e73  r_output.i][3].s
+00001b60: 706c 6974 2829 290a 2020 2020 2020 2020  plit()).        
+00001b70: 2020 2020 290a 2020 2020 2020 2020 656c      ).        el
+00001b80: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00001b90: 706c 6179 6572 5f6f 7574 7075 742e 636c  player_output.cl
+00001ba0: 6970 203d 2030 2c20 706c 6179 6261 636b  ip = 0, playback
+00001bb0: 2e64 7572 6174 696f 6e0a 0a20 2020 2020  .duration..     
+00001bc0: 2020 2070 6c61 7965 725f 6f75 7470 7574     player_output
+00001bd0: 2e70 6175 7365 6420 3d20 4661 6c73 650a  .paused = False.
+00001be0: 2020 2020 2020 2020 706c 6179 6572 5f6f          player_o
+00001bf0: 7574 7075 742e 6475 7261 7469 6f6e 203d  utput.duration =
+00001c00: 2066 756c 6c5f 6475 7261 7469 6f6e 203d   full_duration =
+00001c10: 2070 6c61 7962 6163 6b2e 6475 7261 7469   playback.durati
+00001c20: 6f6e 0a0a 2020 2020 2020 2020 6966 2073  on..        if s
+00001c30: 7973 2e70 6c61 7466 6f72 6d20 3d3d 2022  ys.platform == "
+00001c40: 6461 7277 696e 2220 616e 6420 6361 6e5f  darwin" and can_
+00001c50: 6d61 635f 6e6f 775f 706c 6179 696e 673a  mac_now_playing:
+00001c60: 0a20 2020 2020 2020 2020 2020 206d 6163  .            mac
+00001c70: 5f6e 6f77 5f70 6c61 7969 6e67 2e70 6175  _now_playing.pau
+00001c80: 7365 6420 3d20 4661 6c73 650a 2020 2020  sed = False.    
+00001c90: 2020 2020 2020 2020 6d61 635f 6e6f 775f          mac_now_
+00001ca0: 706c 6179 696e 672e 706f 7320 3d20 300a  playing.pos = 0.
+00001cb0: 2020 2020 2020 2020 2020 2020 6d61 635f              mac_
+00001cc0: 6e6f 775f 706c 6179 696e 672e 6c65 6e67  now_playing.leng
+00001cd0: 7468 203d 2070 6c61 7965 725f 6f75 7470  th = player_outp
+00001ce0: 7574 2e64 7572 6174 696f 6e0a 0a20 2020  ut.duration..   
+00001cf0: 2020 2020 2020 2020 206d 756c 7469 7072           multipr
+00001d00: 6f63 6573 7369 6e67 5f70 7574 5f77 6f72  ocessing_put_wor
+00001d10: 6428 0a20 2020 2020 2020 2020 2020 2020  d(.             
+00001d20: 2020 206d 6163 5f6e 6f77 5f70 6c61 7969     mac_now_playi
+00001d30: 6e67 2e74 6974 6c65 5f71 7565 7565 2c0a  ng.title_queue,.
+00001d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d50: 706c 6179 6572 5f6f 7574 7075 742e 706c  player_output.pl
+00001d60: 6179 6c69 7374 5b70 6c61 7965 725f 6f75  aylist[player_ou
+00001d70: 7470 7574 2e69 5d5b 315d 2c0a 2020 2020  tput.i][1],.    
+00001d80: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00001d90: 2020 2020 2020 6d75 6c74 6970 726f 6365        multiproce
+00001da0: 7373 696e 675f 7075 745f 776f 7264 280a  ssing_put_word(.
+00001db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001dc0: 6d61 635f 6e6f 775f 706c 6179 696e 672e  mac_now_playing.
+00001dd0: 6172 7469 7374 5f71 7565 7565 2c0a 2020  artist_queue,.  
+00001de0: 2020 2020 2020 2020 2020 2020 2020 706c                pl
+00001df0: 6179 6572 5f6f 7574 7075 742e 706c 6179  ayer_output.play
+00001e00: 6c69 7374 5b70 6c61 7965 725f 6f75 7470  list[player_outp
+00001e10: 7574 2e69 5d5b 2d33 5d2c 0a20 2020 2020  ut.i][-3],.     
+00001e20: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+00001e30: 2020 2020 2020 7570 6461 7465 5f6e 6f77        update_now
+00001e40: 5f70 6c61 7969 6e67 203d 2054 7275 650a  _playing = True.
+00001e50: 0a20 2020 2020 2020 2069 6620 706c 6179  .        if play
+00001e60: 6572 5f6f 7574 7075 742e 7570 6461 7465  er_output.update
+00001e70: 5f64 6973 636f 7264 3a0a 2020 2020 2020  _discord:.      
+00001e80: 2020 2020 2020 6d75 6c74 6970 726f 6365        multiproce
+00001e90: 7373 696e 675f 7075 745f 776f 7264 280a  ssing_put_word(.
+00001ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001eb0: 6469 7363 6f72 645f 7469 746c 655f 7175  discord_title_qu
+00001ec0: 6575 652c 2070 6c61 7965 725f 6f75 7470  eue, player_outp
+00001ed0: 7574 2e70 6c61 796c 6973 745b 706c 6179  ut.playlist[play
+00001ee0: 6572 5f6f 7574 7075 742e 695d 5b31 5d0a  er_output.i][1].
+00001ef0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00001f00: 2020 2020 2020 2020 2020 6d75 6c74 6970            multip
+00001f10: 726f 6365 7373 696e 675f 7075 745f 776f  rocessing_put_wo
+00001f20: 7264 280a 2020 2020 2020 2020 2020 2020  rd(.            
+00001f30: 2020 2020 6469 7363 6f72 645f 6172 7469      discord_arti
+00001f40: 7374 5f71 7565 7565 2c0a 2020 2020 2020  st_queue,.      
+00001f50: 2020 2020 2020 2020 2020 706c 6179 6572            player
+00001f60: 5f6f 7574 7075 742e 706c 6179 6c69 7374  _output.playlist
+00001f70: 5b70 6c61 7965 725f 6f75 7470 7574 2e69  [player_output.i
+00001f80: 5d5b 2d33 5d2c 0a20 2020 2020 2020 2020  ][-3],.         
+00001f90: 2020 2029 0a0a 2020 2020 2020 2020 706c     )..        pl
+00001fa0: 6179 6261 636b 2e70 6c61 7928 290a 0a20  ayback.play().. 
+00001fb0: 2020 2020 2020 2069 6620 706c 6179 6572         if player
+00001fc0: 5f6f 7574 7075 742e 636c 6970 5f6d 6f64  _output.clip_mod
+00001fd0: 653a 0a20 2020 2020 2020 2020 2020 2063  e:.            c
+00001fe0: 6c69 705f 7374 6172 742c 2063 6c69 705f  lip_start, clip_
+00001ff0: 656e 6420 3d20 706c 6179 6572 5f6f 7574  end = player_out
+00002000: 7075 742e 636c 6970 0a20 2020 2020 2020  put.clip.       
+00002010: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
+00002020: 7574 2e64 7572 6174 696f 6e20 3d20 636c  ut.duration = cl
+00002030: 6970 5f65 6e64 202d 2063 6c69 705f 7374  ip_end - clip_st
+00002040: 6172 740a 2020 2020 2020 2020 2020 2020  art.            
+00002050: 706c 6179 6261 636b 2e73 6565 6b28 636c  playback.seek(cl
+00002060: 6970 5f73 7461 7274 290a 2020 2020 2020  ip_start).      
+00002070: 2020 2020 2020 6966 2073 7973 2e70 6c61        if sys.pla
+00002080: 7466 6f72 6d20 3d3d 2022 6461 7277 696e  tform == "darwin
+00002090: 2220 616e 6420 6361 6e5f 6d61 635f 6e6f  " and can_mac_no
+000020a0: 775f 706c 6179 696e 673a 0a20 2020 2020  w_playing:.     
+000020b0: 2020 2020 2020 2020 2020 206d 6163 5f6e             mac_n
+000020c0: 6f77 5f70 6c61 7969 6e67 2e70 6f73 203d  ow_playing.pos =
+000020d0: 2072 6f75 6e64 2870 6c61 7962 6163 6b2e   round(playback.
+000020e0: 6375 7272 5f70 6f73 290a 2020 2020 2020  curr_pos).      
+000020f0: 2020 2020 2020 6c61 7374 5f74 696d 6573        last_times
+00002100: 7461 6d70 203d 2070 6c61 7962 6163 6b2e  tamp = playback.
+00002110: 6375 7272 5f70 6f73 0a0a 2020 2020 2020  curr_pos..      
+00002120: 2020 7374 6172 745f 7469 6d65 203d 2070    start_time = p
+00002130: 6175 7365 5f73 7461 7274 203d 2074 696d  ause_start = tim
+00002140: 6528 290a 2020 2020 2020 2020 706c 6179  e().        play
+00002150: 6261 636b 2e73 6574 5f76 6f6c 756d 6528  back.set_volume(
+00002160: 706c 6179 6572 5f6f 7574 7075 742e 766f  player_output.vo
+00002170: 6c75 6d65 290a 0a20 2020 2020 2020 206c  lume)..        l
+00002180: 6173 745f 7469 6d65 7374 616d 7020 3d20  ast_timestamp = 
+00002190: 706c 6179 6261 636b 2e63 7572 725f 706f  playback.curr_po
+000021a0: 730a 2020 2020 2020 2020 6e65 7874 5f73  s.        next_s
+000021b0: 6f6e 6720 3d20 3120 2023 202d 3120 6966  ong = 1  # -1 if
+000021c0: 2067 6f69 6e67 2062 6163 6b2c 2030 2069   going back, 0 i
+000021d0: 6620 7265 7374 6172 7469 6e67 2c20 2b31  f restarting, +1
+000021e0: 2069 6620 6e65 7874 2073 6f6e 670a 2020   if next song.  
+000021f0: 2020 2020 2020 706c 6179 6572 5f6f 7574        player_out
+00002200: 7075 742e 656e 6469 6e67 203d 2046 616c  put.ending = Fal
+00002210: 7365 0a20 2020 2020 2020 2077 6869 6c65  se.        while
+00002220: 2054 7275 653a 0a20 2020 2020 2020 2020   True:.         
+00002230: 2020 2069 6620 6e6f 7420 706c 6179 6261     if not playba
+00002240: 636b 2e61 6374 6976 6520 6f72 2028 0a20  ck.active or (. 
+00002250: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00002260: 6c61 7965 725f 6f75 7470 7574 2e63 6c69  layer_output.cli
+00002270: 705f 6d6f 6465 0a20 2020 2020 2020 2020  p_mode.         
+00002280: 2020 2020 2020 2061 6e64 2070 6c61 7962         and playb
+00002290: 6163 6b2e 6375 7272 5f70 6f73 203e 2070  ack.curr_pos > p
+000022a0: 6c61 7965 725f 6f75 7470 7574 2e63 6c69  layer_output.cli
+000022b0: 705b 315d 0a20 2020 2020 2020 2020 2020  p[1].           
+000022c0: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
+000022d0: 2020 2020 6e65 7874 5f73 6f6e 6720 3d20      next_song = 
+000022e0: 6e6f 7420 706c 6179 6572 5f6f 7574 7075  not player_outpu
+000022f0: 742e 6c6f 6f70 696e 675f 6375 7272 656e  t.looping_curren
+00002300: 745f 736f 6e67 0a20 2020 2020 2020 2020  t_song.         
+00002310: 2020 2020 2020 2062 7265 616b 0a0a 2020         break..  
+00002320: 2020 2020 2020 2020 2020 2320 6661 6465            # fade
+00002330: 2069 6e20 6669 7273 7420 3220 7365 636f   in first 2 seco
+00002340: 6e64 7320 6f66 2063 6c69 700a 2020 2020  nds of clip.    
+00002350: 2020 2020 2020 2020 6966 2028 0a20 2020          if (.   
+00002360: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
+00002370: 7965 725f 6f75 7470 7574 2e63 6c69 705f  yer_output.clip_
+00002380: 6d6f 6465 0a20 2020 2020 2020 2020 2020  mode.           
+00002390: 2020 2020 2061 6e64 2063 6c69 705f 7374       and clip_st
+000023a0: 6172 7420 213d 2030 2020 2320 6966 2063  art != 0  # if c
+000023b0: 6c69 7020 646f 6573 6e27 7420 7374 6172  lip doesn't star
+000023c0: 7420 6174 2062 6567 696e 6e69 6e67 0a20  t at beginning. 
+000023d0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+000023e0: 6e64 2063 6c69 705f 656e 6420 2d20 636c  nd clip_end - cl
+000023f0: 6970 5f73 7461 7274 203e 2035 2020 2320  ip_start > 5  # 
+00002400: 6966 2063 6c69 7020 6973 206c 6f6e 6765  if clip is longe
+00002410: 7220 7468 616e 2035 2073 6563 730a 2020  r than 5 secs.  
+00002420: 2020 2020 2020 2020 2020 2020 2020 616e                an
+00002430: 6420 706c 6179 6261 636b 2e63 7572 725f  d playback.curr_
+00002440: 706f 7320 3c20 636c 6970 5f73 7461 7274  pos < clip_start
+00002450: 202b 2032 0a20 2020 2020 2020 2020 2020   + 2.           
+00002460: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
+00002470: 2020 2020 706c 6179 6261 636b 2e73 6574      playback.set
+00002480: 5f76 6f6c 756d 6528 0a20 2020 2020 2020  _volume(.       
+00002490: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
+000024a0: 7965 725f 6f75 7470 7574 2e76 6f6c 756d  yer_output.volum
+000024b0: 6520 2a20 2870 6c61 7962 6163 6b2e 6375  e * (playback.cu
+000024c0: 7272 5f70 6f73 202d 2063 6c69 705f 7374  rr_pos - clip_st
+000024d0: 6172 7429 202f 2032 0a20 2020 2020 2020  art) / 2.       
+000024e0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+000024f0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00002500: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
+00002510: 7962 6163 6b2e 7365 745f 766f 6c75 6d65  yback.set_volume
+00002520: 2870 6c61 7965 725f 6f75 7470 7574 2e76  (player_output.v
+00002530: 6f6c 756d 6529 0a0a 2020 2020 2020 2020  olume)..        
+00002540: 2020 2020 6966 2073 7973 2e70 6c61 7466      if sys.platf
+00002550: 6f72 6d20 3d3d 2022 6461 7277 696e 2220  orm == "darwin" 
+00002560: 616e 6420 6361 6e5f 6d61 635f 6e6f 775f  and can_mac_now_
+00002570: 706c 6179 696e 673a 0a20 2020 2020 2020  playing:.       
+00002580: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
+00002590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025a0: 2020 6966 2075 7064 6174 655f 6e6f 775f    if update_now_
+000025b0: 706c 6179 696e 673a 0a20 2020 2020 2020  playing:.       
+000025c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025d0: 206d 6163 5f6e 6f77 5f70 6c61 7969 6e67   mac_now_playing
+000025e0: 2e75 7064 6174 6528 290a 2020 2020 2020  .update().      
+000025f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002600: 2020 7570 6461 7465 5f6e 6f77 5f70 6c61    update_now_pla
+00002610: 7969 6e67 203d 2046 616c 7365 0a20 2020  ying = False.   
+00002620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002630: 204e 5352 756e 4c6f 6f70 2e63 7572 7265   NSRunLoop.curre
+00002640: 6e74 5275 6e4c 6f6f 7028 292e 7275 6e55  ntRunLoop().runU
+00002650: 6e74 696c 4461 7465 5f28 0a20 2020 2020  ntilDate_(.     
+00002660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002670: 2020 204e 5344 6174 652e 6461 7465 5769     NSDate.dateWi
+00002680: 7468 5469 6d65 496e 7465 7276 616c 5369  thTimeIntervalSi
+00002690: 6e63 654e 6f77 5f28 302e 3035 290a 2020  nceNow_(0.05).  
+000026a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000026b0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+000026c0: 2020 2020 6578 6365 7074 3a20 2023 2070      except:  # p
+000026d0: 796c 696e 743a 2064 6973 6162 6c65 3d62  ylint: disable=b
+000026e0: 6172 652d 6578 6365 7074 0a20 2020 2020  are-except.     
+000026f0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00002700: 616e 5f6d 6163 5f6e 6f77 5f70 6c61 7969  an_mac_now_playi
+00002710: 6e67 203d 2046 616c 7365 0a0a 2020 2020  ng = False..    
+00002720: 2020 2020 2020 2020 6966 2028 0a20 2020          if (.   
+00002730: 2020 2020 2020 2020 2020 2020 2073 7973               sys
+00002740: 2e70 6c61 7466 6f72 6d20 3d3d 2022 6461  .platform == "da
+00002750: 7277 696e 220a 2020 2020 2020 2020 2020  rwin".          
+00002760: 2020 2020 2020 616e 6420 6361 6e5f 6d61        and can_ma
+00002770: 635f 6e6f 775f 706c 6179 696e 670a 2020  c_now_playing.  
+00002780: 2020 2020 2020 2020 2020 2020 2020 616e                an
+00002790: 6420 6e6f 7420 6d61 635f 6e6f 775f 706c  d not mac_now_pl
+000027a0: 6179 696e 672e 712e 656d 7074 7928 290a  aying.q.empty().
+000027b0: 2020 2020 2020 2020 2020 2020 293a 0a20              ):. 
+000027c0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000027d0: 203d 206d 6163 5f6e 6f77 5f70 6c61 7969   = mac_now_playi
+000027e0: 6e67 2e71 2e67 6574 2829 0a20 2020 2020  ng.q.get().     
+000027f0: 2020 2020 2020 2020 2020 2069 6620 6320             if c 
+00002800: 696e 2022 6e4e 223a 0a20 2020 2020 2020  in "nN":.       
+00002810: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00002820: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00002830: 2020 2020 2020 2020 2020 706c 6179 6572            player
+00002840: 5f6f 7574 7075 742e 6920 3d3d 206c 656e  _output.i == len
+00002850: 2870 6c61 7965 725f 6f75 7470 7574 2e70  (player_output.p
+00002860: 6c61 796c 6973 7429 202d 2031 0a20 2020  laylist) - 1.   
+00002870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002880: 2020 2020 2061 6e64 206e 6f74 206c 6f6f       and not loo
+00002890: 700a 2020 2020 2020 2020 2020 2020 2020  p.              
+000028a0: 2020 2020 2020 293a 0a20 2020 2020 2020        ):.       
+000028b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028c0: 2070 6173 730a 2020 2020 2020 2020 2020   pass.          
+000028d0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+000028e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028f0: 2020 2020 2020 2020 6e65 7874 5f73 6f6e          next_son
+00002900: 6720 3d20 310a 2020 2020 2020 2020 2020  g = 1.          
+00002910: 2020 2020 2020 2020 2020 2020 2020 706c                pl
+00002920: 6179 6261 636b 2e73 746f 7028 290a 2020  ayback.stop().  
+00002930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002940: 2020 2020 2020 6272 6561 6b0a 2020 2020        break.    
+00002950: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00002960: 2063 2069 6e20 2262 4222 3a0a 2020 2020   c in "bB":.    
+00002970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002980: 6966 2070 6c61 7965 725f 6f75 7470 7574  if player_output
+00002990: 2e69 203d 3d20 303a 0a20 2020 2020 2020  .i == 0:.       
+000029a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029b0: 2070 6173 730a 2020 2020 2020 2020 2020   pass.          
+000029c0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+000029d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029e0: 2020 2020 2020 2020 6e65 7874 5f73 6f6e          next_son
+000029f0: 6720 3d20 2d31 0a20 2020 2020 2020 2020  g = -1.         
+00002a00: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00002a10: 6c61 7962 6163 6b2e 7374 6f70 2829 0a20  layback.stop(). 
+00002a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a30: 2020 2020 2020 2062 7265 616b 0a20 2020         break.   
+00002a40: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
+00002a50: 6620 6320 696e 2022 7252 223a 0a20 2020  f c in "rR":.   
+00002a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a70: 2070 6c61 7962 6163 6b2e 7374 6f70 2829   playback.stop()
+00002a80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002a90: 2020 2020 206e 6578 745f 736f 6e67 203d       next_song =
+00002aa0: 2030 0a20 2020 2020 2020 2020 2020 2020   0.             
+00002ab0: 2020 2020 2020 2062 7265 616b 0a20 2020         break.   
+00002ac0: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
+00002ad0: 6620 6320 696e 2022 7151 223a 0a20 2020  f c in "qQ":.   
+00002ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002af0: 2070 6c61 7965 725f 6f75 7470 7574 2e65   player_output.e
+00002b00: 6e64 696e 6720 3d20 5472 7565 0a20 2020  nding = True.   
+00002b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b20: 2062 7265 616b 0a20 2020 2020 2020 2020   break.         
+00002b30: 2020 2020 2020 2065 6c69 6620 6320 3d3d         elif c ==
+00002b40: 2022 2022 3a0a 2020 2020 2020 2020 2020   " ":.          
+00002b50: 2020 2020 2020 2020 2020 706c 6179 6572            player
+00002b60: 5f6f 7574 7075 742e 7061 7573 6564 203d  _output.paused =
+00002b70: 206e 6f74 2070 6c61 7965 725f 6f75 7470   not player_outp
+00002b80: 7574 2e70 6175 7365 640a 0a20 2020 2020  ut.paused..     
+00002b90: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00002ba0: 6620 706c 6179 6572 5f6f 7574 7075 742e  f player_output.
+00002bb0: 7061 7573 6564 3a0a 2020 2020 2020 2020  paused:.        
+00002bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002bd0: 706c 6179 6261 636b 2e70 6175 7365 2829  playback.pause()
+00002be0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002bf0: 2020 2020 2020 2020 2070 6175 7365 5f73           pause_s
+00002c00: 7461 7274 203d 2074 696d 6528 290a 2020  tart = time().  
+00002c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c20: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00002c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c40: 706c 6179 6261 636b 2e72 6573 756d 6528  playback.resume(
+00002c50: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00002c60: 2020 2020 2020 2020 2020 7374 6172 745f            start_
+00002c70: 7469 6d65 202b 3d20 7469 6d65 2829 202d  time += time() -
+00002c80: 2070 6175 7365 5f73 7461 7274 0a0a 2020   pause_start..  
+00002c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ca0: 2020 6966 2073 7973 2e70 6c61 7466 6f72    if sys.platfor
+00002cb0: 6d20 3d3d 2022 6461 7277 696e 2220 616e  m == "darwin" an
+00002cc0: 6420 6361 6e5f 6d61 635f 6e6f 775f 706c  d can_mac_now_pl
+00002cd0: 6179 696e 673a 0a20 2020 2020 2020 2020  aying:.         
+00002ce0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00002cf0: 6163 5f6e 6f77 5f70 6c61 7969 6e67 2e70  ac_now_playing.p
+00002d00: 6175 7365 6420 3d20 706c 6179 6572 5f6f  aused = player_o
+00002d10: 7574 7075 742e 7061 7573 6564 0a20 2020  utput.paused.   
+00002d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d30: 2020 2020 2069 6620 706c 6179 6572 5f6f       if player_o
+00002d40: 7574 7075 742e 7061 7573 6564 3a0a 2020  utput.paused:.  
+00002d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d60: 2020 2020 2020 2020 2020 6d61 635f 6e6f            mac_no
+00002d70: 775f 706c 6179 696e 672e 7061 7573 6528  w_playing.pause(
+00002d80: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00002d90: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
 00002da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002db0: 6d61 635f 6e6f 775f 706c 6179 696e 672e  mac_now_playing.
-00002dc0: 7265 7375 6d65 2829 0a20 2020 2020 2020  resume().       
-00002dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002de0: 2075 7064 6174 655f 6e6f 775f 706c 6179   update_now_play
-00002df0: 696e 6720 3d20 5472 7565 0a0a 2020 2020  ing = True..    
-00002e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e10: 706c 6179 6572 5f6f 7574 7075 742e 6f75  player_output.ou
-00002e20: 7470 7574 2870 6c61 7962 6163 6b2e 6375  tput(playback.cu
-00002e30: 7272 5f70 6f73 290a 2020 2020 2020 2020  rr_pos).        
-00002e40: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00002e50: 2020 2020 2020 2020 2020 6320 3d20 7374            c = st
-00002e60: 6473 6372 2e67 6574 6368 2829 0a20 2020  dscr.getch().   
-00002e70: 2020 2020 2020 2020 2020 2020 206e 6578               nex
-00002e80: 745f 6320 3d20 7374 6473 6372 2e67 6574  t_c = stdscr.get
-00002e90: 6368 2829 0a20 2020 2020 2020 2020 2020  ch().           
-00002ea0: 2020 2020 2077 6869 6c65 206e 6578 745f       while next_
-00002eb0: 6320 213d 202d 313a 0a20 2020 2020 2020  c != -1:.       
-00002ec0: 2020 2020 2020 2020 2020 2020 2063 2c20               c, 
-00002ed0: 6e65 7874 5f63 203d 206e 6578 745f 632c  next_c = next_c,
-00002ee0: 2073 7464 7363 722e 6765 7463 6828 290a   stdscr.getch().
-00002ef0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002f00: 2069 6620 6320 213d 202d 313a 0a20 2020   if c != -1:.   
-00002f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f20: 2069 6620 706c 6179 6572 5f6f 7574 7075   if player_outpu
-00002f30: 742e 7072 6f6d 7074 696e 6720 6973 204e  t.prompting is N
-00002f40: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00002f50: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00002f60: 6320 3d3d 2063 7572 7365 732e 4b45 595f  c == curses.KEY_
-00002f70: 4c45 4654 3a0a 2020 2020 2020 2020 2020  LEFT:.          
-00002f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f90: 2020 706c 6179 6261 636b 2e73 6565 6b28    playback.seek(
-00002fa0: 706c 6179 6261 636b 2e63 7572 725f 706f  playback.curr_po
-00002fb0: 7320 2d20 5343 5255 425f 5449 4d45 290a  s - SCRUB_TIME).
-00002fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002fd0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00002fe0: 7973 2e70 6c61 7466 6f72 6d20 3d3d 2022  ys.platform == "
-00002ff0: 6461 7277 696e 2220 616e 6420 6361 6e5f  darwin" and can_
-00003000: 6d61 635f 6e6f 775f 706c 6179 696e 673a  mac_now_playing:
-00003010: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002db0: 2020 2020 2020 2020 2020 2020 6d61 635f              mac_
+00002dc0: 6e6f 775f 706c 6179 696e 672e 7265 7375  now_playing.resu
+00002dd0: 6d65 2829 0a20 2020 2020 2020 2020 2020  me().           
+00002de0: 2020 2020 2020 2020 2020 2020 2075 7064               upd
+00002df0: 6174 655f 6e6f 775f 706c 6179 696e 6720  ate_now_playing 
+00002e00: 3d20 5472 7565 0a0a 2020 2020 2020 2020  = True..        
+00002e10: 2020 2020 2020 2020 2020 2020 706c 6179              play
+00002e20: 6572 5f6f 7574 7075 742e 6f75 7470 7574  er_output.output
+00002e30: 2870 6c61 7962 6163 6b2e 6375 7272 5f70  (playback.curr_p
+00002e40: 6f73 290a 2020 2020 2020 2020 2020 2020  os).            
+00002e50: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00002e60: 2020 2020 2020 6320 3d20 7374 6473 6372        c = stdscr
+00002e70: 2e67 6574 6368 2829 0a20 2020 2020 2020  .getch().       
+00002e80: 2020 2020 2020 2020 206e 6578 745f 6320           next_c 
+00002e90: 3d20 7374 6473 6372 2e67 6574 6368 2829  = stdscr.getch()
+00002ea0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002eb0: 2077 6869 6c65 206e 6578 745f 6320 213d   while next_c !=
+00002ec0: 202d 313a 0a20 2020 2020 2020 2020 2020   -1:.           
+00002ed0: 2020 2020 2020 2020 2063 2c20 6e65 7874           c, next
+00002ee0: 5f63 203d 206e 6578 745f 632c 2073 7464  _c = next_c, std
+00002ef0: 7363 722e 6765 7463 6828 290a 0a20 2020  scr.getch()..   
+00002f00: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00002f10: 6320 213d 202d 313a 0a20 2020 2020 2020  c != -1:.       
+00002f20: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00002f30: 706c 6179 6572 5f6f 7574 7075 742e 7072  player_output.pr
+00002f40: 6f6d 7074 696e 6720 6973 204e 6f6e 653a  ompting is None:
+00002f50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002f60: 2020 2020 2020 2020 2069 6620 6320 3d3d           if c ==
+00002f70: 2063 7572 7365 732e 4b45 595f 4c45 4654   curses.KEY_LEFT
+00002f80: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00002f90: 2020 2020 2020 2020 2020 2020 2020 706c                pl
+00002fa0: 6179 6261 636b 2e73 6565 6b28 706c 6179  ayback.seek(play
+00002fb0: 6261 636b 2e63 7572 725f 706f 7320 2d20  back.curr_pos - 
+00002fc0: 5343 5255 425f 5449 4d45 290a 2020 2020  SCRUB_TIME).    
+00002fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002fe0: 2020 2020 2020 2020 6966 2073 7973 2e70          if sys.p
+00002ff0: 6c61 7466 6f72 6d20 3d3d 2022 6461 7277  latform == "darw
+00003000: 696e 2220 616e 6420 6361 6e5f 6d61 635f  in" and can_mac_
+00003010: 6e6f 775f 706c 6179 696e 673a 0a20 2020  now_playing:.   
 00003020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003030: 206d 6163 5f6e 6f77 5f70 6c61 7969 6e67   mac_now_playing
-00003040: 2e70 6f73 203d 2072 6f75 6e64 2870 6c61  .pos = round(pla
-00003050: 7962 6163 6b2e 6375 7272 5f70 6f73 290a  yback.curr_pos).
-00003060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003030: 2020 2020 2020 2020 2020 2020 206d 6163               mac
+00003040: 5f6e 6f77 5f70 6c61 7969 6e67 2e70 6f73  _now_playing.pos
+00003050: 203d 2072 6f75 6e64 2870 6c61 7962 6163   = round(playbac
+00003060: 6b2e 6375 7272 5f70 6f73 290a 2020 2020  k.curr_pos).    
 00003070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003080: 7570 6461 7465 5f6e 6f77 5f70 6c61 7969  update_now_playi
-00003090: 6e67 203d 2054 7275 650a 0a20 2020 2020  ng = True..     
-000030a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030b0: 2020 2020 2020 206c 6173 745f 7469 6d65         last_time
-000030c0: 7374 616d 7020 3d20 706c 6179 6261 636b  stamp = playback
-000030d0: 2e63 7572 725f 706f 730a 2020 2020 2020  .curr_pos.      
-000030e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030f0: 2020 2020 2020 706c 6179 6572 5f6f 7574        player_out
-00003100: 7075 742e 6f75 7470 7574 2870 6c61 7962  put.output(playb
-00003110: 6163 6b2e 6375 7272 5f70 6f73 290a 2020  ack.curr_pos).  
-00003120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003130: 2020 2020 2020 656c 6966 2063 203d 3d20        elif c == 
-00003140: 6375 7273 6573 2e4b 4559 5f52 4947 4854  curses.KEY_RIGHT
-00003150: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00003160: 2020 2020 2020 2020 2020 2020 2020 706c                pl
-00003170: 6179 6261 636b 2e73 6565 6b28 706c 6179  ayback.seek(play
-00003180: 6261 636b 2e63 7572 725f 706f 7320 2b20  back.curr_pos + 
-00003190: 5343 5255 425f 5449 4d45 290a 2020 2020  SCRUB_TIME).    
-000031a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000031b0: 2020 2020 2020 2020 6966 2073 7973 2e70          if sys.p
-000031c0: 6c61 7466 6f72 6d20 3d3d 2022 6461 7277  latform == "darw
-000031d0: 696e 2220 616e 6420 6361 6e5f 6d61 635f  in" and can_mac_
-000031e0: 6e6f 775f 706c 6179 696e 673a 0a20 2020  now_playing:.   
-000031f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003200: 2020 2020 2020 2020 2020 2020 206d 6163               mac
-00003210: 5f6e 6f77 5f70 6c61 7969 6e67 2e70 6f73  _now_playing.pos
-00003220: 203d 2072 6f75 6e64 2870 6c61 7962 6163   = round(playbac
-00003230: 6b2e 6375 7272 5f70 6f73 290a 2020 2020  k.curr_pos).    
-00003240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003250: 2020 2020 2020 2020 2020 2020 7570 6461              upda
-00003260: 7465 5f6e 6f77 5f70 6c61 7969 6e67 203d  te_now_playing =
-00003270: 2054 7275 650a 0a20 2020 2020 2020 2020   True..         
-00003280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003290: 2020 206c 6173 745f 7469 6d65 7374 616d     last_timestam
-000032a0: 7020 3d20 706c 6179 6261 636b 2e63 7572  p = playback.cur
-000032b0: 725f 706f 730a 2020 2020 2020 2020 2020  r_pos.          
-000032c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000032d0: 2020 706c 6179 6572 5f6f 7574 7075 742e    player_output.
-000032e0: 6f75 7470 7574 2870 6c61 7962 6163 6b2e  output(playback.
-000032f0: 6375 7272 5f70 6f73 290a 2020 2020 2020  curr_pos).      
-00003300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003310: 2020 656c 6966 2063 203d 3d20 6375 7273    elif c == curs
-00003320: 6573 2e4b 4559 5f55 503a 0a20 2020 2020  es.KEY_UP:.     
-00003330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003340: 2020 2020 2020 2070 6c61 7965 725f 6f75         player_ou
-00003350: 7470 7574 2e73 6372 6f6c 6c65 722e 7363  tput.scroller.sc
-00003360: 726f 6c6c 5f62 6163 6b77 6172 6428 290a  roll_backward().
-00003370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003380: 2020 2020 2020 2020 2020 2020 706c 6179              play
-00003390: 6572 5f6f 7574 7075 742e 6f75 7470 7574  er_output.output
-000033a0: 2870 6c61 7962 6163 6b2e 6375 7272 5f70  (playback.curr_p
-000033b0: 6f73 290a 2020 2020 2020 2020 2020 2020  os).            
-000033c0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-000033d0: 2063 203d 3d20 6375 7273 6573 2e4b 4559   c == curses.KEY
-000033e0: 5f44 4f57 4e3a 0a20 2020 2020 2020 2020  _DOWN:.         
-000033f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003400: 2020 2070 6c61 7965 725f 6f75 7470 7574     player_output
-00003410: 2e73 6372 6f6c 6c65 722e 7363 726f 6c6c  .scroller.scroll
-00003420: 5f66 6f72 7761 7264 2829 0a20 2020 2020  _forward().     
-00003430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003440: 2020 2020 2020 2070 6c61 7965 725f 6f75         player_ou
-00003450: 7470 7574 2e6f 7574 7075 7428 706c 6179  tput.output(play
-00003460: 6261 636b 2e63 7572 725f 706f 7329 0a20  back.curr_pos). 
-00003470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003480: 2020 2020 2020 2065 6c69 6620 6320 3d3d         elif c ==
-00003490: 2063 7572 7365 732e 4b45 595f 454e 5445   curses.KEY_ENTE
-000034a0: 523a 0a20 2020 2020 2020 2020 2020 2020  R:.             
-000034b0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-000034c0: 6c61 7965 725f 6f75 7470 7574 2e69 203d  layer_output.i =
-000034d0: 2070 6c61 7965 725f 6f75 7470 7574 2e73   player_output.s
-000034e0: 6372 6f6c 6c65 722e 706f 7320 2d20 310a  croller.pos - 1.
-000034f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003500: 2020 2020 2020 2020 2020 2020 6e65 7874              next
-00003510: 5f73 6f6e 6720 3d20 310a 2020 2020 2020  _song = 1.      
-00003520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003530: 2020 2020 2020 706c 6179 6261 636b 2e73        playback.s
-00003540: 746f 7028 290a 2020 2020 2020 2020 2020  top().          
-00003550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003560: 2020 6272 6561 6b0a 2020 2020 2020 2020    break.        
-00003570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003580: 656c 6966 2063 203d 3d20 6375 7273 6573  elif c == curses
-00003590: 2e4b 4559 5f44 433a 0a20 2020 2020 2020  .KEY_DC:.       
-000035a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000035b0: 2020 2020 2073 656c 6563 7465 645f 736f       selected_so
-000035c0: 6e67 203d 2070 6c61 7965 725f 6f75 7470  ng = player_outp
-000035d0: 7574 2e73 6372 6f6c 6c65 722e 706f 730a  ut.scroller.pos.
-000035e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000035f0: 2020 2020 2020 2020 2020 2020 6465 6c20              del 
-00003600: 706c 6179 6572 5f6f 7574 7075 742e 706c  player_output.pl
-00003610: 6179 6c69 7374 5b73 656c 6563 7465 645f  aylist[selected_
-00003620: 736f 6e67 5d0a 0a20 2020 2020 2020 2020  song]..         
-00003630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003640: 2020 2069 6620 6c6f 6f70 3a0a 2020 2020     if loop:.    
-00003650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003660: 2020 2020 2020 2020 2020 2020 6966 2072              if r
-00003670: 6573 6875 6666 6c65 3a0a 2020 2020 2020  eshuffle:.      
-00003680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003690: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
-000036a0: 7874 5f70 6c61 796c 6973 7420 3d20 706c  xt_playlist = pl
-000036b0: 6179 6c69 7374 5b3a 5d0a 2020 2020 2020  aylist[:].      
-000036c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000036d0: 2020 2020 2020 2020 2020 2020 2020 7368                sh
-000036e0: 7566 666c 6528 6e65 7874 5f70 6c61 796c  uffle(next_playl
-000036f0: 6973 7429 0a20 2020 2020 2020 2020 2020  ist).           
-00003700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003710: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00003720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003730: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00003740: 656c 206e 6578 745f 706c 6179 6c69 7374  el next_playlist
-00003750: 5b73 656c 6563 7465 645f 736f 6e67 5d0a  [selected_song].
-00003760: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003770: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
-00003780: 7965 725f 6f75 7470 7574 2e73 6372 6f6c  yer_output.scrol
-00003790: 6c65 722e 6e75 6d5f 6c69 6e65 7320 2d3d  ler.num_lines -=
-000037a0: 2031 0a20 2020 2020 2020 2020 2020 2020   1.             
-000037b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000037c0: 6620 280a 2020 2020 2020 2020 2020 2020  f (.            
+00003080: 2020 2020 2020 2020 2020 2020 7570 6461              upda
+00003090: 7465 5f6e 6f77 5f70 6c61 7969 6e67 203d  te_now_playing =
+000030a0: 2054 7275 650a 0a20 2020 2020 2020 2020   True..         
+000030b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000030c0: 2020 206c 6173 745f 7469 6d65 7374 616d     last_timestam
+000030d0: 7020 3d20 706c 6179 6261 636b 2e63 7572  p = playback.cur
+000030e0: 725f 706f 730a 2020 2020 2020 2020 2020  r_pos.          
+000030f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003100: 2020 706c 6179 6572 5f6f 7574 7075 742e    player_output.
+00003110: 6f75 7470 7574 2870 6c61 7962 6163 6b2e  output(playback.
+00003120: 6375 7272 5f70 6f73 290a 2020 2020 2020  curr_pos).      
+00003130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003140: 2020 656c 6966 2063 203d 3d20 6375 7273    elif c == curs
+00003150: 6573 2e4b 4559 5f52 4947 4854 3a0a 2020  es.KEY_RIGHT:.  
+00003160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003170: 2020 2020 2020 2020 2020 706c 6179 6261            playba
+00003180: 636b 2e73 6565 6b28 706c 6179 6261 636b  ck.seek(playback
+00003190: 2e63 7572 725f 706f 7320 2b20 5343 5255  .curr_pos + SCRU
+000031a0: 425f 5449 4d45 290a 2020 2020 2020 2020  B_TIME).        
+000031b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000031c0: 2020 2020 6966 2073 7973 2e70 6c61 7466      if sys.platf
+000031d0: 6f72 6d20 3d3d 2022 6461 7277 696e 2220  orm == "darwin" 
+000031e0: 616e 6420 6361 6e5f 6d61 635f 6e6f 775f  and can_mac_now_
+000031f0: 706c 6179 696e 673a 0a20 2020 2020 2020  playing:.       
+00003200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003210: 2020 2020 2020 2020 206d 6163 5f6e 6f77           mac_now
+00003220: 5f70 6c61 7969 6e67 2e70 6f73 203d 2072  _playing.pos = r
+00003230: 6f75 6e64 2870 6c61 7962 6163 6b2e 6375  ound(playback.cu
+00003240: 7272 5f70 6f73 290a 2020 2020 2020 2020  rr_pos).        
+00003250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003260: 2020 2020 2020 2020 7570 6461 7465 5f6e          update_n
+00003270: 6f77 5f70 6c61 7969 6e67 203d 2054 7275  ow_playing = Tru
+00003280: 650a 0a20 2020 2020 2020 2020 2020 2020  e..             
+00003290: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+000032a0: 6173 745f 7469 6d65 7374 616d 7020 3d20  ast_timestamp = 
+000032b0: 706c 6179 6261 636b 2e63 7572 725f 706f  playback.curr_po
+000032c0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+000032d0: 2020 2020 2020 2020 2020 2020 2020 706c                pl
+000032e0: 6179 6572 5f6f 7574 7075 742e 6f75 7470  ayer_output.outp
+000032f0: 7574 2870 6c61 7962 6163 6b2e 6375 7272  ut(playback.curr
+00003300: 5f70 6f73 290a 2020 2020 2020 2020 2020  _pos).          
+00003310: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00003320: 6966 2063 203d 3d20 6375 7273 6573 2e4b  if c == curses.K
+00003330: 4559 5f55 503a 0a20 2020 2020 2020 2020  EY_UP:.         
+00003340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003350: 2020 2070 6c61 7965 725f 6f75 7470 7574     player_output
+00003360: 2e73 6372 6f6c 6c65 722e 7363 726f 6c6c  .scroller.scroll
+00003370: 5f62 6163 6b77 6172 6428 290a 2020 2020  _backward().    
+00003380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003390: 2020 2020 2020 2020 706c 6179 6572 5f6f          player_o
+000033a0: 7574 7075 742e 6f75 7470 7574 2870 6c61  utput.output(pla
+000033b0: 7962 6163 6b2e 6375 7272 5f70 6f73 290a  yback.curr_pos).
+000033c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000033d0: 2020 2020 2020 2020 656c 6966 2063 203d          elif c =
+000033e0: 3d20 6375 7273 6573 2e4b 4559 5f44 4f57  = curses.KEY_DOW
+000033f0: 4e3a 0a20 2020 2020 2020 2020 2020 2020  N:.             
+00003400: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00003410: 6c61 7965 725f 6f75 7470 7574 2e73 6372  layer_output.scr
+00003420: 6f6c 6c65 722e 7363 726f 6c6c 5f66 6f72  oller.scroll_for
+00003430: 7761 7264 2829 0a20 2020 2020 2020 2020  ward().         
+00003440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003450: 2020 2070 6c61 7965 725f 6f75 7470 7574     player_output
+00003460: 2e6f 7574 7075 7428 706c 6179 6261 636b  .output(playback
+00003470: 2e63 7572 725f 706f 7329 0a20 2020 2020  .curr_pos).     
+00003480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003490: 2020 2065 6c69 6620 6320 3d3d 2063 7572     elif c == cur
+000034a0: 7365 732e 4b45 595f 454e 5445 523a 0a20  ses.KEY_ENTER:. 
+000034b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000034c0: 2020 2020 2020 2020 2020 2070 6c61 7965             playe
+000034d0: 725f 6f75 7470 7574 2e69 203d 2070 6c61  r_output.i = pla
+000034e0: 7965 725f 6f75 7470 7574 2e73 6372 6f6c  yer_output.scrol
+000034f0: 6c65 722e 706f 7320 2d20 310a 2020 2020  ler.pos - 1.    
+00003500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003510: 2020 2020 2020 2020 6e65 7874 5f73 6f6e          next_son
+00003520: 6720 3d20 310a 2020 2020 2020 2020 2020  g = 1.          
+00003530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003540: 2020 706c 6179 6261 636b 2e73 746f 7028    playback.stop(
+00003550: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00003560: 2020 2020 2020 2020 2020 2020 2020 6272                br
+00003570: 6561 6b0a 2020 2020 2020 2020 2020 2020  eak.            
+00003580: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00003590: 2063 203d 3d20 6375 7273 6573 2e4b 4559   c == curses.KEY
+000035a0: 5f44 433a 0a20 2020 2020 2020 2020 2020  _DC:.           
+000035b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000035c0: 2073 656c 6563 7465 645f 736f 6e67 203d   selected_song =
+000035d0: 2070 6c61 7965 725f 6f75 7470 7574 2e73   player_output.s
+000035e0: 6372 6f6c 6c65 722e 706f 730a 2020 2020  croller.pos.    
+000035f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003600: 2020 2020 2020 2020 6465 6c20 706c 6179          del play
+00003610: 6572 5f6f 7574 7075 742e 706c 6179 6c69  er_output.playli
+00003620: 7374 5b73 656c 6563 7465 645f 736f 6e67  st[selected_song
+00003630: 5d0a 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00003640: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00003650: 6620 6c6f 6f70 3a0a 2020 2020 2020 2020  f loop:.        
+00003660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003670: 2020 2020 2020 2020 6966 2072 6573 6875          if reshu
+00003680: 6666 6c65 3a0a 2020 2020 2020 2020 2020  ffle:.          
+00003690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000036a0: 2020 2020 2020 2020 2020 6e65 7874 5f70            next_p
+000036b0: 6c61 796c 6973 7420 3d20 706c 6179 6c69  laylist = playli
+000036c0: 7374 5b3a 5d0a 2020 2020 2020 2020 2020  st[:].          
+000036d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000036e0: 2020 2020 2020 2020 2020 7368 7566 666c            shuffl
+000036f0: 6528 6e65 7874 5f70 6c61 796c 6973 7429  e(next_playlist)
+00003700: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003720: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00003730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003740: 2020 2020 2020 2020 2020 2064 656c 206e             del n
+00003750: 6578 745f 706c 6179 6c69 7374 5b73 656c  ext_playlist[sel
+00003760: 6563 7465 645f 736f 6e67 5d0a 0a20 2020  ected_song]..   
+00003770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003780: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
+00003790: 6f75 7470 7574 2e73 6372 6f6c 6c65 722e  output.scroller.
+000037a0: 6e75 6d5f 6c69 6e65 7320 2d3d 2031 0a20  num_lines -= 1. 
+000037b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000037c0: 2020 2020 2020 2020 2020 2069 6620 280a             if (.
 000037d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000037e0: 2020 2020 7365 6c65 6374 6564 5f73 6f6e      selected_son
-000037f0: 6720 3d3d 2070 6c61 7965 725f 6f75 7470  g == player_outp
-00003800: 7574 2e69 0a20 2020 2020 2020 2020 2020  ut.i.           
-00003810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003820: 2029 3a20 2023 2064 656c 6574 6564 2063   ):  # deleted c
-00003830: 7572 7265 6e74 2073 6f6e 670a 2020 2020  urrent song.    
-00003840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003850: 2020 2020 2020 2020 2020 2020 6e65 7874              next
-00003860: 5f73 6f6e 6720 3d20 310a 2020 2020 2020  _song = 1.      
-00003870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003880: 2020 2020 2020 2020 2020 2320 7769 6c6c            # will
-00003890: 2062 6520 696e 6372 656d 656e 7465 6420   be incremented 
-000038a0: 746f 2069 0a20 2020 2020 2020 2020 2020  to i.           
-000038b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038c0: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
-000038d0: 7574 2e73 6372 6f6c 6c65 722e 706f 7320  ut.scroller.pos 
-000038e0: 3d20 706c 6179 6572 5f6f 7574 7075 742e  = player_output.
-000038f0: 6920 2d20 310a 2020 2020 2020 2020 2020  i - 1.          
-00003900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003910: 2020 2020 2020 706c 6179 6572 5f6f 7574        player_out
-00003920: 7075 742e 6920 2d3d 2031 0a20 2020 2020  put.i -= 1.     
-00003930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003940: 2020 2020 2020 2020 2020 2070 6c61 7962             playb
-00003950: 6163 6b2e 7374 6f70 2829 0a20 2020 2020  ack.stop().     
-00003960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003970: 2020 2020 2020 2020 2020 2062 7265 616b             break
-00003980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003990: 2020 2020 2020 2020 2020 2020 2023 2064               # d
-000039a0: 656c 6574 6564 2073 6f6e 6720 6265 666f  eleted song befo
-000039b0: 7265 2063 7572 7265 6e74 0a20 2020 2020  re current.     
-000039c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000039d0: 2020 2020 2020 2069 6620 7365 6c65 6374         if select
-000039e0: 6564 5f73 6f6e 6720 3c20 706c 6179 6572  ed_song < player
-000039f0: 5f6f 7574 7075 742e 693a 0a20 2020 2020  _output.i:.     
-00003a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a10: 2020 2020 2020 2020 2020 2070 6c61 7965             playe
-00003a20: 725f 6f75 7470 7574 2e69 202d 3d20 310a  r_output.i -= 1.
-00003a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a40: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00003a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a60: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
-00003a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a80: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00003a90: 203d 2063 6872 2863 290a 2020 2020 2020   = chr(c).      
-00003aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ab0: 2020 2020 2020 2020 2020 6966 2063 2069            if c i
-00003ac0: 6e20 226e 4e22 3a0a 2020 2020 2020 2020  n "nN":.        
-00003ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ae0: 2020 2020 2020 2020 2020 2020 6966 2028              if (
-00003af0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000037e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000037f0: 7365 6c65 6374 6564 5f73 6f6e 6720 3d3d  selected_song ==
+00003800: 2070 6c61 7965 725f 6f75 7470 7574 2e69   player_output.i
+00003810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003820: 2020 2020 2020 2020 2020 2020 2029 3a20               ): 
+00003830: 2023 2064 656c 6574 6564 2063 7572 7265   # deleted curre
+00003840: 6e74 2073 6f6e 670a 2020 2020 2020 2020  nt song.        
+00003850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003860: 2020 2020 2020 2020 6e65 7874 5f73 6f6e          next_son
+00003870: 6720 3d20 310a 2020 2020 2020 2020 2020  g = 1.          
+00003880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003890: 2020 2020 2020 2320 7769 6c6c 2062 6520        # will be 
+000038a0: 696e 6372 656d 656e 7465 6420 746f 2069  incremented to i
+000038b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000038c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000038d0: 2070 6c61 7965 725f 6f75 7470 7574 2e73   player_output.s
+000038e0: 6372 6f6c 6c65 722e 706f 7320 3d20 706c  croller.pos = pl
+000038f0: 6179 6572 5f6f 7574 7075 742e 6920 2d20  ayer_output.i - 
+00003900: 310a 2020 2020 2020 2020 2020 2020 2020  1.              
+00003910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003920: 2020 706c 6179 6572 5f6f 7574 7075 742e    player_output.
+00003930: 6920 2d3d 2031 0a20 2020 2020 2020 2020  i -= 1.         
+00003940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003950: 2020 2020 2020 2070 6c61 7962 6163 6b2e         playback.
+00003960: 7374 6f70 2829 0a20 2020 2020 2020 2020  stop().         
+00003970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003980: 2020 2020 2020 2062 7265 616b 0a20 2020         break.   
+00003990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000039a0: 2020 2020 2020 2020 2023 2064 656c 6574           # delet
+000039b0: 6564 2073 6f6e 6720 6265 666f 7265 2063  ed song before c
+000039c0: 7572 7265 6e74 0a20 2020 2020 2020 2020  urrent.         
+000039d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000039e0: 2020 2069 6620 7365 6c65 6374 6564 5f73     if selected_s
+000039f0: 6f6e 6720 3c20 706c 6179 6572 5f6f 7574  ong < player_out
+00003a00: 7075 742e 693a 0a20 2020 2020 2020 2020  put.i:.         
+00003a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a20: 2020 2020 2020 2070 6c61 7965 725f 6f75         player_ou
+00003a30: 7470 7574 2e69 202d 3d20 310a 2020 2020  tput.i -= 1.    
+00003a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a50: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00003a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a70: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+00003a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a90: 2020 2020 2020 2020 2020 2063 203d 2063             c = c
+00003aa0: 6872 2863 290a 2020 2020 2020 2020 2020  hr(c).          
+00003ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ac0: 2020 2020 2020 6966 2063 2069 6e20 226e        if c in "n
+00003ad0: 4e22 3a0a 2020 2020 2020 2020 2020 2020  N":.            
+00003ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003af0: 2020 2020 2020 2020 6966 2028 0a20 2020          if (.   
 00003b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b10: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
-00003b20: 6f75 7470 7574 2e69 0a20 2020 2020 2020  output.i.       
-00003b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b20: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
+00003b30: 7574 2e69 0a20 2020 2020 2020 2020 2020  ut.i.           
 00003b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b50: 203d 3d20 6c65 6e28 706c 6179 6572 5f6f   == len(player_o
-00003b60: 7574 7075 742e 706c 6179 6c69 7374 2920  utput.playlist) 
-00003b70: 2d20 310a 2020 2020 2020 2020 2020 2020  - 1.            
+00003b50: 2020 2020 2020 2020 2020 2020 203d 3d20               == 
+00003b60: 6c65 6e28 706c 6179 6572 5f6f 7574 7075  len(player_outpu
+00003b70: 742e 706c 6179 6c69 7374 2920 2d20 310a  t.playlist) - 1.
 00003b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b90: 2020 2020 2020 2020 2020 2020 616e 6420              and 
-00003ba0: 6e6f 7420 6c6f 6f70 0a20 2020 2020 2020  not loop.       
-00003bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003bc0: 2020 2020 2020 2020 2020 2020 2029 3a0a               ):.
-00003bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ba0: 2020 2020 2020 2020 616e 6420 6e6f 7420          and not 
+00003bb0: 6c6f 6f70 0a20 2020 2020 2020 2020 2020  loop.           
+00003bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003bd0: 2020 2020 2020 2020 2029 3a0a 2020 2020           ):.    
 00003be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003bf0: 2020 2020 2020 2020 7061 7373 0a20 2020          pass.   
-00003c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c00: 2020 2020 7061 7373 0a20 2020 2020 2020      pass.       
 00003c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c20: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00003c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c40: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00003c50: 6578 745f 736f 6e67 203d 2031 0a20 2020  ext_song = 1.   
-00003c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c20: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00003c30: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00003c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c50: 2020 2020 2020 2020 2020 206e 6578 745f             next_
+00003c60: 736f 6e67 203d 2031 0a20 2020 2020 2020  song = 1.       
 00003c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c80: 2020 2020 2070 6c61 7962 6163 6b2e 7374       playback.st
-00003c90: 6f70 2829 0a20 2020 2020 2020 2020 2020  op().           
-00003ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003cb0: 2020 2020 2020 2020 2020 2020 2062 7265               bre
-00003cc0: 616b 0a20 2020 2020 2020 2020 2020 2020  ak.             
+00003c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c90: 2070 6c61 7962 6163 6b2e 7374 6f70 2829   playback.stop()
+00003ca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003cc0: 2020 2020 2020 2020 2062 7265 616b 0a20           break. 
 00003cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ce0: 2020 2065 6c69 6620 6320 696e 2022 6242     elif c in "bB
-00003cf0: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
+00003ce0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00003cf0: 6c69 6620 6320 696e 2022 6242 223a 0a20  lif c in "bB":. 
 00003d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d10: 2020 2020 2020 2069 6620 706c 6179 6572         if player
-00003d20: 5f6f 7574 7075 742e 6920 3d3d 2030 3a0a  _output.i == 0:.
-00003d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d20: 2020 2069 6620 706c 6179 6572 5f6f 7574     if player_out
+00003d30: 7075 742e 6920 3d3d 2030 3a0a 2020 2020  put.i == 0:.    
 00003d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d50: 2020 2020 2020 2020 7061 7373 0a20 2020          pass.   
-00003d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d60: 2020 2020 7061 7373 0a20 2020 2020 2020      pass.       
 00003d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d80: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00003d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003da0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00003db0: 6578 745f 736f 6e67 203d 202d 310a 2020  ext_song = -1.  
-00003dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d80: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00003d90: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00003da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003db0: 2020 2020 2020 2020 2020 206e 6578 745f             next_
+00003dc0: 736f 6e67 203d 202d 310a 2020 2020 2020  song = -1.      
 00003dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003de0: 2020 2020 2020 706c 6179 6261 636b 2e73        playback.s
-00003df0: 746f 7028 290a 2020 2020 2020 2020 2020  top().          
-00003e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003e10: 2020 2020 2020 2020 2020 2020 2020 6272                br
-00003e20: 6561 6b0a 2020 2020 2020 2020 2020 2020  eak.            
+00003de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003df0: 2020 706c 6179 6261 636b 2e73 746f 7028    playback.stop(
+00003e00: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00003e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003e20: 2020 2020 2020 2020 2020 6272 6561 6b0a            break.
 00003e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003e40: 2020 2020 656c 6966 2063 2069 6e20 2272      elif c in "r
-00003e50: 5222 3a0a 2020 2020 2020 2020 2020 2020  R":.            
+00003e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003e50: 656c 6966 2063 2069 6e20 2272 5222 3a0a  elif c in "rR":.
 00003e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003e70: 2020 2020 2020 2020 706c 6179 6261 636b          playback
-00003e80: 2e73 746f 7028 290a 2020 2020 2020 2020  .stop().        
-00003e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ea0: 2020 2020 2020 2020 2020 2020 6e65 7874              next
-00003eb0: 5f73 6f6e 6720 3d20 300a 2020 2020 2020  _song = 0.      
-00003ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ed0: 2020 2020 2020 2020 2020 2020 2020 6272                br
-00003ee0: 6561 6b0a 2020 2020 2020 2020 2020 2020  eak.            
+00003e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003e80: 2020 2020 706c 6179 6261 636b 2e73 746f      playback.sto
+00003e90: 7028 290a 2020 2020 2020 2020 2020 2020  p().            
+00003ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003eb0: 2020 2020 2020 2020 6e65 7874 5f73 6f6e          next_son
+00003ec0: 6720 3d20 300a 2020 2020 2020 2020 2020  g = 0.          
+00003ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ee0: 2020 2020 2020 2020 2020 6272 6561 6b0a            break.
 00003ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003f00: 2020 2020 656c 6966 2063 2069 6e20 226c      elif c in "l
-00003f10: 4c22 3a0a 2020 2020 2020 2020 2020 2020  L":.            
+00003f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f10: 656c 6966 2063 2069 6e20 226c 4c22 3a0a  elif c in "lL":.
 00003f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003f30: 2020 2020 2020 2020 706c 6179 6572 5f6f          player_o
-00003f40: 7574 7075 742e 6c6f 6f70 696e 675f 6375  utput.looping_cu
-00003f50: 7272 656e 745f 736f 6e67 203d 2028 0a20  rrent_song = (. 
-00003f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f40: 2020 2020 706c 6179 6572 5f6f 7574 7075      player_outpu
+00003f50: 742e 6c6f 6f70 696e 675f 6375 7272 656e  t.looping_curren
+00003f60: 745f 736f 6e67 203d 2028 0a20 2020 2020  t_song = (.     
 00003f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003f80: 2020 2020 2020 2070 6c61 7965 725f 6f75         player_ou
-00003f90: 7470 7574 2e6c 6f6f 7069 6e67 5f63 7572  tput.looping_cur
-00003fa0: 7265 6e74 5f73 6f6e 6720 2b20 310a 2020  rent_song + 1.  
-00003fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f90: 2020 2070 6c61 7965 725f 6f75 7470 7574     player_output
+00003fa0: 2e6c 6f6f 7069 6e67 5f63 7572 7265 6e74  .looping_current
+00003fb0: 5f73 6f6e 6720 2b20 310a 2020 2020 2020  _song + 1.      
 00003fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003fd0: 2020 2920 2520 6c65 6e28 4c4f 4f50 5f4d    ) % len(LOOP_M
-00003fe0: 4f44 4553 290a 2020 2020 2020 2020 2020  ODES).          
-00003ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004000: 2020 2020 2020 2020 2020 706c 6179 6572            player
-00004010: 5f6f 7574 7075 742e 6f75 7470 7574 2870  _output.output(p
-00004020: 6c61 7962 6163 6b2e 6375 7272 5f70 6f73  layback.curr_pos
-00004030: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00003fd0: 2020 2020 2020 2020 2020 2020 2020 2920                ) 
+00003fe0: 2520 6c65 6e28 4c4f 4f50 5f4d 4f44 4553  % len(LOOP_MODES
+00003ff0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00004000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004010: 2020 2020 2020 706c 6179 6572 5f6f 7574        player_out
+00004020: 7075 742e 6f75 7470 7574 2870 6c61 7962  put.output(playb
+00004030: 6163 6b2e 6375 7272 5f70 6f73 290a 2020  ack.curr_pos).  
 00004040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004050: 2020 656c 6966 2063 2069 6e20 2263 4322    elif c in "cC"
-00004060: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00004050: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00004060: 6966 2063 2069 6e20 2263 4322 3a0a 2020  if c in "cC":.  
 00004070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004080: 2020 2020 2020 706c 6179 6572 5f6f 7574        player_out
-00004090: 7075 742e 636c 6970 5f6d 6f64 6520 3d20  put.clip_mode = 
-000040a0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00004080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004090: 2020 706c 6179 6572 5f6f 7574 7075 742e    player_output.
+000040a0: 636c 6970 5f6d 6f64 6520 3d20 280a 2020  clip_mode = (.  
 000040b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000040c0: 2020 2020 2020 2020 2020 6e6f 7420 706c            not pl
-000040d0: 6179 6572 5f6f 7574 7075 742e 636c 6970  ayer_output.clip
-000040e0: 5f6d 6f64 650a 2020 2020 2020 2020 2020  _mode.          
-000040f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004100: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00004110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000040c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000040d0: 2020 2020 2020 6e6f 7420 706c 6179 6572        not player
+000040e0: 5f6f 7574 7075 742e 636c 6970 5f6d 6f64  _output.clip_mod
+000040f0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00004100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004110: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
 00004120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004130: 6966 2070 6c61 7965 725f 6f75 7470 7574  if player_output
-00004140: 2e63 6c69 705f 6d6f 6465 3a0a 2020 2020  .clip_mode:.    
-00004150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004130: 2020 2020 2020 2020 2020 2020 6966 2070              if p
+00004140: 6c61 7965 725f 6f75 7470 7574 2e63 6c69  layer_output.cli
+00004150: 705f 6d6f 6465 3a0a 2020 2020 2020 2020  p_mode:.        
 00004160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004170: 2020 2020 280a 2020 2020 2020 2020 2020      (.          
-00004180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004180: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
 00004190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000041a0: 2020 636c 6970 5f73 7461 7274 2c0a 2020    clip_start,.  
-000041b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000041a0: 2020 2020 2020 2020 2020 2020 2020 636c                cl
+000041b0: 6970 5f73 7461 7274 2c0a 2020 2020 2020  ip_start,.      
 000041c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000041d0: 2020 2020 2020 2020 2020 636c 6970 5f65            clip_e
-000041e0: 6e64 2c0a 2020 2020 2020 2020 2020 2020  nd,.            
+000041d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000041e0: 2020 2020 2020 636c 6970 5f65 6e64 2c0a        clip_end,.
 000041f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004200: 2020 2020 2020 2020 2020 2020 2920 3d20              ) = 
-00004210: 706c 6179 6572 5f6f 7574 7075 742e 636c  player_output.cl
-00004220: 6970 0a20 2020 2020 2020 2020 2020 2020  ip.             
+00004200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004210: 2020 2020 2020 2020 2920 3d20 706c 6179          ) = play
+00004220: 6572 5f6f 7574 7075 742e 636c 6970 0a20  er_output.clip. 
 00004230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004240: 2020 2020 2020 2020 2020 2070 6c61 7965             playe
-00004250: 725f 6f75 7470 7574 2e64 7572 6174 696f  r_output.duratio
-00004260: 6e20 3d20 280a 2020 2020 2020 2020 2020  n = (.          
-00004270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004250: 2020 2020 2020 2070 6c61 7965 725f 6f75         player_ou
+00004260: 7470 7574 2e64 7572 6174 696f 6e20 3d20  tput.duration = 
+00004270: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
 00004280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004290: 2020 636c 6970 5f65 6e64 202d 2063 6c69    clip_end - cli
-000042a0: 705f 7374 6172 740a 2020 2020 2020 2020  p_start.        
-000042b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004290: 2020 2020 2020 2020 2020 2020 2020 636c                cl
+000042a0: 6970 5f65 6e64 202d 2063 6c69 705f 7374  ip_end - clip_st
+000042b0: 6172 740a 2020 2020 2020 2020 2020 2020  art.            
 000042c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000042d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000042d0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
 000042e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000042f0: 2020 2020 2020 2020 2020 6966 2028 0a20            if (. 
-00004300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000042f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004300: 2020 2020 2020 6966 2028 0a20 2020 2020        if (.     
 00004310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004320: 2020 2020 2020 2020 2020 2070 6c61 7962             playb
-00004330: 6163 6b2e 6375 7272 5f70 6f73 203c 2063  ack.curr_pos < c
-00004340: 6c69 705f 7374 6172 740a 2020 2020 2020  lip_start.      
-00004350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004330: 2020 2020 2020 2070 6c61 7962 6163 6b2e         playback.
+00004340: 6375 7272 5f70 6f73 203c 2063 6c69 705f  curr_pos < clip_
+00004350: 7374 6172 740a 2020 2020 2020 2020 2020  start.          
 00004360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004370: 2020 2020 2020 6f72 2070 6c61 7962 6163        or playbac
-00004380: 6b2e 6375 7272 5f70 6f73 203e 2063 6c69  k.curr_pos > cli
-00004390: 705f 656e 640a 2020 2020 2020 2020 2020  p_end.          
-000043a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000043b0: 2020 2020 2020 2020 2020 2020 2020 293a                ):
-000043c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004380: 2020 6f72 2070 6c61 7962 6163 6b2e 6375    or playback.cu
+00004390: 7272 5f70 6f73 203e 2063 6c69 705f 656e  rr_pos > clip_en
+000043a0: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
+000043b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000043c0: 2020 2020 2020 2020 2020 293a 0a20 2020            ):.   
 000043d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000043e0: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
-000043f0: 7962 6163 6b2e 7365 656b 2863 6c69 705f  yback.seek(clip_
-00004400: 7374 6172 7429 0a20 2020 2020 2020 2020  start).         
-00004410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000043e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000043f0: 2020 2020 2020 2020 2070 6c61 7962 6163           playbac
+00004400: 6b2e 7365 656b 2863 6c69 705f 7374 6172  k.seek(clip_star
+00004410: 7429 0a20 2020 2020 2020 2020 2020 2020  t).             
 00004420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004430: 2020 2069 6620 280a 2020 2020 2020 2020     if (.        
-00004440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004430: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00004440: 6620 280a 2020 2020 2020 2020 2020 2020  f (.            
 00004450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004460: 2020 2020 2020 2020 7379 732e 706c 6174          sys.plat
-00004470: 666f 726d 203d 3d20 2264 6172 7769 6e22  form == "darwin"
-00004480: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004470: 2020 2020 7379 732e 706c 6174 666f 726d      sys.platform
+00004480: 203d 3d20 2264 6172 7769 6e22 0a20 2020   == "darwin".   
 00004490: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000044a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000044b0: 2061 6e64 2063 616e 5f6d 6163 5f6e 6f77   and can_mac_now
-000044c0: 5f70 6c61 7969 6e67 0a20 2020 2020 2020  _playing.       
-000044d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000044b0: 2020 2020 2020 2020 2020 2020 2061 6e64               and
+000044c0: 2063 616e 5f6d 6163 5f6e 6f77 5f70 6c61   can_mac_now_pla
+000044d0: 7969 6e67 0a20 2020 2020 2020 2020 2020  ying.           
 000044e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000044f0: 2020 2020 2029 3a0a 2020 2020 2020 2020       ):.        
-00004500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000044f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004500: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
 00004510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004520: 2020 2020 2020 2020 6d61 635f 6e6f 775f          mac_now_
-00004530: 706c 6179 696e 672e 706f 7320 3d20 726f  playing.pos = ro
-00004540: 756e 6428 0a20 2020 2020 2020 2020 2020  und(.           
-00004550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004530: 2020 2020 6d61 635f 6e6f 775f 706c 6179      mac_now_play
+00004540: 696e 672e 706f 7320 3d20 726f 756e 6428  ing.pos = round(
+00004550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00004560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004570: 2020 2020 2020 2020 2070 6c61 7962 6163           playbac
-00004580: 6b2e 6375 7272 5f70 6f73 0a20 2020 2020  k.curr_pos.     
-00004590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004580: 2020 2020 2070 6c61 7962 6163 6b2e 6375       playback.cu
+00004590: 7272 5f70 6f73 0a20 2020 2020 2020 2020  rr_pos.         
 000045a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000045b0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-000045c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000045b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000045c0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
 000045d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000045e0: 2020 2020 2020 2020 2020 2020 2075 7064               upd
-000045f0: 6174 655f 6e6f 775f 706c 6179 696e 6720  ate_now_playing 
-00004600: 3d20 5472 7565 0a20 2020 2020 2020 2020  = True.         
-00004610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000045e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000045f0: 2020 2020 2020 2020 2075 7064 6174 655f           update_
+00004600: 6e6f 775f 706c 6179 696e 6720 3d20 5472  now_playing = Tr
+00004610: 7565 0a20 2020 2020 2020 2020 2020 2020  ue.             
 00004620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004630: 2020 206c 6173 745f 7469 6d65 7374 616d     last_timestam
-00004640: 7020 3d20 706c 6179 6261 636b 2e63 7572  p = playback.cur
-00004650: 725f 706f 730a 2020 2020 2020 2020 2020  r_pos.          
-00004660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004670: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00004680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004630: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00004640: 6173 745f 7469 6d65 7374 616d 7020 3d20  ast_timestamp = 
+00004650: 706c 6179 6261 636b 2e63 7572 725f 706f  playback.curr_po
+00004660: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+00004670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004680: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
 00004690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000046a0: 2020 2020 2020 2020 706c 6179 6572 5f6f          player_o
-000046b0: 7574 7075 742e 6475 7261 7469 6f6e 203d  utput.duration =
-000046c0: 2066 756c 6c5f 6475 7261 7469 6f6e 0a20   full_duration. 
-000046d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046b0: 2020 2020 706c 6179 6572 5f6f 7574 7075      player_outpu
+000046c0: 742e 6475 7261 7469 6f6e 203d 2066 756c  t.duration = ful
+000046d0: 6c5f 6475 7261 7469 6f6e 0a20 2020 2020  l_duration.     
 000046e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000046f0: 2020 2070 6c61 7965 725f 6f75 7470 7574     player_output
-00004700: 2e6f 7574 7075 7428 706c 6179 6261 636b  .output(playback
-00004710: 2e63 7572 725f 706f 7329 0a20 2020 2020  .curr_pos).     
-00004720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004730: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00004740: 6320 696e 2022 7050 223a 0a20 2020 2020  c in "pP":.     
-00004750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004760: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00004770: 6c61 7965 725f 6f75 7470 7574 2e73 6372  layer_output.scr
-00004780: 6f6c 6c65 722e 706f 7320 3d20 706c 6179  oller.pos = play
-00004790: 6572 5f6f 7574 7075 742e 690a 2020 2020  er_output.i.    
-000047a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046f0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00004700: 6c61 7965 725f 6f75 7470 7574 2e6f 7574  layer_output.out
+00004710: 7075 7428 706c 6179 6261 636b 2e63 7572  put(playback.cur
+00004720: 725f 706f 7329 0a20 2020 2020 2020 2020  r_pos).         
+00004730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004740: 2020 2020 2020 2065 6c69 6620 6320 696e         elif c in
+00004750: 2022 7050 223a 0a20 2020 2020 2020 2020   "pP":.         
+00004760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004770: 2020 2020 2020 2020 2020 2070 6c61 7965             playe
+00004780: 725f 6f75 7470 7574 2e73 6372 6f6c 6c65  r_output.scrolle
+00004790: 722e 706f 7320 3d20 706c 6179 6572 5f6f  r.pos = player_o
+000047a0: 7574 7075 742e 690a 2020 2020 2020 2020  utput.i.        
 000047b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000047c0: 706c 6179 6572 5f6f 7574 7075 742e 7363  player_output.sc
-000047d0: 726f 6c6c 6572 2e72 6573 697a 6528 290a  roller.resize().
-000047e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000047c0: 2020 2020 2020 2020 2020 2020 706c 6179              play
+000047d0: 6572 5f6f 7574 7075 742e 7363 726f 6c6c  er_output.scroll
+000047e0: 6572 2e72 6573 697a 6528 290a 2020 2020  er.resize().    
 000047f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004800: 2020 2020 706c 6179 6572 5f6f 7574 7075      player_outpu
-00004810: 742e 6f75 7470 7574 2870 6c61 7962 6163  t.output(playbac
-00004820: 6b2e 6375 7272 5f70 6f73 290a 2020 2020  k.curr_pos).    
-00004830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004840: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-00004850: 2063 2069 6e20 2267 4722 3a0a 2020 2020   c in "gG":.    
-00004860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004810: 706c 6179 6572 5f6f 7574 7075 742e 6f75  player_output.ou
+00004820: 7470 7574 2870 6c61 7962 6163 6b2e 6375  tput(playback.cu
+00004830: 7272 5f70 6f73 290a 2020 2020 2020 2020  rr_pos).        
+00004840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004850: 2020 2020 2020 2020 656c 6966 2063 2069          elif c i
+00004860: 6e20 2267 4722 3a0a 2020 2020 2020 2020  n "gG":.        
 00004870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004880: 6966 206c 6f6f 703a 0a20 2020 2020 2020  if loop:.       
-00004890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004880: 2020 2020 2020 2020 2020 2020 6966 206c              if l
+00004890: 6f6f 703a 0a20 2020 2020 2020 2020 2020  oop:.           
 000048a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000048b0: 2070 6c61 7962 6163 6b2e 7374 6f70 2829   playback.stop()
-000048c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000048b0: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
+000048c0: 7962 6163 6b2e 7374 6f70 2829 0a20 2020  yback.stop().   
 000048d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000048e0: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
-000048f0: 6f75 7470 7574 2e69 203d 2028 0a20 2020  output.i = (.   
-00004900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000048e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000048f0: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
+00004900: 7574 2e69 203d 2028 0a20 2020 2020 2020  ut.i = (.       
 00004910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004920: 2020 2020 2020 2020 206c 656e 2870 6c61           len(pla
-00004930: 7965 725f 6f75 7470 7574 2e70 6c61 796c  yer_output.playl
-00004940: 6973 7429 202d 2031 0a20 2020 2020 2020  ist) - 1.       
-00004950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004930: 2020 2020 206c 656e 2870 6c61 7965 725f       len(player_
+00004940: 6f75 7470 7574 2e70 6c61 796c 6973 7429  output.playlist)
+00004950: 202d 2031 0a20 2020 2020 2020 2020 2020   - 1.           
 00004960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004970: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+00004970: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
 00004980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004990: 2020 2020 2020 2020 2020 206e 6578 745f             next_
-000049a0: 736f 6e67 203d 2031 0a20 2020 2020 2020  song = 1.       
-000049b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000049a0: 2020 2020 2020 206e 6578 745f 736f 6e67         next_song
+000049b0: 203d 2031 0a20 2020 2020 2020 2020 2020   = 1.           
 000049c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000049d0: 2062 7265 616b 0a20 2020 2020 2020 2020   break.         
-000049e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000049f0: 2020 2020 2020 2065 6c69 6620 6320 696e         elif c in
-00004a00: 2022 6545 223a 0a20 2020 2020 2020 2020   "eE":.         
-00004a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a20: 2020 2020 2020 2020 2020 2070 6c61 7965             playe
-00004a30: 725f 6f75 7470 7574 2e65 6e64 696e 6720  r_output.ending 
-00004a40: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+000049d0: 2020 2020 2020 2020 2020 2020 2062 7265               bre
+000049e0: 616b 0a20 2020 2020 2020 2020 2020 2020  ak.             
+000049f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a00: 2020 2065 6c69 6620 6320 696e 2022 6545     elif c in "eE
+00004a10: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
+00004a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a30: 2020 2020 2020 2070 6c61 7965 725f 6f75         player_ou
+00004a40: 7470 7574 2e65 6e64 696e 6720 3d20 280a  tput.ending = (.
 00004a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a60: 2020 2020 2020 2020 2020 2020 6e6f 7420              not 
-00004a70: 706c 6179 6572 5f6f 7574 7075 742e 656e  player_output.en
-00004a80: 6469 6e67 0a20 2020 2020 2020 2020 2020  ding.           
-00004a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004aa0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00004ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ac0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00004ad0: 6c61 7965 725f 6f75 7470 7574 2e6f 7574  layer_output.out
-00004ae0: 7075 7428 706c 6179 6261 636b 2e63 7572  put(playback.cur
-00004af0: 725f 706f 7329 0a20 2020 2020 2020 2020  r_pos).         
-00004b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b10: 2020 2020 2020 2065 6c69 6620 6320 696e         elif c in
-00004b20: 2022 7151 223a 0a20 2020 2020 2020 2020   "qQ":.         
-00004b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b40: 2020 2020 2020 2020 2020 2070 6c61 7965             playe
-00004b50: 725f 6f75 7470 7574 2e65 6e64 696e 6720  r_output.ending 
-00004b60: 3d20 5472 7565 0a20 2020 2020 2020 2020  = True.         
-00004b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b80: 2020 2020 2020 2020 2020 2062 7265 616b             break
-00004b90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a70: 2020 2020 2020 2020 6e6f 7420 706c 6179          not play
+00004a80: 6572 5f6f 7574 7075 742e 656e 6469 6e67  er_output.ending
+00004a90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ab0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00004ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ad0: 2020 2020 2020 2020 2020 2070 6c61 7965             playe
+00004ae0: 725f 6f75 7470 7574 2e6f 7574 7075 7428  r_output.output(
+00004af0: 706c 6179 6261 636b 2e63 7572 725f 706f  playback.curr_po
+00004b00: 7329 0a20 2020 2020 2020 2020 2020 2020  s).             
+00004b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b20: 2020 2065 6c69 6620 6320 696e 2022 7151     elif c in "qQ
+00004b30: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
+00004b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b50: 2020 2020 2020 2070 6c61 7965 725f 6f75         player_ou
+00004b60: 7470 7574 2e65 6e64 696e 6720 3d20 5472  tput.ending = Tr
+00004b70: 7565 0a20 2020 2020 2020 2020 2020 2020  ue.             
+00004b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b90: 2020 2020 2020 2062 7265 616b 0a20 2020         break.   
 00004ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004bb0: 2065 6c69 6620 6320 696e 2022 6444 223a   elif c in "dD":
-00004bc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004bb0: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
+00004bc0: 6620 6320 696e 2022 6444 223a 0a20 2020  f c in "dD":.   
 00004bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004be0: 2020 2020 2069 6620 706c 6179 6572 5f6f       if player_o
-00004bf0: 7574 7075 742e 7570 6461 7465 5f64 6973  utput.update_dis
-00004c00: 636f 7264 3a0a 2020 2020 2020 2020 2020  cord:.          
-00004c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c20: 2020 2020 2020 2020 2020 2020 2020 706c                pl
-00004c30: 6179 6572 5f6f 7574 7075 742e 7570 6461  ayer_output.upda
-00004c40: 7465 5f64 6973 636f 7264 203d 2046 616c  te_discord = Fal
-00004c50: 7365 0a20 2020 2020 2020 2020 2020 2020  se.             
+00004be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004bf0: 2069 6620 706c 6179 6572 5f6f 7574 7075   if player_outpu
+00004c00: 742e 7570 6461 7465 5f64 6973 636f 7264  t.update_discord
+00004c10: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00004c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c30: 2020 2020 2020 2020 2020 706c 6179 6572            player
+00004c40: 5f6f 7574 7075 742e 7570 6461 7465 5f64  _output.update_d
+00004c50: 6973 636f 7264 203d 2046 616c 7365 0a20  iscord = False. 
 00004c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c70: 2020 2020 2020 2020 2020 2064 6973 636f             disco
-00004c80: 7264 5f70 7265 7365 6e63 655f 7072 6f63  rd_presence_proc
-00004c90: 6573 732e 7465 726d 696e 6174 6528 290a  ess.terminate().
-00004ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c80: 2020 2020 2020 2064 6973 636f 7264 5f70         discord_p
+00004c90: 7265 7365 6e63 655f 7072 6f63 6573 732e  resence_process.
+00004ca0: 7465 726d 696e 6174 6528 290a 2020 2020  terminate().    
 00004cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004cc0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00004cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004cd0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
 00004ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004cf0: 2020 706c 6179 6572 5f6f 7574 7075 742e    player_output.
-00004d00: 7570 6461 7465 5f64 6973 636f 7264 203d  update_discord =
-00004d10: 2054 7275 650a 0a20 2020 2020 2020 2020   True..         
-00004d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d30: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00004d40: 6973 636f 7264 5f74 6974 6c65 5f71 7565  iscord_title_que
-00004d50: 7565 203d 2028 0a20 2020 2020 2020 2020  ue = (.         
-00004d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004cf0: 2020 2020 2020 2020 2020 2020 2020 706c                pl
+00004d00: 6179 6572 5f6f 7574 7075 742e 7570 6461  ayer_output.upda
+00004d10: 7465 5f64 6973 636f 7264 203d 2054 7275  te_discord = Tru
+00004d20: 650a 0a20 2020 2020 2020 2020 2020 2020  e..             
+00004d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d40: 2020 2020 2020 2020 2020 2064 6973 636f             disco
+00004d50: 7264 5f74 6974 6c65 5f71 7565 7565 203d  rd_title_queue =
+00004d60: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
 00004d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d80: 2020 206d 756c 7469 7072 6f63 6573 7369     multiprocessi
-00004d90: 6e67 2e53 696d 706c 6551 7565 7565 2829  ng.SimpleQueue()
-00004da0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004d80: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00004d90: 756c 7469 7072 6f63 6573 7369 6e67 2e53  ultiprocessing.S
+00004da0: 696d 706c 6551 7565 7565 2829 0a20 2020  impleQueue().   
 00004db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004dc0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00004dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004dd0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
 00004de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004df0: 2020 2066 6f72 2063 2069 6e20 706c 6179     for c in play
-00004e00: 6572 5f6f 7574 7075 742e 706c 6179 6c69  er_output.playli
-00004e10: 7374 5b0a 2020 2020 2020 2020 2020 2020  st[.            
+00004df0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00004e00: 6f72 2063 2069 6e20 706c 6179 6572 5f6f  or c in player_o
+00004e10: 7574 7075 742e 706c 6179 6c69 7374 5b0a  utput.playlist[.
 00004e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e40: 706c 6179 6572 5f6f 7574 7075 742e 690a  player_output.i.
-00004e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e40: 2020 2020 2020 2020 2020 2020 706c 6179              play
+00004e50: 6572 5f6f 7574 7075 742e 690a 2020 2020  er_output.i.    
 00004e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e70: 2020 2020 2020 2020 5d5b 315d 3a0a 2020          ][1]:.  
-00004e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e80: 2020 2020 5d5b 315d 3a0a 2020 2020 2020      ][1]:.      
 00004e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ea0: 2020 2020 2020 2020 2020 6469 7363 6f72            discor
-00004eb0: 645f 7469 746c 655f 7175 6575 652e 7075  d_title_queue.pu
-00004ec0: 7428 6329 0a20 2020 2020 2020 2020 2020  t(c).           
-00004ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ee0: 2020 2020 2020 2020 2020 2020 2064 6973               dis
-00004ef0: 636f 7264 5f74 6974 6c65 5f71 7565 7565  cord_title_queue
-00004f00: 2e70 7574 2822 5c6e 2229 0a0a 2020 2020  .put("\n")..    
-00004f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004eb0: 2020 2020 2020 6469 7363 6f72 645f 7469        discord_ti
+00004ec0: 746c 655f 7175 6575 652e 7075 7428 6329  tle_queue.put(c)
+00004ed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ef0: 2020 2020 2020 2020 2064 6973 636f 7264           discord
+00004f00: 5f74 6974 6c65 5f71 7565 7565 2e70 7574  _title_queue.put
+00004f10: 2822 5c6e 2229 0a0a 2020 2020 2020 2020  ("\n")..        
 00004f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f30: 2020 2020 6469 7363 6f72 645f 6172 7469      discord_arti
-00004f40: 7374 5f71 7565 7565 203d 2028 0a20 2020  st_queue = (.   
-00004f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f40: 6469 7363 6f72 645f 6172 7469 7374 5f71  discord_artist_q
+00004f50: 7565 7565 203d 2028 0a20 2020 2020 2020  ueue = (.       
 00004f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f70: 2020 2020 2020 2020 206d 756c 7469 7072           multipr
-00004f80: 6f63 6573 7369 6e67 2e53 696d 706c 6551  ocessing.SimpleQ
-00004f90: 7565 7565 2829 0a20 2020 2020 2020 2020  ueue().         
-00004fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004fb0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00004fc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f80: 2020 2020 206d 756c 7469 7072 6f63 6573       multiproces
+00004f90: 7369 6e67 2e53 696d 706c 6551 7565 7565  sing.SimpleQueue
+00004fa0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00004fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004fc0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
 00004fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004fe0: 2020 2020 2020 2020 2066 6f72 2063 2069           for c i
-00004ff0: 6e20 706c 6179 6572 5f6f 7574 7075 742e  n player_output.
-00005000: 706c 6179 6c69 7374 5b0a 2020 2020 2020  playlist[.      
-00005010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ff0: 2020 2020 2066 6f72 2063 2069 6e20 706c       for c in pl
+00005000: 6179 6572 5f6f 7574 7075 742e 706c 6179  ayer_output.play
+00005010: 6c69 7374 5b0a 2020 2020 2020 2020 2020  list[.          
 00005020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005030: 2020 2020 2020 706c 6179 6572 5f6f 7574        player_out
-00005040: 7075 742e 690a 2020 2020 2020 2020 2020  put.i.          
-00005050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005060: 2020 2020 2020 2020 2020 2020 2020 5d5b                ][
-00005070: 2d33 5d3a 0a20 2020 2020 2020 2020 2020  -3]:.           
-00005080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005040: 2020 706c 6179 6572 5f6f 7574 7075 742e    player_output.
+00005050: 690a 2020 2020 2020 2020 2020 2020 2020  i.              
+00005060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005070: 2020 2020 2020 2020 2020 5d5b 2d33 5d3a            ][-3]:
+00005080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00005090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000050a0: 2064 6973 636f 7264 5f61 7274 6973 745f   discord_artist_
-000050b0: 7175 6575 652e 7075 7428 6329 0a20 2020  queue.put(c).   
-000050c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000050a0: 2020 2020 2020 2020 2020 2020 2064 6973               dis
+000050b0: 636f 7264 5f61 7274 6973 745f 7175 6575  cord_artist_queu
+000050c0: 652e 7075 7428 6329 0a20 2020 2020 2020  e.put(c).       
 000050d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000050e0: 2020 2020 2064 6973 636f 7264 5f61 7274       discord_art
-000050f0: 6973 745f 7175 6575 652e 7075 7428 225c  ist_queue.put("\
-00005100: 6e22 290a 0a20 2020 2020 2020 2020 2020  n")..           
-00005110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005120: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
-00005130: 7965 725f 6f75 7470 7574 2e64 6973 636f  yer_output.disco
-00005140: 7264 5f63 6f6e 6e65 6374 6564 203d 2028  rd_connected = (
-00005150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000050e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000050f0: 2064 6973 636f 7264 5f61 7274 6973 745f   discord_artist_
+00005100: 7175 6575 652e 7075 7428 225c 6e22 290a  queue.put("\n").
+00005110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005130: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
+00005140: 6f75 7470 7574 2e64 6973 636f 7264 5f63  output.discord_c
+00005150: 6f6e 6e65 6374 6564 203d 2028 0a20 2020  onnected = (.   
 00005160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005170: 2020 2020 2020 2020 2020 2020 206d 756c               mul
-00005180: 7469 7072 6f63 6573 7369 6e67 2e56 616c  tiprocessing.Val
-00005190: 7565 2822 6922 2c20 3229 0a20 2020 2020  ue("i", 2).     
-000051a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005180: 2020 2020 2020 2020 206d 756c 7469 7072           multipr
+00005190: 6f63 6573 7369 6e67 2e56 616c 7565 2822  ocessing.Value("
+000051a0: 6922 2c20 3229 0a20 2020 2020 2020 2020  i", 2).         
 000051b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000051c0: 2020 2029 0a0a 2020 2020 2020 2020 2020     )..          
-000051d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000051e0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-000051f0: 7374 6172 7420 6e65 7720 7072 6f63 6573  start new proces
-00005200: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+000051c0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+000051d0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000051e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000051f0: 2020 2020 2020 2020 2020 2320 7374 6172            # star
+00005200: 7420 6e65 7720 7072 6f63 6573 730a 2020  t new process.  
 00005210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005220: 2020 2020 2020 2020 2020 6469 7363 6f72            discor
-00005230: 645f 7072 6573 656e 6365 5f70 726f 6365  d_presence_proce
-00005240: 7373 203d 206d 756c 7469 7072 6f63 6573  ss = multiproces
-00005250: 7369 6e67 2e50 726f 6365 7373 280a 2020  sing.Process(.  
-00005260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005230: 2020 2020 2020 6469 7363 6f72 645f 7072        discord_pr
+00005240: 6573 656e 6365 5f70 726f 6365 7373 203d  esence_process =
+00005250: 206d 756c 7469 7072 6f63 6573 7369 6e67   multiprocessing
+00005260: 2e50 726f 6365 7373 280a 2020 2020 2020  .Process(.      
 00005270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005280: 2020 2020 2020 2020 2020 6461 656d 6f6e            daemon
-00005290: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
-000052a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005290: 2020 2020 2020 6461 656d 6f6e 3d54 7275        daemon=Tru
+000052a0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
 000052b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000052c0: 2020 2074 6172 6765 743d 6469 7363 6f72     target=discor
-000052d0: 645f 7072 6573 656e 6365 5f6c 6f6f 702c  d_presence_loop,
-000052e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000052c0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+000052d0: 6172 6765 743d 6469 7363 6f72 645f 7072  arget=discord_pr
+000052e0: 6573 656e 6365 5f6c 6f6f 702c 0a20 2020  esence_loop,.   
 000052f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005300: 2020 2020 2020 2020 2020 2020 2061 7267               arg
-00005310: 733d 280a 2020 2020 2020 2020 2020 2020  s=(.            
+00005300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005310: 2020 2020 2020 2020 2061 7267 733d 280a           args=(.
 00005320: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00005330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005340: 2020 2020 6469 7363 6f72 645f 7469 746c      discord_titl
-00005350: 655f 7175 6575 652c 0a20 2020 2020 2020  e_queue,.       
-00005360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005350: 6469 7363 6f72 645f 7469 746c 655f 7175  discord_title_qu
+00005360: 6575 652c 0a20 2020 2020 2020 2020 2020  eue,.           
 00005370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005380: 2020 2020 2020 2020 2064 6973 636f 7264           discord
-00005390: 5f61 7274 6973 745f 7175 6575 652c 0a20  _artist_queue,. 
-000053a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005390: 2020 2020 2064 6973 636f 7264 5f61 7274       discord_art
+000053a0: 6973 745f 7175 6575 652c 0a20 2020 2020  ist_queue,.     
 000053b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000053c0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-000053d0: 6c61 7965 725f 6f75 7470 7574 2e64 6973  layer_output.dis
-000053e0: 636f 7264 5f63 6f6e 6e65 6374 6564 2c0a  cord_connected,.
-000053f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000053c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000053d0: 2020 2020 2020 2020 2020 2070 6c61 7965             playe
+000053e0: 725f 6f75 7470 7574 2e64 6973 636f 7264  r_output.discord
+000053f0: 5f63 6f6e 6e65 6374 6564 2c0a 2020 2020  _connected,.    
 00005400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005410: 2020 2020 2020 2020 2020 2020 292c 0a20              ),. 
-00005420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005420: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
 00005430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005440: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00005450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005450: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
 00005460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005470: 2064 6973 636f 7264 5f70 7265 7365 6e63   discord_presenc
-00005480: 655f 7072 6f63 6573 732e 7374 6172 7428  e_process.start(
-00005490: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00005470: 2020 2020 2020 2020 2020 2020 2064 6973               dis
+00005480: 636f 7264 5f70 7265 7365 6e63 655f 7072  cord_presence_pr
+00005490: 6f63 6573 732e 7374 6172 7428 290a 2020  ocess.start().  
 000054a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000054b0: 2020 656c 6966 2063 2069 6e20 2269 4922    elif c in "iI"
-000054c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000054b0: 2020 2020 2020 2020 2020 2020 2020 656c                el
+000054c0: 6966 2063 2069 6e20 2269 4922 3a0a 2020  if c in "iI":.  
 000054d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000054e0: 2020 2020 2020 706c 6179 6572 5f6f 7574        player_out
-000054f0: 7075 742e 7072 6f6d 7074 696e 6720 3d20  put.prompting = 
-00005500: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000054e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000054f0: 2020 706c 6179 6572 5f6f 7574 7075 742e    player_output.
+00005500: 7072 6f6d 7074 696e 6720 3d20 280a 2020  prompting = (.  
 00005510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005520: 2020 2020 2020 2020 2020 2222 2c0a 2020            "",.  
-00005530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005530: 2020 2020 2020 2222 2c0a 2020 2020 2020        "",.      
 00005540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005550: 2020 2020 2020 302c 0a20 2020 2020 2020        0,.       
-00005560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005560: 2020 302c 0a20 2020 2020 2020 2020 2020    0,.           
 00005570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005580: 2050 524f 4d50 545f 4d4f 4445 535b 2269   PROMPT_MODES["i
-00005590: 6e73 6572 7422 5d2c 0a20 2020 2020 2020  nsert"],.       
-000055a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000055b0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-000055c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005580: 2020 2020 2020 2020 2020 2020 2050 524f               PRO
+00005590: 4d50 545f 4d4f 4445 535b 2269 6e73 6572  MPT_MODES["inser
+000055a0: 7422 5d2c 0a20 2020 2020 2020 2020 2020  t"],.           
+000055b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000055c0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
 000055d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000055e0: 2020 2063 7572 7365 732e 6375 7273 5f73     curses.curs_s
-000055f0: 6574 2854 7275 6529 0a20 2020 2020 2020  et(True).       
-00005600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005610: 2020 2020 2020 2020 2020 2020 2073 6372               scr
-00005620: 6565 6e5f 7369 7a65 203d 2073 7464 7363  een_size = stdsc
-00005630: 722e 6765 746d 6178 7978 2829 0a20 2020  r.getmaxyx().   
-00005640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000055e0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000055f0: 7572 7365 732e 6375 7273 5f73 6574 2854  urses.curs_set(T
+00005600: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
+00005610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005620: 2020 2020 2020 2020 2073 6372 6565 6e5f           screen_
+00005630: 7369 7a65 203d 2073 7464 7363 722e 6765  size = stdscr.ge
+00005640: 746d 6178 7978 2829 0a20 2020 2020 2020  tmaxyx().       
 00005650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005660: 2070 6c61 7965 725f 6f75 7470 7574 2e73   player_output.s
-00005670: 6372 6f6c 6c65 722e 7265 7369 7a65 280a  croller.resize(.
-00005680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005660: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
+00005670: 7965 725f 6f75 7470 7574 2e73 6372 6f6c  yer_output.scrol
+00005680: 6c65 722e 7265 7369 7a65 280a 2020 2020  ler.resize(.    
 00005690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000056a0: 2020 2020 2020 2020 7363 7265 656e 5f73          screen_s
-000056b0: 697a 655b 305d 202d 2033 0a20 2020 2020  ize[0] - 3.     
-000056c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000056d0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-000056e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000056a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000056b0: 2020 2020 7363 7265 656e 5f73 697a 655b      screen_size[
+000056c0: 305d 202d 2033 0a20 2020 2020 2020 2020  0] - 3.         
+000056d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000056e0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
 000056f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005700: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
-00005710: 7574 2e6f 7574 7075 7428 706c 6179 6261  ut.output(playba
-00005720: 636b 2e63 7572 725f 706f 7329 0a20 2020  ck.curr_pos).   
-00005730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005740: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
-00005750: 6620 6320 696e 2022 6141 223a 0a20 2020  f c in "aA":.   
-00005760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005710: 2070 6c61 7965 725f 6f75 7470 7574 2e6f   player_output.o
+00005720: 7574 7075 7428 706c 6179 6261 636b 2e63  utput(playback.c
+00005730: 7572 725f 706f 7329 0a20 2020 2020 2020  urr_pos).       
+00005740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005750: 2020 2020 2020 2020 2065 6c69 6620 6320           elif c 
+00005760: 696e 2022 6141 223a 0a20 2020 2020 2020  in "aA":.       
 00005770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005780: 2070 6c61 7965 725f 6f75 7470 7574 2e70   player_output.p
-00005790: 726f 6d70 7469 6e67 203d 2028 0a20 2020  rompting = (.   
-000057a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005780: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
+00005790: 7965 725f 6f75 7470 7574 2e70 726f 6d70  yer_output.promp
+000057a0: 7469 6e67 203d 2028 0a20 2020 2020 2020  ting = (.       
 000057b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000057c0: 2020 2020 2022 222c 0a20 2020 2020 2020       "",.       
-000057d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000057c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000057d0: 2022 222c 0a20 2020 2020 2020 2020 2020   "",.           
 000057e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000057f0: 2030 2c0a 2020 2020 2020 2020 2020 2020   0,.            
+000057f0: 2020 2020 2020 2020 2020 2020 2030 2c0a               0,.
 00005800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005810: 2020 2020 2020 2020 2020 2020 5052 4f4d              PROM
-00005820: 5054 5f4d 4f44 4553 5b22 6164 6422 5d2c  PT_MODES["add"],
-00005830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005820: 2020 2020 2020 2020 5052 4f4d 5054 5f4d          PROMPT_M
+00005830: 4f44 4553 5b22 6164 6422 5d2c 0a20 2020  ODES["add"],.   
 00005840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005850: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00005860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005870: 2020 2020 2020 2020 2020 2063 7572 7365             curse
-00005880: 732e 6375 7273 5f73 6574 2854 7275 6529  s.curs_set(True)
-00005890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005860: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+00005870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005880: 2020 2020 2020 2063 7572 7365 732e 6375         curses.cu
+00005890: 7273 5f73 6574 2854 7275 6529 0a20 2020  rs_set(True).   
 000058a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000058b0: 2020 2020 2073 6372 6565 6e5f 7369 7a65       screen_size
-000058c0: 203d 2073 7464 7363 722e 6765 746d 6178   = stdscr.getmax
-000058d0: 7978 2829 0a20 2020 2020 2020 2020 2020  yx().           
-000058e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000058f0: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
-00005900: 6f75 7470 7574 2e73 6372 6f6c 6c65 722e  output.scroller.
-00005910: 7265 7369 7a65 280a 2020 2020 2020 2020  resize(.        
-00005920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000058b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000058c0: 2073 6372 6565 6e5f 7369 7a65 203d 2073   screen_size = s
+000058d0: 7464 7363 722e 6765 746d 6178 7978 2829  tdscr.getmaxyx()
+000058e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000058f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005900: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
+00005910: 7574 2e73 6372 6f6c 6c65 722e 7265 7369  ut.scroller.resi
+00005920: 7a65 280a 2020 2020 2020 2020 2020 2020  ze(.            
 00005930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005940: 7363 7265 656e 5f73 697a 655b 305d 202d  screen_size[0] -
-00005950: 2033 0a20 2020 2020 2020 2020 2020 2020   3.             
+00005940: 2020 2020 2020 2020 2020 2020 7363 7265              scre
+00005950: 656e 5f73 697a 655b 305d 202d 2033 0a20  en_size[0] - 3. 
 00005960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005970: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00005980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005990: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
-000059a0: 7965 725f 6f75 7470 7574 2e6f 7574 7075  yer_output.outpu
-000059b0: 7428 706c 6179 6261 636b 2e63 7572 725f  t(playback.curr_
-000059c0: 706f 7329 0a20 2020 2020 2020 2020 2020  pos).           
-000059d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000059e0: 2020 2020 2065 6c69 6620 6320 696e 2022       elif c in "
-000059f0: 7454 223a 0a20 2020 2020 2020 2020 2020  tT":.           
-00005a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a10: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
-00005a20: 6f75 7470 7574 2e70 726f 6d70 7469 6e67  output.prompting
-00005a30: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
-00005a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a50: 2020 2020 2020 2020 2020 2020 2022 222c               "",
-00005a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005980: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00005990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000059a0: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
+000059b0: 6f75 7470 7574 2e6f 7574 7075 7428 706c  output.output(pl
+000059c0: 6179 6261 636b 2e63 7572 725f 706f 7329  ayback.curr_pos)
+000059d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000059e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000059f0: 2065 6c69 6620 6320 696e 2022 7454 223a   elif c in "tT":
+00005a00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a20: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
+00005a30: 7574 2e70 726f 6d70 7469 6e67 203d 2028  ut.prompting = (
+00005a40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a60: 2020 2020 2020 2020 2022 222c 0a20 2020           "",.   
 00005a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a80: 2020 2020 2020 2020 2030 2c0a 2020 2020           0,.    
-00005a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a90: 2020 2020 2030 2c0a 2020 2020 2020 2020       0,.        
 00005aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ab0: 2020 2020 5052 4f4d 5054 5f4d 4f44 4553      PROMPT_MODES
-00005ac0: 5b22 7461 6722 5d2c 0a20 2020 2020 2020  ["tag"],.       
-00005ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ae0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-00005af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ac0: 5052 4f4d 5054 5f4d 4f44 4553 5b22 7461  PROMPT_MODES["ta
+00005ad0: 6722 5d2c 0a20 2020 2020 2020 2020 2020  g"],.           
+00005ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005af0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
 00005b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b10: 2020 2063 7572 7365 732e 6375 7273 5f73     curses.curs_s
-00005b20: 6574 2854 7275 6529 0a20 2020 2020 2020  et(True).       
-00005b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b40: 2020 2020 2020 2020 2020 2020 2073 6372               scr
-00005b50: 6565 6e5f 7369 7a65 203d 2073 7464 7363  een_size = stdsc
-00005b60: 722e 6765 746d 6178 7978 2829 0a20 2020  r.getmaxyx().   
-00005b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005b10: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00005b20: 7572 7365 732e 6375 7273 5f73 6574 2854  urses.curs_set(T
+00005b30: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
+00005b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005b50: 2020 2020 2020 2020 2073 6372 6565 6e5f           screen_
+00005b60: 7369 7a65 203d 2073 7464 7363 722e 6765  size = stdscr.ge
+00005b70: 746d 6178 7978 2829 0a20 2020 2020 2020  tmaxyx().       
 00005b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b90: 2070 6c61 7965 725f 6f75 7470 7574 2e73   player_output.s
-00005ba0: 6372 6f6c 6c65 722e 7265 7369 7a65 280a  croller.resize(.
-00005bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005b90: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
+00005ba0: 7965 725f 6f75 7470 7574 2e73 6372 6f6c  yer_output.scrol
+00005bb0: 6c65 722e 7265 7369 7a65 280a 2020 2020  ler.resize(.    
 00005bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005bd0: 2020 2020 2020 2020 7363 7265 656e 5f73          screen_s
-00005be0: 697a 655b 305d 202d 2033 0a20 2020 2020  ize[0] - 3.     
-00005bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c00: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00005c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005be0: 2020 2020 7363 7265 656e 5f73 697a 655b      screen_size[
+00005bf0: 305d 202d 2033 0a20 2020 2020 2020 2020  0] - 3.         
+00005c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c10: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
 00005c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c30: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
-00005c40: 7574 2e6f 7574 7075 7428 706c 6179 6261  ut.output(playba
-00005c50: 636b 2e63 7572 725f 706f 7329 0a20 2020  ck.curr_pos).   
-00005c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c70: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
-00005c80: 6620 6320 696e 2022 6d4d 223a 0a20 2020  f c in "mM":.   
-00005c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c40: 2070 6c61 7965 725f 6f75 7470 7574 2e6f   player_output.o
+00005c50: 7574 7075 7428 706c 6179 6261 636b 2e63  utput(playback.c
+00005c60: 7572 725f 706f 7329 0a20 2020 2020 2020  urr_pos).       
+00005c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c80: 2020 2020 2020 2020 2065 6c69 6620 6320           elif c 
+00005c90: 696e 2022 6d4d 223a 0a20 2020 2020 2020  in "mM":.       
 00005ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005cb0: 2069 6620 706c 6179 6572 5f6f 7574 7075   if player_outpu
-00005cc0: 742e 766f 6c75 6d65 203d 3d20 303a 0a20  t.volume == 0:. 
-00005cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005cb0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00005cc0: 706c 6179 6572 5f6f 7574 7075 742e 766f  player_output.vo
+00005cd0: 6c75 6d65 203d 3d20 303a 0a20 2020 2020  lume == 0:.     
 00005ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005cf0: 2020 2020 2020 2070 6c61 7965 725f 6f75         player_ou
-00005d00: 7470 7574 2e76 6f6c 756d 6520 3d20 7072  tput.volume = pr
-00005d10: 6576 5f76 6f6c 756d 650a 2020 2020 2020  ev_volume.      
-00005d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d30: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00005d40: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00005cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d00: 2020 2070 6c61 7965 725f 6f75 7470 7574     player_output
+00005d10: 2e76 6f6c 756d 6520 3d20 7072 6576 5f76  .volume = prev_v
+00005d20: 6f6c 756d 650a 2020 2020 2020 2020 2020  olume.          
+00005d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d40: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
 00005d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d60: 2020 2020 2020 2020 2020 2020 706c 6179              play
-00005d70: 6572 5f6f 7574 7075 742e 766f 6c75 6d65  er_output.volume
-00005d80: 203d 2030 0a20 2020 2020 2020 2020 2020   = 0.           
-00005d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005da0: 2020 2020 2020 2020 2070 6c61 7962 6163           playbac
-00005db0: 6b2e 7365 745f 766f 6c75 6d65 2870 6c61  k.set_volume(pla
-00005dc0: 7965 725f 6f75 7470 7574 2e76 6f6c 756d  yer_output.volum
-00005dd0: 6529 0a0a 2020 2020 2020 2020 2020 2020  e)..            
+00005d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d70: 2020 2020 2020 2020 706c 6179 6572 5f6f          player_o
+00005d80: 7574 7075 742e 766f 6c75 6d65 203d 2030  utput.volume = 0
+00005d90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005db0: 2020 2020 2070 6c61 7962 6163 6b2e 7365       playback.se
+00005dc0: 745f 766f 6c75 6d65 2870 6c61 7965 725f  t_volume(player_
+00005dd0: 6f75 7470 7574 2e76 6f6c 756d 6529 0a0a  output.volume)..
 00005de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005df0: 2020 2020 2020 2020 706c 6179 6572 5f6f          player_o
-00005e00: 7574 7075 742e 6f75 7470 7574 2870 6c61  utput.output(pla
-00005e10: 7962 6163 6b2e 6375 7272 5f70 6f73 290a  yback.curr_pos).
-00005e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e00: 2020 2020 706c 6179 6572 5f6f 7574 7075      player_outpu
+00005e10: 742e 6f75 7470 7574 2870 6c61 7962 6163  t.output(playbac
+00005e20: 6b2e 6375 7272 5f70 6f73 290a 2020 2020  k.curr_pos).    
 00005e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e40: 656c 6966 2063 2069 6e20 2276 5622 3a0a  elif c in "vV":.
-00005e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e40: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00005e50: 2063 2069 6e20 2276 5622 3a0a 2020 2020   c in "vV":.    
 00005e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e70: 2020 2020 706c 6179 6572 5f6f 7574 7075      player_outpu
-00005e80: 742e 7669 7375 616c 697a 6520 3d20 280a  t.visualize = (.
-00005e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e80: 706c 6179 6572 5f6f 7574 7075 742e 7669  player_output.vi
+00005e90: 7375 616c 697a 6520 3d20 280a 2020 2020  sualize = (.    
 00005ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005eb0: 2020 2020 2020 2020 6e6f 7420 706c 6179          not play
-00005ec0: 6572 5f6f 7574 7075 742e 7669 7375 616c  er_output.visual
-00005ed0: 697a 650a 2020 2020 2020 2020 2020 2020  ize.            
+00005eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ec0: 2020 2020 6e6f 7420 706c 6179 6572 5f6f      not player_o
+00005ed0: 7574 7075 742e 7669 7375 616c 697a 650a  utput.visualize.
 00005ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ef0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00005f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f10: 2020 2020 2020 2020 2020 2020 2020 706c                pl
-00005f20: 6179 6572 5f6f 7574 7075 742e 6f75 7470  ayer_output.outp
-00005f30: 7574 2870 6c61 7962 6163 6b2e 6375 7272  ut(playback.curr
-00005f40: 5f70 6f73 290a 2020 2020 2020 2020 2020  _pos).          
-00005f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f60: 2020 2020 2020 656c 6966 2063 203d 3d20        elif c == 
-00005f70: 2220 223a 0a20 2020 2020 2020 2020 2020  " ":.           
-00005f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f90: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
-00005fa0: 6f75 7470 7574 2e70 6175 7365 6420 3d20  output.paused = 
-00005fb0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00005ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f00: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00005f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f20: 2020 2020 2020 2020 2020 706c 6179 6572            player
+00005f30: 5f6f 7574 7075 742e 6f75 7470 7574 2870  _output.output(p
+00005f40: 6c61 7962 6163 6b2e 6375 7272 5f70 6f73  layback.curr_pos
+00005f50: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00005f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f70: 2020 656c 6966 2063 203d 3d20 2220 223a    elif c == " ":
+00005f80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005fa0: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
+00005fb0: 7574 2e70 6175 7365 6420 3d20 280a 2020  ut.paused = (.  
 00005fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005fd0: 2020 2020 2020 2020 2020 6e6f 7420 706c            not pl
-00005fe0: 6179 6572 5f6f 7574 7075 742e 7061 7573  ayer_output.paus
-00005ff0: 6564 0a20 2020 2020 2020 2020 2020 2020  ed.             
+00005fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005fe0: 2020 2020 2020 6e6f 7420 706c 6179 6572        not player
+00005ff0: 5f6f 7574 7075 742e 7061 7573 6564 0a20  _output.paused. 
 00006000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006010: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-00006020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006030: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00006040: 2070 6c61 7965 725f 6f75 7470 7574 2e70   player_output.p
-00006050: 6175 7365 643a 0a20 2020 2020 2020 2020  aused:.         
-00006060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006070: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00006080: 6c61 7962 6163 6b2e 7061 7573 6528 290a  layback.pause().
-00006090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006020: 2020 2029 0a0a 2020 2020 2020 2020 2020     )..          
+00006030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006040: 2020 2020 2020 2020 2020 6966 2070 6c61            if pla
+00006050: 7965 725f 6f75 7470 7574 2e70 6175 7365  yer_output.pause
+00006060: 643a 0a20 2020 2020 2020 2020 2020 2020  d:.             
+00006070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006080: 2020 2020 2020 2020 2020 2070 6c61 7962             playb
+00006090: 6163 6b2e 7061 7573 6528 290a 2020 2020  ack.pause().    
 000060a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060b0: 2020 2020 2020 2020 7061 7573 655f 7374          pause_st
-000060c0: 6172 7420 3d20 7469 6d65 2829 0a20 2020  art = time().   
-000060d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000060b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000060c0: 2020 2020 7061 7573 655f 7374 6172 7420      pause_start 
+000060d0: 3d20 7469 6d65 2829 0a20 2020 2020 2020  = time().       
 000060e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060f0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00006100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006110: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00006120: 6c61 7962 6163 6b2e 7265 7375 6d65 2829  layback.resume()
-00006130: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000060f0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00006100: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00006110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006120: 2020 2020 2020 2020 2020 2070 6c61 7962             playb
+00006130: 6163 6b2e 7265 7375 6d65 2829 0a20 2020  ack.resume().   
 00006140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006150: 2020 2020 2020 2020 2073 7461 7274 5f74           start_t
-00006160: 696d 6520 2b3d 2074 696d 6528 2920 2d20  ime += time() - 
-00006170: 7061 7573 655f 7374 6172 740a 0a20 2020  pause_start..   
-00006180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006160: 2020 2020 2073 7461 7274 5f74 696d 6520       start_time 
+00006170: 2b3d 2074 696d 6528 2920 2d20 7061 7573  += time() - paus
+00006180: 655f 7374 6172 740a 0a20 2020 2020 2020  e_start..       
 00006190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061a0: 2069 6620 280a 2020 2020 2020 2020 2020   if (.          
-000061b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061c0: 2020 2020 2020 2020 2020 2020 2020 7379                sy
-000061d0: 732e 706c 6174 666f 726d 203d 3d20 2264  s.platform == "d
-000061e0: 6172 7769 6e22 0a20 2020 2020 2020 2020  arwin".         
-000061f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006200: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00006210: 6e64 2063 616e 5f6d 6163 5f6e 6f77 5f70  nd can_mac_now_p
-00006220: 6c61 7969 6e67 0a20 2020 2020 2020 2020  laying.         
-00006230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006240: 2020 2020 2020 2020 2020 2029 3a0a 2020             ):.  
-00006250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000061a0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000061b0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000061c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000061d0: 2020 2020 2020 2020 2020 7379 732e 706c            sys.pl
+000061e0: 6174 666f 726d 203d 3d20 2264 6172 7769  atform == "darwi
+000061f0: 6e22 0a20 2020 2020 2020 2020 2020 2020  n".             
+00006200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006210: 2020 2020 2020 2020 2020 2061 6e64 2063             and c
+00006220: 616e 5f6d 6163 5f6e 6f77 5f70 6c61 7969  an_mac_now_playi
+00006230: 6e67 0a20 2020 2020 2020 2020 2020 2020  ng.             
+00006240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006250: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
 00006260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006270: 2020 2020 2020 6d61 635f 6e6f 775f 706c        mac_now_pl
-00006280: 6179 696e 672e 7061 7573 6564 203d 2028  aying.paused = (
-00006290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006280: 2020 6d61 635f 6e6f 775f 706c 6179 696e    mac_now_playin
+00006290: 672e 7061 7573 6564 203d 2028 0a20 2020  g.paused = (.   
 000062a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062b0: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
-000062c0: 7965 725f 6f75 7470 7574 2e70 6175 7365  yer_output.pause
-000062d0: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
+000062b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000062c0: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
+000062d0: 6f75 7470 7574 2e70 6175 7365 640a 2020  output.paused.  
 000062e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062f0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00006300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000062f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006300: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
 00006310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006320: 2020 2020 6966 2070 6c61 7965 725f 6f75      if player_ou
-00006330: 7470 7574 2e70 6175 7365 643a 0a20 2020  tput.paused:.   
-00006340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006330: 6966 2070 6c61 7965 725f 6f75 7470 7574  if player_output
+00006340: 2e70 6175 7365 643a 0a20 2020 2020 2020  .paused:.       
 00006350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006360: 2020 2020 2020 2020 206d 6163 5f6e 6f77           mac_now
-00006370: 5f70 6c61 7969 6e67 2e70 6175 7365 2829  _playing.pause()
-00006380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006370: 2020 2020 206d 6163 5f6e 6f77 5f70 6c61       mac_now_pla
+00006380: 7969 6e67 2e70 6175 7365 2829 0a20 2020  ying.pause().   
 00006390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000063a0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-000063b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063b0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
 000063c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000063d0: 2020 2020 2020 2020 2020 206d 6163 5f6e             mac_n
-000063e0: 6f77 5f70 6c61 7969 6e67 2e72 6573 756d  ow_playing.resum
-000063f0: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
+000063d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063e0: 2020 2020 2020 206d 6163 5f6e 6f77 5f70         mac_now_p
+000063f0: 6c61 7969 6e67 2e72 6573 756d 6528 290a  laying.resume().
 00006400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006410: 2020 2020 2020 2020 2020 2020 7570 6461              upda
-00006420: 7465 5f6e 6f77 5f70 6c61 7969 6e67 203d  te_now_playing =
-00006430: 2054 7275 650a 0a20 2020 2020 2020 2020   True..         
-00006440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006450: 2020 2020 2020 2020 2020 2070 6c61 7965             playe
-00006460: 725f 6f75 7470 7574 2e6f 7574 7075 7428  r_output.output(
-00006470: 706c 6179 6261 636b 2e63 7572 725f 706f  playback.curr_po
-00006480: 7329 0a20 2020 2020 2020 2020 2020 2020  s).             
+00006410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006420: 2020 2020 2020 2020 7570 6461 7465 5f6e          update_n
+00006430: 6f77 5f70 6c61 7969 6e67 203d 2054 7275  ow_playing = Tru
+00006440: 650a 0a20 2020 2020 2020 2020 2020 2020  e..             
+00006450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006460: 2020 2020 2020 2070 6c61 7965 725f 6f75         player_ou
+00006470: 7470 7574 2e6f 7574 7075 7428 706c 6179  tput.output(play
+00006480: 6261 636b 2e63 7572 725f 706f 7329 0a20  back.curr_pos). 
 00006490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000064a0: 2020 2065 6c69 6620 6320 3d3d 2022 5b22     elif c == "["
-000064b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000064a0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+000064b0: 6c69 6620 6320 3d3d 2022 5b22 3a0a 2020  lif c == "[":.  
 000064c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000064d0: 2020 2020 2020 706c 6179 6572 5f6f 7574        player_out
-000064e0: 7075 742e 766f 6c75 6d65 203d 206d 6178  put.volume = max
-000064f0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000064d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000064e0: 2020 706c 6179 6572 5f6f 7574 7075 742e    player_output.
+000064f0: 766f 6c75 6d65 203d 206d 6178 280a 2020  volume = max(.  
 00006500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006510: 2020 2020 2020 2020 2020 302c 2070 6c61            0, pla
-00006520: 7965 725f 6f75 7470 7574 2e76 6f6c 756d  yer_output.volum
-00006530: 6520 2d20 564f 4c55 4d45 5f53 5445 500a  e - VOLUME_STEP.
-00006540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006520: 2020 2020 2020 302c 2070 6c61 7965 725f        0, player_
+00006530: 6f75 7470 7574 2e76 6f6c 756d 6520 2d20  output.volume - 
+00006540: 564f 4c55 4d45 5f53 5445 500a 2020 2020  VOLUME_STEP.    
 00006550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006560: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00006570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006580: 2020 2020 2020 2020 2020 706c 6179 6261            playba
-00006590: 636b 2e73 6574 5f76 6f6c 756d 6528 706c  ck.set_volume(pl
-000065a0: 6179 6572 5f6f 7574 7075 742e 766f 6c75  ayer_output.volu
-000065b0: 6d65 290a 0a20 2020 2020 2020 2020 2020  me)..           
-000065c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065d0: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
-000065e0: 6f75 7470 7574 2e6f 7574 7075 7428 706c  output.output(pl
-000065f0: 6179 6261 636b 2e63 7572 725f 706f 7329  ayback.curr_pos)
-00006600: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00006560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006570: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00006580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006590: 2020 2020 2020 706c 6179 6261 636b 2e73        playback.s
+000065a0: 6574 5f76 6f6c 756d 6528 706c 6179 6572  et_volume(player
+000065b0: 5f6f 7574 7075 742e 766f 6c75 6d65 290a  _output.volume).
+000065c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000065d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000065e0: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
+000065f0: 7574 2e6f 7574 7075 7428 706c 6179 6261  ut.output(playba
+00006600: 636b 2e63 7572 725f 706f 7329 0a0a 2020  ck.curr_pos)..  
 00006610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006620: 2020 2020 2020 7072 6576 5f76 6f6c 756d        prev_volum
-00006630: 6520 3d20 706c 6179 6572 5f6f 7574 7075  e = player_outpu
-00006640: 742e 766f 6c75 6d65 0a20 2020 2020 2020  t.volume.       
-00006650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006660: 2020 2020 2020 2020 2065 6c69 6620 6320           elif c 
-00006670: 3d3d 2022 5d22 3a0a 2020 2020 2020 2020  == "]":.        
-00006680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006690: 2020 2020 2020 2020 2020 2020 706c 6179              play
-000066a0: 6572 5f6f 7574 7075 742e 766f 6c75 6d65  er_output.volume
-000066b0: 203d 206d 696e 280a 2020 2020 2020 2020   = min(.        
-000066c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006630: 2020 7072 6576 5f76 6f6c 756d 6520 3d20    prev_volume = 
+00006640: 706c 6179 6572 5f6f 7574 7075 742e 766f  player_output.vo
+00006650: 6c75 6d65 0a20 2020 2020 2020 2020 2020  lume.           
+00006660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006670: 2020 2020 2065 6c69 6620 6320 3d3d 2022       elif c == "
+00006680: 5d22 3a0a 2020 2020 2020 2020 2020 2020  ]":.            
+00006690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000066a0: 2020 2020 2020 2020 706c 6179 6572 5f6f          player_o
+000066b0: 7574 7075 742e 766f 6c75 6d65 203d 206d  utput.volume = m
+000066c0: 696e 280a 2020 2020 2020 2020 2020 2020  in(.            
 000066d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000066e0: 312c 2070 6c61 7965 725f 6f75 7470 7574  1, player_output
-000066f0: 2e76 6f6c 756d 6520 2b20 564f 4c55 4d45  .volume + VOLUME
-00006700: 5f53 5445 500a 2020 2020 2020 2020 2020  _STEP.          
-00006710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006720: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00006730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000066e0: 2020 2020 2020 2020 2020 2020 312c 2070              1, p
+000066f0: 6c61 7965 725f 6f75 7470 7574 2e76 6f6c  layer_output.vol
+00006700: 756d 6520 2b20 564f 4c55 4d45 5f53 5445  ume + VOLUME_STE
+00006710: 500a 2020 2020 2020 2020 2020 2020 2020  P.              
+00006720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006730: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
 00006740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006750: 706c 6179 6261 636b 2e73 6574 5f76 6f6c  playback.set_vol
-00006760: 756d 6528 706c 6179 6572 5f6f 7574 7075  ume(player_outpu
-00006770: 742e 766f 6c75 6d65 290a 0a20 2020 2020  t.volume)..     
-00006780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006790: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-000067a0: 6c61 7965 725f 6f75 7470 7574 2e6f 7574  layer_output.out
-000067b0: 7075 7428 706c 6179 6261 636b 2e63 7572  put(playback.cur
-000067c0: 725f 706f 7329 0a0a 2020 2020 2020 2020  r_pos)..        
-000067d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000067e0: 2020 2020 2020 2020 2020 2020 7072 6576              prev
-000067f0: 5f76 6f6c 756d 6520 3d20 706c 6179 6572  _volume = player
-00006800: 5f6f 7574 7075 742e 766f 6c75 6d65 0a20  _output.volume. 
-00006810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006820: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00006830: 6c69 6620 6320 696e 2022 5c72 5c6e 223a  lif c in "\r\n":
-00006840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006750: 2020 2020 2020 2020 2020 2020 706c 6179              play
+00006760: 6261 636b 2e73 6574 5f76 6f6c 756d 6528  back.set_volume(
+00006770: 706c 6179 6572 5f6f 7574 7075 742e 766f  player_output.vo
+00006780: 6c75 6d65 290a 0a20 2020 2020 2020 2020  lume)..         
+00006790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000067a0: 2020 2020 2020 2020 2020 2070 6c61 7965             playe
+000067b0: 725f 6f75 7470 7574 2e6f 7574 7075 7428  r_output.output(
+000067c0: 706c 6179 6261 636b 2e63 7572 725f 706f  playback.curr_po
+000067d0: 7329 0a0a 2020 2020 2020 2020 2020 2020  s)..            
+000067e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000067f0: 2020 2020 2020 2020 7072 6576 5f76 6f6c          prev_vol
+00006800: 756d 6520 3d20 706c 6179 6572 5f6f 7574  ume = player_out
+00006810: 7075 742e 766f 6c75 6d65 0a20 2020 2020  put.volume.     
+00006820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006830: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00006840: 6320 696e 2022 5c72 5c6e 223a 0a20 2020  c in "\r\n":.   
 00006850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006860: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
-00006870: 7574 2e69 203d 2028 0a20 2020 2020 2020  ut.i = (.       
-00006880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006870: 2070 6c61 7965 725f 6f75 7470 7574 2e69   player_output.i
+00006880: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
 00006890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068a0: 2070 6c61 7965 725f 6f75 7470 7574 2e73   player_output.s
-000068b0: 6372 6f6c 6c65 722e 706f 7320 2d20 310a  croller.pos - 1.
-000068c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000068a0: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
+000068b0: 7965 725f 6f75 7470 7574 2e73 6372 6f6c  yer_output.scrol
+000068c0: 6c65 722e 706f 7320 2d20 310a 2020 2020  ler.pos - 1.    
 000068d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068e0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-000068f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006900: 2020 2020 2020 2020 2020 6e65 7874 5f73            next_s
-00006910: 6f6e 6720 3d20 310a 2020 2020 2020 2020  ong = 1.        
-00006920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006930: 2020 2020 2020 2020 2020 2020 706c 6179              play
-00006940: 6261 636b 2e73 746f 7028 290a 2020 2020  back.stop().    
-00006950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000068e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000068f0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00006900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006910: 2020 2020 2020 6e65 7874 5f73 6f6e 6720        next_song 
+00006920: 3d20 310a 2020 2020 2020 2020 2020 2020  = 1.            
+00006930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006940: 2020 2020 2020 2020 706c 6179 6261 636b          playback
+00006950: 2e73 746f 7028 290a 2020 2020 2020 2020  .stop().        
 00006960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006970: 6272 6561 6b0a 2020 2020 2020 2020 2020  break.          
-00006980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006990: 2020 2020 2020 656c 6966 2063 2069 6e20        elif c in 
-000069a0: 225c 625c 7837 6622 3a0a 2020 2020 2020  "\b\x7f":.      
-000069b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069c0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000069d0: 6c65 6374 6564 5f73 6f6e 6720 3d20 706c  lected_song = pl
-000069e0: 6179 6572 5f6f 7574 7075 742e 7363 726f  ayer_output.scro
-000069f0: 6c6c 6572 2e70 6f73 0a20 2020 2020 2020  ller.pos.       
-00006a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a10: 2020 2020 2020 2020 2020 2020 2064 656c               del
-00006a20: 2070 6c61 7965 725f 6f75 7470 7574 2e70   player_output.p
-00006a30: 6c61 796c 6973 745b 7365 6c65 6374 6564  laylist[selected
-00006a40: 5f73 6f6e 675d 0a0a 2020 2020 2020 2020  _song]..        
-00006a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a60: 2020 2020 2020 2020 2020 2020 6966 206c              if l
-00006a70: 6f6f 703a 0a20 2020 2020 2020 2020 2020  oop:.           
-00006a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a90: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00006aa0: 7265 7368 7566 666c 653a 0a20 2020 2020  reshuffle:.     
-00006ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006970: 2020 2020 2020 2020 2020 2020 6272 6561              brea
+00006980: 6b0a 2020 2020 2020 2020 2020 2020 2020  k.              
+00006990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000069a0: 2020 656c 6966 2063 2069 6e20 225c 625c    elif c in "\b\
+000069b0: 7837 6622 3a0a 2020 2020 2020 2020 2020  x7f":.          
+000069c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000069d0: 2020 2020 2020 2020 2020 7365 6c65 6374            select
+000069e0: 6564 5f73 6f6e 6720 3d20 706c 6179 6572  ed_song = player
+000069f0: 5f6f 7574 7075 742e 7363 726f 6c6c 6572  _output.scroller
+00006a00: 2e70 6f73 0a20 2020 2020 2020 2020 2020  .pos.           
+00006a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a20: 2020 2020 2020 2020 2064 656c 2070 6c61           del pla
+00006a30: 7965 725f 6f75 7470 7574 2e70 6c61 796c  yer_output.playl
+00006a40: 6973 745b 7365 6c65 6374 6564 5f73 6f6e  ist[selected_son
+00006a50: 675d 0a0a 2020 2020 2020 2020 2020 2020  g]..            
+00006a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a70: 2020 2020 2020 2020 6966 206c 6f6f 703a          if loop:
+00006a80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006aa0: 2020 2020 2020 2020 2069 6620 7265 7368           if resh
+00006ab0: 7566 666c 653a 0a20 2020 2020 2020 2020  uffle:.         
 00006ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ad0: 2020 2020 2020 206e 6578 745f 706c 6179         next_play
-00006ae0: 6c69 7374 203d 2070 6c61 796c 6973 745b  list = playlist[
-00006af0: 3a5d 0a20 2020 2020 2020 2020 2020 2020  :].             
+00006ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ae0: 2020 206e 6578 745f 706c 6179 6c69 7374     next_playlist
+00006af0: 203d 2070 6c61 796c 6973 745b 3a5d 0a20   = playlist[:]. 
 00006b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b10: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00006b20: 6875 6666 6c65 286e 6578 745f 706c 6179  huffle(next_play
-00006b30: 6c69 7374 290a 2020 2020 2020 2020 2020  list).          
-00006b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b50: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00006b60: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00006b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b20: 2020 2020 2020 2020 2020 2073 6875 6666             shuff
+00006b30: 6c65 286e 6578 745f 706c 6179 6c69 7374  le(next_playlist
+00006b40: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00006b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b60: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
 00006b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b90: 6465 6c20 6e65 7874 5f70 6c61 796c 6973  del next_playlis
-00006ba0: 745b 7365 6c65 6374 6564 5f73 6f6e 675d  t[selected_song]
-00006bb0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00006b90: 2020 2020 2020 2020 2020 2020 6465 6c20              del 
+00006ba0: 6e65 7874 5f70 6c61 796c 6973 745b 7365  next_playlist[se
+00006bb0: 6c65 6374 6564 5f73 6f6e 675d 0a0a 2020  lected_song]..  
 00006bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006bd0: 2020 2020 2020 706c 6179 6572 5f6f 7574        player_out
-00006be0: 7075 742e 7363 726f 6c6c 6572 2e6e 756d  put.scroller.num
-00006bf0: 5f6c 696e 6573 202d 3d20 310a 2020 2020  _lines -= 1.    
-00006c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006be0: 2020 706c 6179 6572 5f6f 7574 7075 742e    player_output.
+00006bf0: 7363 726f 6c6c 6572 2e6e 756d 5f6c 696e  scroller.num_lin
+00006c00: 6573 202d 3d20 310a 2020 2020 2020 2020  es -= 1.        
 00006c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c20: 6966 2028 0a20 2020 2020 2020 2020 2020  if (.           
-00006c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c40: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00006c50: 6563 7465 645f 736f 6e67 203d 3d20 706c  ected_song == pl
-00006c60: 6179 6572 5f6f 7574 7075 742e 690a 2020  ayer_output.i.  
-00006c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c20: 2020 2020 2020 2020 2020 2020 6966 2028              if (
+00006c30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c50: 2020 2020 2020 2020 2073 656c 6563 7465           selecte
+00006c60: 645f 736f 6e67 203d 3d20 706c 6179 6572  d_song == player
+00006c70: 5f6f 7574 7075 742e 690a 2020 2020 2020  _output.i.      
 00006c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c90: 2020 293a 2020 2320 6465 6c65 7465 6420    ):  # deleted 
-00006ca0: 6375 7272 656e 7420 736f 6e67 0a20 2020  current song.   
-00006cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c90: 2020 2020 2020 2020 2020 2020 2020 293a                ):
+00006ca0: 2020 2320 6465 6c65 7465 6420 6375 7272    # deleted curr
+00006cb0: 656e 7420 736f 6e67 0a20 2020 2020 2020  ent song.       
 00006cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006cd0: 2020 2020 206e 6578 745f 736f 6e67 203d       next_song =
-00006ce0: 2031 0a20 2020 2020 2020 2020 2020 2020   1.             
+00006cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ce0: 206e 6578 745f 736f 6e67 203d 2031 0a20   next_song = 1. 
 00006cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d00: 2020 2020 2020 2020 2020 2023 2077 696c             # wil
-00006d10: 6c20 6265 2069 6e63 7265 6d65 6e74 6564  l be incremented
-00006d20: 2074 6f20 690a 2020 2020 2020 2020 2020   to i.          
-00006d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d40: 2020 2020 2020 2020 2020 2020 2020 706c                pl
-00006d50: 6179 6572 5f6f 7574 7075 742e 7363 726f  ayer_output.scro
-00006d60: 6c6c 6572 2e70 6f73 203d 2028 0a20 2020  ller.pos = (.   
-00006d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d10: 2020 2020 2020 2023 2077 696c 6c20 6265         # will be
+00006d20: 2069 6e63 7265 6d65 6e74 6564 2074 6f20   incremented to 
+00006d30: 690a 2020 2020 2020 2020 2020 2020 2020  i.              
+00006d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d50: 2020 2020 2020 2020 2020 706c 6179 6572            player
+00006d60: 5f6f 7574 7075 742e 7363 726f 6c6c 6572  _output.scroller
+00006d70: 2e70 6f73 203d 2028 0a20 2020 2020 2020  .pos = (.       
 00006d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d90: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
-00006da0: 6f75 7470 7574 2e69 202d 2031 0a20 2020  output.i - 1.   
-00006db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006da0: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
+00006db0: 7574 2e69 202d 2031 0a20 2020 2020 2020  ut.i - 1.       
 00006dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006dd0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00006de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006df0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00006e00: 6c61 7965 725f 6f75 7470 7574 2e69 202d  layer_output.i -
-00006e10: 3d20 310a 2020 2020 2020 2020 2020 2020  = 1.            
+00006dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006de0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+00006df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006e00: 2020 2020 2020 2020 2020 2070 6c61 7965             playe
+00006e10: 725f 6f75 7470 7574 2e69 202d 3d20 310a  r_output.i -= 1.
 00006e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e30: 2020 2020 2020 2020 2020 2020 706c 6179              play
-00006e40: 6261 636b 2e73 746f 7028 290a 2020 2020  back.stop().    
-00006e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006e40: 2020 2020 2020 2020 706c 6179 6261 636b          playback
+00006e50: 2e73 746f 7028 290a 2020 2020 2020 2020  .stop().        
 00006e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e70: 2020 2020 6272 6561 6b0a 2020 2020 2020      break.      
-00006e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e90: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00006ea0: 6465 6c65 7465 6420 736f 6e67 2062 6566  deleted song bef
-00006eb0: 6f72 6520 6375 7272 656e 740a 2020 2020  ore current.    
-00006ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006e80: 6272 6561 6b0a 2020 2020 2020 2020 2020  break.          
+00006e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ea0: 2020 2020 2020 2020 2020 2320 6465 6c65            # dele
+00006eb0: 7465 6420 736f 6e67 2062 6566 6f72 6520  ted song before 
+00006ec0: 6375 7272 656e 740a 2020 2020 2020 2020  current.        
 00006ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ee0: 6966 2073 656c 6563 7465 645f 736f 6e67  if selected_song
-00006ef0: 203c 2070 6c61 7965 725f 6f75 7470 7574   < player_output
-00006f00: 2e69 3a0a 2020 2020 2020 2020 2020 2020  .i:.            
+00006ee0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00006ef0: 656c 6563 7465 645f 736f 6e67 203c 2070  elected_song < p
+00006f00: 6c61 7965 725f 6f75 7470 7574 2e69 3a0a  layer_output.i:.
 00006f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f20: 2020 2020 2020 2020 2020 2020 706c 6179              play
-00006f30: 6572 5f6f 7574 7075 742e 6920 2d3d 2031  er_output.i -= 1
-00006f40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006f50: 2020 2020 2020 2020 2020 2020 2065 7863               exc
-00006f60: 6570 7420 2856 616c 7565 4572 726f 722c  ept (ValueError,
-00006f70: 204f 7665 7266 6c6f 7745 7272 6f72 293a   OverflowError):
-00006f80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f30: 2020 2020 2020 2020 706c 6179 6572 5f6f          player_o
+00006f40: 7574 7075 742e 6920 2d3d 2031 0a20 2020  utput.i -= 1.   
+00006f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f60: 2020 2020 2020 2020 2065 7863 6570 7420           except 
+00006f70: 2856 616c 7565 4572 726f 722c 204f 7665  (ValueError, Ove
+00006f80: 7266 6c6f 7745 7272 6f72 293a 0a20 2020  rflowError):.   
 00006f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006fa0: 2070 6173 730a 2020 2020 2020 2020 2020   pass.          
-00006fb0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00006fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006fd0: 2020 2020 2020 2020 6966 2063 203d 3d20          if c == 
-00006fe0: 6375 7273 6573 2e4b 4559 5f4c 4546 543a  curses.KEY_LEFT:
-00006ff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007000: 2020 2020 2020 2020 2020 2020 2023 2070               # p
-00007010: 796c 696e 743a 2064 6973 6162 6c65 3d75  ylint: disable=u
-00007020: 6e73 7562 7363 7269 7074 6162 6c65 2d6f  nsubscriptable-o
-00007030: 626a 6563 740a 2020 2020 2020 2020 2020  bject.          
-00007040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007050: 2020 706c 6179 6572 5f6f 7574 7075 742e    player_output.
-00007060: 7072 6f6d 7074 696e 6720 3d20 280a 2020  prompting = (.  
-00007070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007080: 2020 2020 2020 2020 2020 2020 2020 706c                pl
-00007090: 6179 6572 5f6f 7574 7075 742e 7072 6f6d  ayer_output.prom
-000070a0: 7074 696e 675b 305d 2c0a 2020 2020 2020  pting[0],.      
-000070b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070c0: 2020 2020 2020 2020 2020 6d61 7828 706c            max(pl
-000070d0: 6179 6572 5f6f 7574 7075 742e 7072 6f6d  ayer_output.prom
-000070e0: 7074 696e 675b 315d 202d 2031 2c20 3029  pting[1] - 1, 0)
-000070f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00006fa0: 2020 2020 2020 2020 2020 2020 2070 6173               pas
+00006fb0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+00006fc0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00006fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006fe0: 2020 2020 6966 2063 203d 3d20 6375 7273      if c == curs
+00006ff0: 6573 2e4b 4559 5f4c 4546 543a 0a20 2020  es.KEY_LEFT:.   
+00007000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007010: 2020 2020 2020 2020 2023 2070 796c 696e           # pylin
+00007020: 743a 2064 6973 6162 6c65 3d75 6e73 7562  t: disable=unsub
+00007030: 7363 7269 7074 6162 6c65 2d6f 626a 6563  scriptable-objec
+00007040: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
+00007050: 2020 2020 2020 2020 2020 2020 2020 706c                pl
+00007060: 6179 6572 5f6f 7574 7075 742e 7072 6f6d  ayer_output.prom
+00007070: 7074 696e 6720 3d20 280a 2020 2020 2020  pting = (.      
+00007080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007090: 2020 2020 2020 2020 2020 706c 6179 6572            player
+000070a0: 5f6f 7574 7075 742e 7072 6f6d 7074 696e  _output.promptin
+000070b0: 675b 305d 2c0a 2020 2020 2020 2020 2020  g[0],.          
+000070c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000070d0: 2020 2020 2020 6d61 7828 706c 6179 6572        max(player
+000070e0: 5f6f 7574 7075 742e 7072 6f6d 7074 696e  _output.promptin
+000070f0: 675b 315d 202d 2031 2c20 3029 2c0a 2020  g[1] - 1, 0),.  
 00007100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007110: 2020 706c 6179 6572 5f6f 7574 7075 742e    player_output.
-00007120: 7072 6f6d 7074 696e 675b 325d 2c0a 2020  prompting[2],.  
-00007130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007140: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00007150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007160: 2020 2020 2020 2020 706c 6179 6572 5f6f          player_o
-00007170: 7574 7075 742e 6f75 7470 7574 2870 6c61  utput.output(pla
-00007180: 7962 6163 6b2e 6375 7272 5f70 6f73 290a  yback.curr_pos).
-00007190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000071a0: 2020 2020 2020 2020 656c 6966 2063 203d          elif c =
-000071b0: 3d20 6375 7273 6573 2e4b 4559 5f52 4947  = curses.KEY_RIG
-000071c0: 4854 3a0a 2020 2020 2020 2020 2020 2020  HT:.            
+00007110: 2020 2020 2020 2020 2020 2020 2020 706c                pl
+00007120: 6179 6572 5f6f 7574 7075 742e 7072 6f6d  ayer_output.prom
+00007130: 7074 696e 675b 325d 2c0a 2020 2020 2020  pting[2],.      
+00007140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007150: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00007160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007170: 2020 2020 706c 6179 6572 5f6f 7574 7075      player_outpu
+00007180: 742e 6f75 7470 7574 2870 6c61 7962 6163  t.output(playbac
+00007190: 6b2e 6375 7272 5f70 6f73 290a 2020 2020  k.curr_pos).    
+000071a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000071b0: 2020 2020 656c 6966 2063 203d 3d20 6375      elif c == cu
+000071c0: 7273 6573 2e4b 4559 5f52 4947 4854 3a0a  rses.KEY_RIGHT:.
 000071d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000071e0: 2320 7079 6c69 6e74 3a20 6469 7361 626c  # pylint: disabl
-000071f0: 653d 756e 7375 6273 6372 6970 7461 626c  e=unsubscriptabl
-00007200: 652d 6f62 6a65 6374 0a20 2020 2020 2020  e-object.       
-00007210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007220: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
-00007230: 7574 2e70 726f 6d70 7469 6e67 203d 2028  ut.prompting = (
-00007240: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000071e0: 2020 2020 2020 2020 2020 2020 2320 7079              # py
+000071f0: 6c69 6e74 3a20 6469 7361 626c 653d 756e  lint: disable=un
+00007200: 7375 6273 6372 6970 7461 626c 652d 6f62  subscriptable-ob
+00007210: 6a65 6374 0a20 2020 2020 2020 2020 2020  ject.           
+00007220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007230: 2070 6c61 7965 725f 6f75 7470 7574 2e70   player_output.p
+00007240: 726f 6d70 7469 6e67 203d 2028 0a20 2020  rompting = (.   
 00007250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007260: 2070 6c61 7965 725f 6f75 7470 7574 2e70   player_output.p
-00007270: 726f 6d70 7469 6e67 5b30 5d2c 0a20 2020  rompting[0],.   
-00007280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007290: 2020 2020 2020 2020 2020 2020 206d 696e               min
-000072a0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00007260: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
+00007270: 7965 725f 6f75 7470 7574 2e70 726f 6d70  yer_output.promp
+00007280: 7469 6e67 5b30 5d2c 0a20 2020 2020 2020  ting[0],.       
+00007290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000072a0: 2020 2020 2020 2020 206d 696e 280a 2020           min(.  
 000072b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000072c0: 2020 2020 2020 706c 6179 6572 5f6f 7574        player_out
-000072d0: 7075 742e 7072 6f6d 7074 696e 675b 315d  put.prompting[1]
-000072e0: 202b 2031 2c0a 2020 2020 2020 2020 2020   + 1,.          
-000072f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007300: 2020 2020 2020 2020 2020 6c65 6e28 706c            len(pl
-00007310: 6179 6572 5f6f 7574 7075 742e 7072 6f6d  ayer_output.prom
-00007320: 7074 696e 675b 305d 292c 0a20 2020 2020  pting[0]),.     
-00007330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007340: 2020 2020 2020 2020 2020 2029 2c0a 2020             ),.  
-00007350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007360: 2020 2020 2020 2020 2020 2020 2020 706c                pl
-00007370: 6179 6572 5f6f 7574 7075 742e 7072 6f6d  ayer_output.prom
-00007380: 7074 696e 675b 325d 2c0a 2020 2020 2020  pting[2],.      
-00007390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000073a0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-000073b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000073c0: 2020 2020 706c 6179 6572 5f6f 7574 7075      player_outpu
-000073d0: 742e 6f75 7470 7574 2870 6c61 7962 6163  t.output(playbac
-000073e0: 6b2e 6375 7272 5f70 6f73 290a 2020 2020  k.curr_pos).    
-000073f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007400: 2020 2020 656c 6966 2063 203d 3d20 6375      elif c == cu
-00007410: 7273 6573 2e4b 4559 5f55 503a 0a20 2020  rses.KEY_UP:.   
-00007420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007430: 2020 2020 2020 2020 2069 6620 706c 6179           if play
-00007440: 6572 5f6f 7574 7075 742e 7363 726f 6c6c  er_output.scroll
-00007450: 6572 2e70 6f73 2021 3d20 303a 0a20 2020  er.pos != 0:.   
-00007460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007470: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
-00007480: 7965 725f 6f75 7470 7574 2e73 6372 6f6c  yer_output.scrol
-00007490: 6c65 722e 7363 726f 6c6c 5f62 6163 6b77  ler.scroll_backw
-000074a0: 6172 6428 290a 2020 2020 2020 2020 2020  ard().          
-000074b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000074c0: 2020 2020 2020 706c 6179 6572 5f6f 7574        player_out
-000074d0: 7075 742e 6f75 7470 7574 2870 6c61 7962  put.output(playb
-000074e0: 6163 6b2e 6375 7272 5f70 6f73 290a 2020  ack.curr_pos).  
-000074f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007500: 2020 2020 2020 656c 6966 2063 203d 3d20        elif c == 
-00007510: 6375 7273 6573 2e4b 4559 5f44 4f57 4e3a  curses.KEY_DOWN:
-00007520: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007530: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00007540: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000072c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000072d0: 2020 706c 6179 6572 5f6f 7574 7075 742e    player_output.
+000072e0: 7072 6f6d 7074 696e 675b 315d 202b 2031  prompting[1] + 1
+000072f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00007300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007310: 2020 2020 2020 6c65 6e28 706c 6179 6572        len(player
+00007320: 5f6f 7574 7075 742e 7072 6f6d 7074 696e  _output.promptin
+00007330: 675b 305d 292c 0a20 2020 2020 2020 2020  g[0]),.         
+00007340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007350: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
+00007360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007370: 2020 2020 2020 2020 2020 706c 6179 6572            player
+00007380: 5f6f 7574 7075 742e 7072 6f6d 7074 696e  _output.promptin
+00007390: 675b 325d 2c0a 2020 2020 2020 2020 2020  g[2],.          
+000073a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000073b0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+000073c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000073d0: 706c 6179 6572 5f6f 7574 7075 742e 6f75  player_output.ou
+000073e0: 7470 7574 2870 6c61 7962 6163 6b2e 6375  tput(playback.cu
+000073f0: 7272 5f70 6f73 290a 2020 2020 2020 2020  rr_pos).        
+00007400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007410: 656c 6966 2063 203d 3d20 6375 7273 6573  elif c == curses
+00007420: 2e4b 4559 5f55 503a 0a20 2020 2020 2020  .KEY_UP:.       
+00007430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007440: 2020 2020 2069 6620 706c 6179 6572 5f6f       if player_o
+00007450: 7574 7075 742e 7363 726f 6c6c 6572 2e70  utput.scroller.p
+00007460: 6f73 2021 3d20 303a 0a20 2020 2020 2020  os != 0:.       
+00007470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007480: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
+00007490: 6f75 7470 7574 2e73 6372 6f6c 6c65 722e  output.scroller.
+000074a0: 7363 726f 6c6c 5f62 6163 6b77 6172 6428  scroll_backward(
+000074b0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000074c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000074d0: 2020 706c 6179 6572 5f6f 7574 7075 742e    player_output.
+000074e0: 6f75 7470 7574 2870 6c61 7962 6163 6b2e  output(playback.
+000074f0: 6375 7272 5f70 6f73 290a 2020 2020 2020  curr_pos).      
+00007500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007510: 2020 656c 6966 2063 203d 3d20 6375 7273    elif c == curs
+00007520: 6573 2e4b 4559 5f44 4f57 4e3a 0a20 2020  es.KEY_DOWN:.   
+00007530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007540: 2020 2020 2020 2020 2069 6620 280a 2020           if (.  
 00007550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007560: 2020 706c 6179 6572 5f6f 7574 7075 742e    player_output.
-00007570: 7363 726f 6c6c 6572 2e70 6f73 0a20 2020  scroller.pos.   
-00007580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007590: 2020 2020 2020 2020 2020 2020 2021 3d20               != 
-000075a0: 706c 6179 6572 5f6f 7574 7075 742e 7363  player_output.sc
-000075b0: 726f 6c6c 6572 2e6e 756d 5f6c 696e 6573  roller.num_lines
-000075c0: 202d 2031 0a20 2020 2020 2020 2020 2020   - 1.           
-000075d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000075e0: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
+00007560: 2020 2020 2020 2020 2020 2020 2020 706c                pl
+00007570: 6179 6572 5f6f 7574 7075 742e 7363 726f  ayer_output.scro
+00007580: 6c6c 6572 2e70 6f73 0a20 2020 2020 2020  ller.pos.       
+00007590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000075a0: 2020 2020 2020 2020 2021 3d20 706c 6179           != play
+000075b0: 6572 5f6f 7574 7075 742e 7363 726f 6c6c  er_output.scroll
+000075c0: 6572 2e6e 756d 5f6c 696e 6573 202d 2031  er.num_lines - 1
+000075d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000075e0: 2020 2020 2020 2020 2020 2020 2029 3a0a               ):.
 000075f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007600: 2020 2020 706c 6179 6572 5f6f 7574 7075      player_outpu
-00007610: 742e 7363 726f 6c6c 6572 2e73 6372 6f6c  t.scroller.scrol
-00007620: 6c5f 666f 7277 6172 6428 290a 2020 2020  l_forward().    
-00007630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007640: 2020 2020 2020 2020 2020 2020 706c 6179              play
-00007650: 6572 5f6f 7574 7075 742e 6f75 7470 7574  er_output.output
-00007660: 2870 6c61 7962 6163 6b2e 6375 7272 5f70  (playback.curr_p
-00007670: 6f73 290a 2020 2020 2020 2020 2020 2020  os).            
-00007680: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-00007690: 2063 203d 3d20 6375 7273 6573 2e4b 4559   c == curses.KEY
-000076a0: 5f44 433a 0a20 2020 2020 2020 2020 2020  _DC:.           
-000076b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000076c0: 2023 2070 796c 696e 743a 2064 6973 6162   # pylint: disab
-000076d0: 6c65 3d75 6e73 7562 7363 7269 7074 6162  le=unsubscriptab
-000076e0: 6c65 2d6f 626a 6563 740a 2020 2020 2020  le-object.      
-000076f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007700: 2020 2020 2020 6966 2070 6c61 7965 725f        if player_
-00007710: 6f75 7470 7574 2e70 726f 6d70 7469 6e67  output.prompting
-00007720: 5b31 5d20 3e20 303a 0a20 2020 2020 2020  [1] > 0:.       
-00007730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007740: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
-00007750: 6f75 7470 7574 2e70 726f 6d70 7469 6e67  output.prompting
-00007760: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
-00007770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007780: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
-00007790: 6f75 7470 7574 2e70 726f 6d70 7469 6e67  output.prompting
-000077a0: 5b30 5d5b 0a20 2020 2020 2020 2020 2020  [0][.           
-000077b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000077c0: 2020 2020 2020 2020 2020 2020 203a 2070               : p
-000077d0: 6c61 7965 725f 6f75 7470 7574 2e70 726f  layer_output.pro
-000077e0: 6d70 7469 6e67 5b31 5d20 2d20 310a 2020  mpting[1] - 1.  
-000077f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007610: 706c 6179 6572 5f6f 7574 7075 742e 7363  player_output.sc
+00007620: 726f 6c6c 6572 2e73 6372 6f6c 6c5f 666f  roller.scroll_fo
+00007630: 7277 6172 6428 290a 2020 2020 2020 2020  rward().        
+00007640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007650: 2020 2020 2020 2020 706c 6179 6572 5f6f          player_o
+00007660: 7574 7075 742e 6f75 7470 7574 2870 6c61  utput.output(pla
+00007670: 7962 6163 6b2e 6375 7272 5f70 6f73 290a  yback.curr_pos).
+00007680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007690: 2020 2020 2020 2020 656c 6966 2063 203d          elif c =
+000076a0: 3d20 6375 7273 6573 2e4b 4559 5f44 433a  = curses.KEY_DC:
+000076b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000076c0: 2020 2020 2020 2020 2020 2020 2023 2070               # p
+000076d0: 796c 696e 743a 2064 6973 6162 6c65 3d75  ylint: disable=u
+000076e0: 6e73 7562 7363 7269 7074 6162 6c65 2d6f  nsubscriptable-o
+000076f0: 626a 6563 740a 2020 2020 2020 2020 2020  bject.          
+00007700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007710: 2020 6966 2070 6c61 7965 725f 6f75 7470    if player_outp
+00007720: 7574 2e70 726f 6d70 7469 6e67 5b31 5d20  ut.prompting[1] 
+00007730: 3e20 303a 0a20 2020 2020 2020 2020 2020  > 0:.           
+00007740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007750: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
+00007760: 7574 2e70 726f 6d70 7469 6e67 203d 2028  ut.prompting = (
+00007770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007790: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
+000077a0: 7574 2e70 726f 6d70 7469 6e67 5b30 5d5b  ut.prompting[0][
+000077b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000077c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000077d0: 2020 2020 2020 2020 203a 2070 6c61 7965           : playe
+000077e0: 725f 6f75 7470 7574 2e70 726f 6d70 7469  r_output.prompti
+000077f0: 6e67 5b31 5d20 2d20 310a 2020 2020 2020  ng[1] - 1.      
 00007800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007810: 2020 5d0a 2020 2020 2020 2020 2020 2020    ].            
+00007810: 2020 2020 2020 2020 2020 2020 2020 5d0a                ].
 00007820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007830: 2020 2020 2020 2020 2b20 706c 6179 6572          + player
-00007840: 5f6f 7574 7075 742e 7072 6f6d 7074 696e  _output.promptin
-00007850: 675b 305d 5b0a 2020 2020 2020 2020 2020  g[0][.          
-00007860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007870: 2020 2020 2020 2020 2020 2020 2020 706c                pl
-00007880: 6179 6572 5f6f 7574 7075 742e 7072 6f6d  ayer_output.prom
-00007890: 7074 696e 675b 315d 203a 0a20 2020 2020  pting[1] :.     
-000078a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078b0: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
-000078c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00007830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007840: 2020 2020 2b20 706c 6179 6572 5f6f 7574      + player_out
+00007850: 7075 742e 7072 6f6d 7074 696e 675b 305d  put.prompting[0]
+00007860: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
+00007870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007880: 2020 2020 2020 2020 2020 706c 6179 6572            player
+00007890: 5f6f 7574 7075 742e 7072 6f6d 7074 696e  _output.promptin
+000078a0: 675b 315d 203a 0a20 2020 2020 2020 2020  g[1] :.         
+000078b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000078c0: 2020 2020 2020 2020 2020 205d 2c0a 2020             ],.  
 000078d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078e0: 2020 2020 2020 706c 6179 6572 5f6f 7574        player_out
-000078f0: 7075 742e 7072 6f6d 7074 696e 675b 315d  put.prompting[1]
-00007900: 202d 2031 2c0a 2020 2020 2020 2020 2020   - 1,.          
-00007910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007920: 2020 2020 2020 2020 2020 706c 6179 6572            player
-00007930: 5f6f 7574 7075 742e 7072 6f6d 7074 696e  _output.promptin
-00007940: 675b 325d 2c0a 2020 2020 2020 2020 2020  g[2],.          
-00007950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007960: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00007970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007980: 2020 2020 706c 6179 6572 5f6f 7574 7075      player_outpu
-00007990: 742e 6f75 7470 7574 2870 6c61 7962 6163  t.output(playbac
-000079a0: 6b2e 6375 7272 5f70 6f73 290a 2020 2020  k.curr_pos).    
-000079b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000079c0: 2020 2020 656c 6966 2063 203d 3d20 6375      elif c == cu
-000079d0: 7273 6573 2e4b 4559 5f45 4e54 4552 3a0a  rses.KEY_ENTER:.
-000079e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000079f0: 2020 2020 2020 2020 2020 2020 2320 7079              # py
-00007a00: 6c69 6e74 3a20 6469 7361 626c 653d 756e  lint: disable=un
-00007a10: 7375 6273 6372 6970 7461 626c 652d 6f62  subscriptable-ob
-00007a20: 6a65 6374 0a20 2020 2020 2020 2020 2020  ject.           
-00007a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a40: 2069 6620 706c 6179 6572 5f6f 7574 7075   if player_outpu
-00007a50: 742e 7072 6f6d 7074 696e 675b 0a20 2020  t.prompting[.   
-00007a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a70: 2020 2020 2020 2020 2020 2020 2030 0a20               0. 
-00007a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a90: 2020 2020 2020 2020 2020 205d 2e69 736e             ].isn
-00007aa0: 756d 6572 6963 2829 2061 6e64 2070 6c61  umeric() and pla
-00007ab0: 7965 725f 6f75 7470 7574 2e70 726f 6d70  yer_output.promp
-00007ac0: 7469 6e67 5b32 5d20 696e 2028 0a20 2020  ting[2] in (.   
-00007ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ae0: 2020 2020 2020 2020 2020 2020 2050 524f               PRO
-00007af0: 4d50 545f 4d4f 4445 535b 2261 6464 225d  MPT_MODES["add"]
-00007b00: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000078e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000078f0: 2020 706c 6179 6572 5f6f 7574 7075 742e    player_output.
+00007900: 7072 6f6d 7074 696e 675b 315d 202d 2031  prompting[1] - 1
+00007910: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00007920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007930: 2020 2020 2020 706c 6179 6572 5f6f 7574        player_out
+00007940: 7075 742e 7072 6f6d 7074 696e 675b 325d  put.prompting[2]
+00007950: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00007960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007970: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00007980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007990: 706c 6179 6572 5f6f 7574 7075 742e 6f75  player_output.ou
+000079a0: 7470 7574 2870 6c61 7962 6163 6b2e 6375  tput(playback.cu
+000079b0: 7272 5f70 6f73 290a 2020 2020 2020 2020  rr_pos).        
+000079c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000079d0: 656c 6966 2063 203d 3d20 6375 7273 6573  elif c == curses
+000079e0: 2e4b 4559 5f45 4e54 4552 3a0a 2020 2020  .KEY_ENTER:.    
+000079f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a00: 2020 2020 2020 2020 2320 7079 6c69 6e74          # pylint
+00007a10: 3a20 6469 7361 626c 653d 756e 7375 6273  : disable=unsubs
+00007a20: 6372 6970 7461 626c 652d 6f62 6a65 6374  criptable-object
+00007a30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007a40: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00007a50: 706c 6179 6572 5f6f 7574 7075 742e 7072  player_output.pr
+00007a60: 6f6d 7074 696e 675b 0a20 2020 2020 2020  ompting[.       
+00007a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a80: 2020 2020 2020 2020 2030 0a20 2020 2020           0.     
+00007a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007aa0: 2020 2020 2020 205d 2e69 736e 756d 6572         ].isnumer
+00007ab0: 6963 2829 2061 6e64 2070 6c61 7965 725f  ic() and player_
+00007ac0: 6f75 7470 7574 2e70 726f 6d70 7469 6e67  output.prompting
+00007ad0: 5b32 5d20 696e 2028 0a20 2020 2020 2020  [2] in (.       
+00007ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007af0: 2020 2020 2020 2020 2050 524f 4d50 545f           PROMPT_
+00007b00: 4d4f 4445 535b 2261 6464 225d 2c0a 2020  MODES["add"],.  
 00007b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b20: 2020 5052 4f4d 5054 5f4d 4f44 4553 5b22    PROMPT_MODES["
-00007b30: 696e 7365 7274 225d 2c0a 2020 2020 2020  insert"],.      
-00007b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b50: 2020 2020 2020 293a 0a20 2020 2020 2020        ):.       
-00007b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b70: 2020 2020 2020 2020 2066 6f72 2064 6574           for det
-00007b80: 6169 6c73 2069 6e20 706c 6179 6572 5f6f  ails in player_o
-00007b90: 7574 7075 742e 706c 6179 6c69 7374 3a0a  utput.playlist:.
-00007ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b20: 2020 2020 2020 2020 2020 2020 2020 5052                PR
+00007b30: 4f4d 5054 5f4d 4f44 4553 5b22 696e 7365  OMPT_MODES["inse
+00007b40: 7274 225d 2c0a 2020 2020 2020 2020 2020  rt"],.          
+00007b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b60: 2020 293a 0a20 2020 2020 2020 2020 2020    ):.           
+00007b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b80: 2020 2020 2066 6f72 2064 6574 6169 6c73       for details
+00007b90: 2069 6e20 706c 6179 6572 5f6f 7574 7075   in player_outpu
+00007ba0: 742e 706c 6179 6c69 7374 3a0a 2020 2020  t.playlist:.    
 00007bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007bc0: 2020 2020 6966 2069 6e74 2864 6574 6169      if int(detai
-00007bd0: 6c73 5b30 5d29 203d 3d20 696e 7428 0a20  ls[0]) == int(. 
-00007be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007bd0: 6966 2069 6e74 2864 6574 6169 6c73 5b30  if int(details[0
+00007be0: 5d29 203d 3d20 696e 7428 0a20 2020 2020  ]) == int(.     
 00007bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c00: 2020 2020 2020 2070 6c61 7965 725f 6f75         player_ou
-00007c10: 7470 7574 2e70 726f 6d70 7469 6e67 5b30  tput.prompting[0
-00007c20: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00007c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c10: 2020 2070 6c61 7965 725f 6f75 7470 7574     player_output
+00007c20: 2e70 726f 6d70 7469 6e67 5b30 5d0a 2020  .prompting[0].  
 00007c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c40: 2020 2020 2020 293a 0a20 2020 2020 2020        ):.       
-00007c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c50: 2020 293a 0a20 2020 2020 2020 2020 2020    ):.           
 00007c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c70: 2062 7265 616b 0a20 2020 2020 2020 2020   break.         
-00007c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c90: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00007ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c70: 2020 2020 2020 2020 2020 2020 2062 7265               bre
+00007c80: 616b 0a20 2020 2020 2020 2020 2020 2020  ak.             
+00007c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ca0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
 00007cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007cc0: 2077 6974 6820 6f70 656e 280a 2020 2020   with open(.    
-00007cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007cc0: 2020 2020 2020 2020 2020 2020 2077 6974               wit
+00007cd0: 6820 6f70 656e 280a 2020 2020 2020 2020  h open(.        
 00007ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007cf0: 2020 2020 534f 4e47 535f 494e 464f 5f50      SONGS_INFO_P
-00007d00: 4154 482c 0a20 2020 2020 2020 2020 2020  ATH,.           
-00007d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d20: 2020 2020 2020 2020 2020 2020 2022 7222               "r"
-00007d30: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00007cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d00: 534f 4e47 535f 494e 464f 5f50 4154 482c  SONGS_INFO_PATH,
+00007d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d30: 2020 2020 2020 2020 2022 7222 2c0a 2020           "r",.  
 00007d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d50: 2020 2020 2020 2020 2020 656e 636f 6469            encodi
-00007d60: 6e67 3d22 7574 662d 3822 2c0a 2020 2020  ng="utf-8",.    
-00007d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d60: 2020 2020 2020 656e 636f 6469 6e67 3d22        encoding="
+00007d70: 7574 662d 3822 2c0a 2020 2020 2020 2020  utf-8",.        
 00007d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d90: 2920 6173 2073 6f6e 6773 5f66 696c 653a  ) as songs_file:
-00007da0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007d90: 2020 2020 2020 2020 2020 2020 2920 6173              ) as
+00007da0: 2073 6f6e 6773 5f66 696c 653a 0a20 2020   songs_file:.   
 00007db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007dc0: 2020 2020 2020 2020 2066 6f72 206c 696e           for lin
-00007dd0: 6520 696e 2073 6f6e 6773 5f66 696c 653a  e in songs_file:
-00007de0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007dd0: 2020 2020 2066 6f72 206c 696e 6520 696e       for line in
+00007de0: 2073 6f6e 6773 5f66 696c 653a 0a20 2020   songs_file:.   
 00007df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e00: 2020 2020 2020 2020 2020 2020 2064 6574               det
-00007e10: 6169 6c73 203d 206c 696e 652e 7374 7269  ails = line.stri
-00007e20: 7028 292e 7370 6c69 7428 227c 2229 0a20  p().split("|"). 
-00007e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007e10: 2020 2020 2020 2020 2064 6574 6169 6c73           details
+00007e20: 203d 206c 696e 652e 7374 7269 7028 292e   = line.strip().
+00007e30: 7370 6c69 7428 227c 2229 0a20 2020 2020  split("|").     
 00007e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e50: 2020 2020 2020 2020 2020 2073 6f6e 675f             song_
-00007e60: 6964 203d 2069 6e74 2864 6574 6169 6c73  id = int(details
-00007e70: 5b30 5d29 0a20 2020 2020 2020 2020 2020  [0]).           
-00007e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007e60: 2020 2020 2020 2073 6f6e 675f 6964 203d         song_id =
+00007e70: 2069 6e74 2864 6574 6169 6c73 5b30 5d29   int(details[0])
+00007e80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00007e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ea0: 2069 6620 736f 6e67 5f69 6420 3d3d 2069   if song_id == i
-00007eb0: 6e74 280a 2020 2020 2020 2020 2020 2020  nt(.            
+00007ea0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00007eb0: 736f 6e67 5f69 6420 3d3d 2069 6e74 280a  song_id == int(.
 00007ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ee0: 2020 2020 706c 6179 6572 5f6f 7574 7075      player_outpu
-00007ef0: 742e 7072 6f6d 7074 696e 675b 305d 0a20  t.prompting[0]. 
-00007f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ef0: 706c 6179 6572 5f6f 7574 7075 742e 7072  player_output.pr
+00007f00: 6f6d 7074 696e 675b 305d 0a20 2020 2020  ompting[0].     
 00007f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f20: 2020 2020 2020 2020 2020 2029 3a0a 2020             ):.  
-00007f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f30: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
 00007f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f50: 2020 2020 2020 2020 2020 2020 2020 736f                so
-00007f60: 6e67 5f64 6174 6120 3d20 6d75 7369 635f  ng_data = music_
-00007f70: 7461 672e 6c6f 6164 5f66 696c 6528 0a20  tag.load_file(. 
-00007f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f60: 2020 2020 2020 2020 2020 736f 6e67 5f64            song_d
+00007f70: 6174 6120 3d20 6d75 7369 635f 7461 672e  ata = music_tag.
+00007f80: 6c6f 6164 5f66 696c 6528 0a20 2020 2020  load_file(.     
 00007f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007fb0: 2020 206f 732e 7061 7468 2e6a 6f69 6e28     os.path.join(
-00007fc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007fb0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+00007fc0: 732e 7061 7468 2e6a 6f69 6e28 0a20 2020  s.path.join(.   
 00007fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ff0: 2020 2020 2020 2020 2053 4f4e 4753 5f44           SONGS_D
-00008000: 4952 2c20 6465 7461 696c 735b 315d 0a20  IR, details[1]. 
-00008010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008000: 2020 2020 2053 4f4e 4753 5f44 4952 2c20       SONGS_DIR, 
+00008010: 6465 7461 696c 735b 315d 0a20 2020 2020  details[1].     
 00008020: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008040: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00008050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008040: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00008050: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00008060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008070: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00008080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008080: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
 00008090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000080a0: 2020 2020 2020 2064 6574 6169 6c73 202b         details +
-000080b0: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
+000080a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000080b0: 2020 2064 6574 6169 6c73 202b 3d20 5b0a     details += [.
 000080c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000080d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000080e0: 2020 2020 2020 2020 280a 2020 2020 2020          (.      
-000080f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000080e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000080f0: 2020 2020 280a 2020 2020 2020 2020 2020      (.          
 00008100: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008120: 2020 736f 6e67 5f64 6174 615b 0a20 2020    song_data[.   
-00008130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008120: 2020 2020 2020 2020 2020 2020 2020 736f                so
+00008130: 6e67 5f64 6174 615b 0a20 2020 2020 2020  ng_data[.       
 00008140: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008160: 2020 2020 2020 2020 2022 6172 7469 7374           "artist
-00008170: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00008160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008170: 2020 2020 2022 6172 7469 7374 220a 2020       "artist".  
 00008180: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000081a0: 2020 2020 2020 2020 2020 5d2e 7661 6c75            ].valu
-000081b0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+000081a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000081b0: 2020 2020 2020 5d2e 7661 6c75 650a 2020        ].value.  
 000081c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000081d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000081e0: 2020 2020 2020 2020 2020 6f72 2022 556e            or "Un
-000081f0: 6b6e 6f77 6e20 4172 7469 7374 220a 2020  known Artist".  
-00008200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000081e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000081f0: 2020 2020 2020 6f72 2022 556e 6b6e 6f77        or "Unknow
+00008200: 6e20 4172 7469 7374 220a 2020 2020 2020  n Artist".      
 00008210: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008230: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
-00008240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008230: 2020 2020 2020 2020 2020 2020 2020 292c                ),
+00008240: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00008250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008260: 2020 2020 2020 2020 2028 0a20 2020 2020           (.     
-00008270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008270: 2020 2020 2028 0a20 2020 2020 2020 2020       (.         
 00008280: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000082a0: 2020 2073 6f6e 675f 6461 7461 5b22 616c     song_data["al
-000082b0: 6275 6d22 5d2e 7661 6c75 650a 2020 2020  bum"].value.    
-000082c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000082a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000082b0: 6f6e 675f 6461 7461 5b22 616c 6275 6d22  ong_data["album"
+000082c0: 5d2e 7661 6c75 650a 2020 2020 2020 2020  ].value.        
 000082d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000082e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000082f0: 2020 2020 6f72 2022 556e 6b6e 6f77 6e20      or "Unknown 
-00008300: 416c 6275 6d22 0a20 2020 2020 2020 2020  Album".         
-00008310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000082f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008300: 6f72 2022 556e 6b6e 6f77 6e20 416c 6275  or "Unknown Albu
+00008310: 6d22 0a20 2020 2020 2020 2020 2020 2020  m".             
 00008320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008330: 2020 2020 2020 2020 2020 2029 2c0a 2020             ),.  
-00008340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008340: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
 00008350: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008370: 2020 280a 2020 2020 2020 2020 2020 2020    (.            
+00008370: 2020 2020 2020 2020 2020 2020 2020 280a                (.
 00008380: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000083a0: 2020 2020 2020 2020 2020 2020 736f 6e67              song
-000083b0: 5f64 6174 615b 0a20 2020 2020 2020 2020  _data[.         
-000083c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000083a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000083b0: 2020 2020 2020 2020 736f 6e67 5f64 6174          song_dat
+000083c0: 615b 0a20 2020 2020 2020 2020 2020 2020  a[.             
 000083d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000083e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000083f0: 2020 2022 616c 6275 6d61 7274 6973 7422     "albumartist"
-00008400: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000083f0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00008400: 616c 6275 6d61 7274 6973 7422 0a20 2020  albumartist".   
 00008410: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008430: 2020 2020 2020 2020 205d 2e76 616c 7565           ].value
-00008440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008440: 2020 2020 205d 2e76 616c 7565 0a20 2020       ].value.   
 00008450: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008470: 2020 2020 2020 2020 206f 7220 2255 6e6b           or "Unk
-00008480: 6e6f 776e 2041 6c62 756d 2041 7274 6973  nown Album Artis
-00008490: 7422 0a20 2020 2020 2020 2020 2020 2020  t".             
+00008470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008480: 2020 2020 206f 7220 2255 6e6b 6e6f 776e       or "Unknown
+00008490: 2041 6c62 756d 2041 7274 6973 7422 0a20   Album Artist". 
 000084a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000084b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000084c0: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
-000084d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000084c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000084d0: 2020 2029 2c0a 2020 2020 2020 2020 2020     ),.          
 000084e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000084f0: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
-00008500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000084f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008500: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
 00008510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008520: 2020 2020 2020 2020 2020 2020 6966 2028              if (
-00008530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008530: 2020 2020 2020 2020 6966 2028 0a20 2020          if (.   
 00008540: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008560: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
-00008570: 7574 2e70 726f 6d70 7469 6e67 5b32 5d0a  ut.prompting[2].
-00008580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008570: 2070 6c61 7965 725f 6f75 7470 7574 2e70   player_output.p
+00008580: 726f 6d70 7469 6e67 5b32 5d0a 2020 2020  rompting[2].    
 00008590: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000085a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000085b0: 2020 2020 3d3d 2050 524f 4d50 545f 4d4f      == PROMPT_MO
-000085c0: 4445 535b 2269 6e73 6572 7422 5d0a 2020  DES["insert"].  
-000085d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000085b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000085c0: 3d3d 2050 524f 4d50 545f 4d4f 4445 535b  == PROMPT_MODES[
+000085d0: 2269 6e73 6572 7422 5d0a 2020 2020 2020  "insert"].      
 000085e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000085f0: 2020 2020 2020 2020 2020 2020 2020 293a                ):
-00008600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000085f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008600: 2020 2020 2020 2020 2020 293a 0a20 2020            ):.   
 00008610: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008630: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
-00008640: 7574 2e70 6c61 796c 6973 742e 696e 7365  ut.playlist.inse
-00008650: 7274 280a 2020 2020 2020 2020 2020 2020  rt(.            
+00008630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008640: 2070 6c61 7965 725f 6f75 7470 7574 2e70   player_output.p
+00008650: 6c61 796c 6973 742e 696e 7365 7274 280a  laylist.insert(.
 00008660: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008680: 2020 2020 2020 2020 2020 2020 706c 6179              play
-00008690: 6572 5f6f 7574 7075 742e 7363 726f 6c6c  er_output.scroll
-000086a0: 6572 2e70 6f73 0a20 2020 2020 2020 2020  er.pos.         
-000086b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008690: 2020 2020 2020 2020 706c 6179 6572 5f6f          player_o
+000086a0: 7574 7075 742e 7363 726f 6c6c 6572 2e70  utput.scroller.p
+000086b0: 6f73 0a20 2020 2020 2020 2020 2020 2020  os.             
 000086c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000086d0: 2020 2020 2020 2020 2020 2020 2020 202b                 +
-000086e0: 2031 2c0a 2020 2020 2020 2020 2020 2020   1,.            
+000086d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000086e0: 2020 2020 2020 2020 2020 202b 2031 2c0a             + 1,.
 000086f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008710: 2020 2020 2020 2020 2020 2020 6465 7461              deta
-00008720: 696c 732c 0a20 2020 2020 2020 2020 2020  ils,.           
-00008730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008720: 2020 2020 2020 2020 6465 7461 696c 732c          details,
+00008730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00008740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008750: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00008760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008760: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
 00008770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008780: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00008790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008790: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
 000087a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000087b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000087c0: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
-000087d0: 7574 2e70 6c61 796c 6973 742e 6170 7065  ut.playlist.appe
-000087e0: 6e64 280a 2020 2020 2020 2020 2020 2020  nd(.            
+000087c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000087d0: 2070 6c61 7965 725f 6f75 7470 7574 2e70   player_output.p
+000087e0: 6c61 796c 6973 742e 6170 7065 6e64 280a  laylist.append(.
 000087f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008810: 2020 2020 2020 2020 2020 2020 6465 7461              deta
-00008820: 696c 730a 2020 2020 2020 2020 2020 2020  ils.            
+00008810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008820: 2020 2020 2020 2020 6465 7461 696c 730a          details.
 00008830: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008850: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00008860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008860: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
 00008870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008880: 2020 2020 2020 2020 2020 6966 206c 6f6f            if loo
-00008890: 703a 0a20 2020 2020 2020 2020 2020 2020  p:.             
+00008880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008890: 2020 2020 2020 6966 206c 6f6f 703a 0a20        if loop:. 
 000088a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000088b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000088c0: 2020 2020 2020 2069 6620 7265 7368 7566         if reshuf
-000088d0: 666c 653a 0a20 2020 2020 2020 2020 2020  fle:.           
-000088e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000088c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000088d0: 2020 2069 6620 7265 7368 7566 666c 653a     if reshuffle:
+000088e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 000088f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008900: 2020 2020 2020 2020 2020 2020 206e 6578               nex
-00008910: 745f 706c 6179 6c69 7374 2e69 6e73 6572  t_playlist.inser
-00008920: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
+00008900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008910: 2020 2020 2020 2020 206e 6578 745f 706c           next_pl
+00008920: 6179 6c69 7374 2e69 6e73 6572 7428 0a20  aylist.insert(. 
 00008930: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008950: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00008960: 616e 6469 6e74 280a 2020 2020 2020 2020  andint(.        
-00008970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008960: 2020 2020 2020 2020 2020 2072 616e 6469             randi
+00008970: 6e74 280a 2020 2020 2020 2020 2020 2020  nt(.            
 00008980: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089a0: 2020 2020 2020 2020 302c 0a20 2020 2020          0,.     
-000089b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000089a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000089b0: 2020 2020 302c 0a20 2020 2020 2020 2020      0,.         
 000089c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000089d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089e0: 2020 2020 2020 2020 2020 206c 656e 280a             len(.
-000089f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000089e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000089f0: 2020 2020 2020 206c 656e 280a 2020 2020         len(.    
 00008a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a30: 2020 2020 6e65 7874 5f70 6c61 796c 6973      next_playlis
-00008a40: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
+00008a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a40: 6e65 7874 5f70 6c61 796c 6973 740a 2020  next_playlist.  
 00008a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a80: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00008a80: 2020 2020 2020 2020 2020 2020 2020 290a                ).
 00008a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ac0: 2020 2020 2d20 312c 0a20 2020 2020 2020      - 1,.       
-00008ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ad0: 2d20 312c 0a20 2020 2020 2020 2020 2020  - 1,.           
 00008ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b00: 2020 2020 2029 2c0a 2020 2020 2020 2020       ),.        
-00008b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b10: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
 00008b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b40: 2020 2020 6465 7461 696c 732c 0a20 2020      details,.   
-00008b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b50: 6465 7461 696c 732c 0a20 2020 2020 2020  details,.       
 00008b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b80: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00008b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b90: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
 00008ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008bb0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00008bc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008bc0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
 00008bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008bf0: 2020 2020 2020 2020 2069 6620 280a 2020           if (.  
-00008c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008c00: 2020 2020 2069 6620 280a 2020 2020 2020       if (.      
 00008c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c30: 2020 2020 2020 2020 2020 706c 6179 6572            player
-00008c40: 5f6f 7574 7075 742e 7072 6f6d 7074 696e  _output.promptin
-00008c50: 675b 0a20 2020 2020 2020 2020 2020 2020  g[.             
+00008c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008c40: 2020 2020 2020 706c 6179 6572 5f6f 7574        player_out
+00008c50: 7075 742e 7072 6f6d 7074 696e 675b 0a20  put.prompting[. 
 00008c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c90: 2020 2032 0a20 2020 2020 2020 2020 2020     2.           
-00008ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008c90: 2020 2020 2020 2020 2020 2020 2020 2032                 2
+00008ca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00008cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008cd0: 205d 0a20 2020 2020 2020 2020 2020 2020   ].             
+00008cd0: 2020 2020 2020 2020 2020 2020 205d 0a20               ]. 
 00008ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d00: 2020 2020 2020 2020 2020 2020 2020 203d                 =
-00008d10: 3d20 5052 4f4d 5054 5f4d 4f44 4553 5b0a  = PROMPT_MODES[.
-00008d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008d10: 2020 2020 2020 2020 2020 203d 3d20 5052             == PR
+00008d20: 4f4d 5054 5f4d 4f44 4553 5b0a 2020 2020  OMPT_MODES[.    
 00008d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d60: 2269 6e73 6572 7422 0a20 2020 2020 2020  "insert".       
-00008d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008d60: 2020 2020 2020 2020 2020 2020 2269 6e73              "ins
+00008d70: 6572 7422 0a20 2020 2020 2020 2020 2020  ert".           
 00008d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008da0: 2020 2020 205d 0a20 2020 2020 2020 2020       ].         
-00008db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008db0: 205d 0a20 2020 2020 2020 2020 2020 2020   ].             
 00008dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008dd0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00008de0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00008dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008de0: 2020 2020 2020 2020 2020 2029 3a0a 2020             ):.  
 00008df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e10: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
-00008e20: 7874 5f70 6c61 796c 6973 742e 696e 7365  xt_playlist.inse
-00008e30: 7274 280a 2020 2020 2020 2020 2020 2020  rt(.            
+00008e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e20: 2020 2020 2020 2020 2020 6e65 7874 5f70            next_p
+00008e30: 6c61 796c 6973 742e 696e 7365 7274 280a  laylist.insert(.
 00008e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e70: 2020 2020 706c 6179 6572 5f6f 7574 7075      player_outpu
-00008e80: 742e 7363 726f 6c6c 6572 2e70 6f73 0a20  t.scroller.pos. 
-00008e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e80: 706c 6179 6572 5f6f 7574 7075 742e 7363  player_output.sc
+00008e90: 726f 6c6c 6572 2e70 6f73 0a20 2020 2020  roller.pos.     
 00008ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ec0: 2020 2020 2020 2020 2020 2020 2020 202b                 +
-00008ed0: 2031 2c0a 2020 2020 2020 2020 2020 2020   1,.            
+00008ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ed0: 2020 2020 2020 2020 2020 202b 2031 2c0a             + 1,.
 00008ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f10: 2020 2020 6465 7461 696c 732c 0a20 2020      details,.   
-00008f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f20: 6465 7461 696c 732c 0a20 2020 2020 2020  details,.       
 00008f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f50: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00008f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f60: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
 00008f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f90: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00008fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f90: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00008fa0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
 00008fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008fd0: 2020 2020 206e 6578 745f 706c 6179 6c69       next_playli
-00008fe0: 7374 2e61 7070 656e 6428 0a20 2020 2020  st.append(.     
-00008ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008fe0: 206e 6578 745f 706c 6179 6c69 7374 2e61   next_playlist.a
+00008ff0: 7070 656e 6428 0a20 2020 2020 2020 2020  ppend(.         
 00009000: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009020: 2020 2020 2020 2020 2020 2064 6574 6169             detai
-00009030: 6c73 0a20 2020 2020 2020 2020 2020 2020  ls.             
+00009020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009030: 2020 2020 2020 2064 6574 6169 6c73 0a20         details. 
 00009040: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009060: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00009070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009070: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
 00009080: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000090a0: 2070 6c61 7965 725f 6f75 7470 7574 2e73   player_output.s
-000090b0: 6372 6f6c 6c65 722e 6e75 6d5f 6c69 6e65  croller.num_line
-000090c0: 7320 2b3d 2028 0a20 2020 2020 2020 2020  s += (.         
-000090d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000090a0: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
+000090b0: 7965 725f 6f75 7470 7574 2e73 6372 6f6c  yer_output.scrol
+000090c0: 6c65 722e 6e75 6d5f 6c69 6e65 7320 2b3d  ler.num_lines +=
+000090d0: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
 000090e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000090f0: 2020 2020 2020 2020 2020 2031 0a20 2020             1.   
-00009100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000090f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009100: 2020 2020 2020 2031 0a20 2020 2020 2020         1.       
 00009110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009120: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-00009130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009130: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
 00009140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009150: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00009160: 6c61 7965 725f 6f75 7470 7574 2e70 726f  layer_output.pro
-00009170: 6d70 7469 6e67 203d 204e 6f6e 650a 2020  mpting = None.  
-00009180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009160: 2020 2020 2020 2020 2020 2070 6c61 7965             playe
+00009170: 725f 6f75 7470 7574 2e70 726f 6d70 7469  r_output.prompti
+00009180: 6e67 203d 204e 6f6e 650a 2020 2020 2020  ng = None.      
 00009190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000091a0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-000091b0: 7273 6573 2e63 7572 735f 7365 7428 4661  rses.curs_set(Fa
-000091c0: 6c73 6529 0a20 2020 2020 2020 2020 2020  lse).           
-000091d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000091a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000091b0: 2020 2020 2020 2020 2020 6375 7273 6573            curses
+000091c0: 2e63 7572 735f 7365 7428 4661 6c73 6529  .curs_set(False)
+000091d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 000091e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000091f0: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
-00009200: 7574 2e73 6372 6f6c 6c65 722e 7265 7369  ut.scroller.resi
-00009210: 7a65 280a 2020 2020 2020 2020 2020 2020  ze(.            
+000091f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009200: 2070 6c61 7965 725f 6f75 7470 7574 2e73   player_output.s
+00009210: 6372 6f6c 6c65 722e 7265 7369 7a65 280a  croller.resize(.
 00009220: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009240: 2020 2020 2020 2020 7363 7265 656e 5f73          screen_s
-00009250: 697a 655b 305d 202d 2032 0a20 2020 2020  ize[0] - 2.     
-00009260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009250: 2020 2020 7363 7265 656e 5f73 697a 655b      screen_size[
+00009260: 305d 202d 2032 0a20 2020 2020 2020 2020  0] - 2.         
 00009270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009280: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00009290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009290: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
 000092a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000092b0: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
-000092c0: 7965 725f 6f75 7470 7574 2e6f 7574 7075  yer_output.outpu
-000092d0: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
+000092b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000092c0: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
+000092d0: 6f75 7470 7574 2e6f 7574 7075 7428 0a20  output.output(. 
 000092e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000092f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009300: 2020 2020 2020 2070 6c61 7962 6163 6b2e         playback.
-00009310: 6375 7272 5f70 6f73 0a20 2020 2020 2020  curr_pos.       
-00009320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009310: 2020 2070 6c61 7962 6163 6b2e 6375 7272     playback.curr
+00009320: 5f70 6f73 0a20 2020 2020 2020 2020 2020  _pos.           
 00009330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009340: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00009350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009350: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
 00009360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009370: 2020 2020 2020 2020 2020 2062 7265 616b             break
-00009380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009390: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
-000093a0: 6620 280a 2020 2020 2020 2020 2020 2020  f (.            
+00009370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009380: 2020 2020 2020 2062 7265 616b 0a20 2020         break.   
+00009390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000093a0: 2020 2020 2020 2020 2065 6c69 6620 280a           elif (.
 000093b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000093c0: 2020 2020 227c 2220 6e6f 7420 696e 2070      "|" not in p
-000093d0: 6c61 7965 725f 6f75 7470 7574 2e70 726f  layer_output.pro
-000093e0: 6d70 7469 6e67 5b30 5d0a 2020 2020 2020  mpting[0].      
-000093f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009400: 2020 2020 2020 2020 2020 616e 6420 706c            and pl
-00009410: 6179 6572 5f6f 7574 7075 742e 7072 6f6d  ayer_output.prom
-00009420: 7074 696e 675b 325d 0a20 2020 2020 2020  pting[2].       
-00009430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009440: 2020 2020 2020 2020 203d 3d20 5052 4f4d           == PROM
-00009450: 5054 5f4d 4f44 4553 5b22 7461 6722 5d0a  PT_MODES["tag"].
-00009460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009470: 2020 2020 2020 2020 2020 2020 293a 0a20              ):. 
-00009480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009490: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-000094a0: 6167 7320 3d20 706c 6179 6572 5f6f 7574  ags = player_out
-000094b0: 7075 742e 7072 6f6d 7074 696e 675b 305d  put.prompting[0]
-000094c0: 2e73 706c 6974 2822 2c22 290a 0a20 2020  .split(",")..   
-000094d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000094e0: 2020 2020 2020 2020 2020 2020 2074 6167               tag
-000094f0: 6769 6e67 5f69 6473 203d 207b 7d0a 2020  ging_ids = {}.  
-00009500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009510: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00009520: 7220 6920 696e 2072 616e 6765 286c 656e  r i in range(len
-00009530: 2870 6c61 7965 725f 6f75 7470 7574 2e70  (player_output.p
-00009540: 6c61 796c 6973 7429 293a 0a20 2020 2020  laylist)):.     
-00009550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009560: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00009570: 6167 6769 6e67 5f69 6473 5b0a 2020 2020  agging_ids[.    
-00009580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000093c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000093d0: 227c 2220 6e6f 7420 696e 2070 6c61 7965  "|" not in playe
+000093e0: 725f 6f75 7470 7574 2e70 726f 6d70 7469  r_output.prompti
+000093f0: 6e67 5b30 5d0a 2020 2020 2020 2020 2020  ng[0].          
+00009400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009410: 2020 2020 2020 616e 6420 706c 6179 6572        and player
+00009420: 5f6f 7574 7075 742e 7072 6f6d 7074 696e  _output.promptin
+00009430: 675b 325d 0a20 2020 2020 2020 2020 2020  g[2].           
+00009440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009450: 2020 2020 203d 3d20 5052 4f4d 5054 5f4d       == PROMPT_M
+00009460: 4f44 4553 5b22 7461 6722 5d0a 2020 2020  ODES["tag"].    
+00009470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009480: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
+00009490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000094a0: 2020 2020 2020 2020 2020 2074 6167 7320             tags 
+000094b0: 3d20 706c 6179 6572 5f6f 7574 7075 742e  = player_output.
+000094c0: 7072 6f6d 7074 696e 675b 305d 2e73 706c  prompting[0].spl
+000094d0: 6974 2822 2c22 290a 0a20 2020 2020 2020  it(",")..       
+000094e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000094f0: 2020 2020 2020 2020 2074 6167 6769 6e67           tagging
+00009500: 5f69 6473 203d 207b 7d0a 2020 2020 2020  _ids = {}.      
+00009510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009520: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
+00009530: 696e 2072 616e 6765 286c 656e 2870 6c61  in range(len(pla
+00009540: 7965 725f 6f75 7470 7574 2e70 6c61 796c  yer_output.playl
+00009550: 6973 7429 293a 0a20 2020 2020 2020 2020  ist)):.         
+00009560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009570: 2020 2020 2020 2020 2020 2074 6167 6769             taggi
+00009580: 6e67 5f69 6473 5b0a 2020 2020 2020 2020  ng_ids[.        
 00009590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000095a0: 2020 2020 696e 7428 706c 6179 6572 5f6f      int(player_o
-000095b0: 7574 7075 742e 706c 6179 6c69 7374 5b69  utput.playlist[i
-000095c0: 5d5b 305d 290a 2020 2020 2020 2020 2020  ][0]).          
-000095d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000095e0: 2020 2020 2020 2020 2020 5d20 3d20 690a            ] = i.
-000095f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000095a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000095b0: 696e 7428 706c 6179 6572 5f6f 7574 7075  int(player_outpu
+000095c0: 742e 706c 6179 6c69 7374 5b69 5d5b 305d  t.playlist[i][0]
+000095d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000095e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000095f0: 2020 2020 2020 5d20 3d20 690a 0a20 2020        ] = i..   
 00009600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009610: 2073 6f6e 6773 5f66 696c 6520 3d20 6f70   songs_file = op
-00009620: 656e 280a 2020 2020 2020 2020 2020 2020  en(.            
+00009610: 2020 2020 2020 2020 2020 2020 2073 6f6e               son
+00009620: 6773 5f66 696c 6520 3d20 6f70 656e 280a  gs_file = open(.
 00009630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009640: 2020 2020 2020 2020 534f 4e47 535f 494e          SONGS_IN
-00009650: 464f 5f50 4154 482c 2022 7222 2c20 656e  FO_PATH, "r", en
-00009660: 636f 6469 6e67 3d22 7574 662d 3822 0a20  coding="utf-8". 
-00009670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009680: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00009690: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009650: 2020 2020 534f 4e47 535f 494e 464f 5f50      SONGS_INFO_P
+00009660: 4154 482c 2022 7222 2c20 656e 636f 6469  ATH, "r", encodi
+00009670: 6e67 3d22 7574 662d 3822 0a20 2020 2020  ng="utf-8".     
+00009680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009690: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
 000096a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000096b0: 206c 696e 6573 203d 2073 6f6e 6773 5f66   lines = songs_f
-000096c0: 696c 652e 7265 6164 2829 2e73 706c 6974  ile.read().split
-000096d0: 6c69 6e65 7328 290a 2020 2020 2020 2020  lines().        
-000096e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000096f0: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-00009700: 2072 616e 6765 286c 656e 286c 696e 6573   range(len(lines
-00009710: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
+000096b0: 2020 2020 2020 2020 2020 2020 206c 696e               lin
+000096c0: 6573 203d 2073 6f6e 6773 5f66 696c 652e  es = songs_file.
+000096d0: 7265 6164 2829 2e73 706c 6974 6c69 6e65  read().splitline
+000096e0: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
+000096f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009700: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+00009710: 6765 286c 656e 286c 696e 6573 2929 3a0a  ge(len(lines)):.
 00009720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009730: 2020 2020 2020 2020 6465 7461 696c 7320          details 
-00009740: 3d20 6c69 6e65 735b 695d 2e73 7472 6970  = lines[i].strip
-00009750: 2829 2e73 706c 6974 2822 7c22 290a 2020  ().split("|").  
-00009760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009740: 2020 2020 6465 7461 696c 7320 3d20 6c69      details = li
+00009750: 6e65 735b 695d 2e73 7472 6970 2829 2e73  nes[i].strip().s
+00009760: 706c 6974 2822 7c22 290a 2020 2020 2020  plit("|").      
 00009770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009780: 2020 736f 6e67 5f69 6420 3d20 696e 7428    song_id = int(
-00009790: 6465 7461 696c 735b 305d 290a 2020 2020  details[0]).    
-000097a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009780: 2020 2020 2020 2020 2020 2020 2020 736f                so
+00009790: 6e67 5f69 6420 3d20 696e 7428 6465 7461  ng_id = int(deta
+000097a0: 696c 735b 305d 290a 2020 2020 2020 2020  ils[0]).        
 000097b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000097c0: 6966 2073 6f6e 675f 6964 2069 6e20 7461  if song_id in ta
-000097d0: 6767 696e 675f 6964 733a 0a20 2020 2020  gging_ids:.     
-000097e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000097c0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+000097d0: 6f6e 675f 6964 2069 6e20 7461 6767 696e  ong_id in taggin
+000097e0: 675f 6964 733a 0a20 2020 2020 2020 2020  g_ids:.         
 000097f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009800: 2020 2069 6620 6465 7461 696c 735b 325d     if details[2]
-00009810: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00009800: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00009810: 6620 6465 7461 696c 735b 325d 3a0a 2020  f details[2]:.  
 00009820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009830: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
-00009840: 775f 7461 6773 203d 2064 6574 6169 6c73  w_tags = details
-00009850: 5b32 5d2e 7370 6c69 7428 222c 2229 0a20  [2].split(","). 
-00009860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009840: 2020 2020 2020 2020 2020 6e65 775f 7461            new_ta
+00009850: 6773 203d 2064 6574 6169 6c73 5b32 5d2e  gs = details[2].
+00009860: 7370 6c69 7428 222c 2229 0a20 2020 2020  split(",").     
 00009870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009880: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00009890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009890: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
 000098a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000098b0: 2020 2020 2020 2020 206e 6577 5f74 6167           new_tag
-000098c0: 7320 3d20 5b5d 0a20 2020 2020 2020 2020  s = [].         
-000098d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000098e0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-000098f0: 6577 5f74 6167 7320 2b3d 205b 0a20 2020  ew_tags += [.   
-00009900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000098b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000098c0: 2020 2020 206e 6577 5f74 6167 7320 3d20       new_tags = 
+000098d0: 5b5d 0a20 2020 2020 2020 2020 2020 2020  [].             
+000098e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000098f0: 2020 2020 2020 2020 2020 206e 6577 5f74             new_t
+00009900: 6167 7320 2b3d 205b 0a20 2020 2020 2020  ags += [.       
 00009910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009920: 2020 2020 2020 2020 2074 6167 0a20 2020           tag.   
-00009930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009930: 2020 2020 2074 6167 0a20 2020 2020 2020       tag.       
 00009940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009950: 2020 2020 2020 2020 2066 6f72 2074 6167           for tag
-00009960: 2069 6e20 7461 6773 0a20 2020 2020 2020   in tags.       
-00009970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009960: 2020 2020 2066 6f72 2074 6167 2069 6e20       for tag in 
+00009970: 7461 6773 0a20 2020 2020 2020 2020 2020  tags.           
 00009980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009990: 2020 2020 2069 6620 7461 6720 6e6f 7420       if tag not 
-000099a0: 696e 206e 6577 5f74 6167 730a 2020 2020  in new_tags.    
-000099b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000099a0: 2069 6620 7461 6720 6e6f 7420 696e 206e   if tag not in n
+000099b0: 6577 5f74 6167 730a 2020 2020 2020 2020  ew_tags.        
 000099c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000099d0: 2020 2020 5d0a 2020 2020 2020 2020 2020      ].          
-000099e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000099f0: 2020 2020 2020 2020 2020 2020 2020 6465                de
-00009a00: 7461 696c 735b 325d 203d 2022 2c22 2e6a  tails[2] = ",".j
-00009a10: 6f69 6e28 6e65 775f 7461 6773 290a 2020  oin(new_tags).  
-00009a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000099d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000099e0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+000099f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009a00: 2020 2020 2020 2020 2020 6465 7461 696c            detail
+00009a10: 735b 325d 203d 2022 2c22 2e6a 6f69 6e28  s[2] = ",".join(
+00009a20: 6e65 775f 7461 6773 290a 2020 2020 2020  new_tags).      
 00009a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a40: 2020 2020 2020 6c69 6e65 735b 695d 203d        lines[i] =
-00009a50: 2022 7c22 2e6a 6f69 6e28 6465 7461 696c   "|".join(detail
-00009a60: 7329 0a20 2020 2020 2020 2020 2020 2020  s).             
+00009a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009a50: 2020 6c69 6e65 735b 695d 203d 2022 7c22    lines[i] = "|"
+00009a60: 2e6a 6f69 6e28 6465 7461 696c 7329 0a20  .join(details). 
 00009a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a80: 2020 2020 2020 2020 2020 2070 6c61 7965             playe
-00009a90: 725f 6f75 7470 7574 2e70 6c61 796c 6973  r_output.playlis
-00009aa0: 745b 0a20 2020 2020 2020 2020 2020 2020  t[.             
+00009a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009a90: 2020 2020 2020 2070 6c61 7965 725f 6f75         player_ou
+00009aa0: 7470 7574 2e70 6c61 796c 6973 745b 0a20  tput.playlist[. 
 00009ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ac0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00009ad0: 6167 6769 6e67 5f69 6473 5b73 6f6e 675f  agging_ids[song_
-00009ae0: 6964 5d0a 2020 2020 2020 2020 2020 2020  id].            
+00009ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ad0: 2020 2020 2020 2020 2020 2074 6167 6769             taggi
+00009ae0: 6e67 5f69 6473 5b73 6f6e 675f 6964 5d0a  ng_ids[song_id].
 00009af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b00: 2020 2020 2020 2020 2020 2020 5d5b 325d              ][2]
-00009b10: 203d 2064 6574 6169 6c73 5b32 5d0a 2020   = details[2].  
-00009b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b30: 2020 2020 2020 2020 2020 2020 2020 736f                so
-00009b40: 6e67 735f 6669 6c65 2e63 6c6f 7365 2829  ngs_file.close()
-00009b50: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00009b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b10: 2020 2020 2020 2020 5d5b 325d 203d 2064          ][2] = d
+00009b20: 6574 6169 6c73 5b32 5d0a 2020 2020 2020  etails[2].      
+00009b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b40: 2020 2020 2020 2020 2020 736f 6e67 735f            songs_
+00009b50: 6669 6c65 2e63 6c6f 7365 2829 0a0a 2020  file.close()..  
 00009b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b70: 2020 736f 6e67 735f 6669 6c65 203d 206f    songs_file = o
-00009b80: 7065 6e28 0a20 2020 2020 2020 2020 2020  pen(.           
-00009b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ba0: 2020 2020 2020 2020 2053 4f4e 4753 5f49           SONGS_I
-00009bb0: 4e46 4f5f 5041 5448 2c20 2277 222c 2065  NFO_PATH, "w", e
-00009bc0: 6e63 6f64 696e 673d 2275 7466 2d38 220a  ncoding="utf-8".
-00009bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b70: 2020 2020 2020 2020 2020 2020 2020 736f                so
+00009b80: 6e67 735f 6669 6c65 203d 206f 7065 6e28  ngs_file = open(
+00009b90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009bb0: 2020 2020 2053 4f4e 4753 5f49 4e46 4f5f       SONGS_INFO_
+00009bc0: 5041 5448 2c20 2277 222c 2065 6e63 6f64  PATH, "w", encod
+00009bd0: 696e 673d 2275 7466 2d38 220a 2020 2020  ing="utf-8".    
 00009be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009bf0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00009bf0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
 00009c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c10: 2020 736f 6e67 735f 6669 6c65 2e77 7269    songs_file.wri
-00009c20: 7465 2822 5c6e 222e 6a6f 696e 286c 696e  te("\n".join(lin
-00009c30: 6573 2929 0a20 2020 2020 2020 2020 2020  es)).           
-00009c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c50: 2020 2020 2073 6f6e 6773 5f66 696c 652e       songs_file.
-00009c60: 636c 6f73 6528 290a 0a20 2020 2020 2020  close()..       
-00009c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c80: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
-00009c90: 6f75 7470 7574 2e70 726f 6d70 7469 6e67  output.prompting
-00009ca0: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
-00009cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009cc0: 2020 2020 2020 2020 6375 7273 6573 2e63          curses.c
-00009cd0: 7572 735f 7365 7428 4661 6c73 6529 0a20  urs_set(False). 
-00009ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009cf0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00009d00: 6c61 7965 725f 6f75 7470 7574 2e6f 7574  layer_output.out
-00009d10: 7075 7428 706c 6179 6261 636b 2e63 7572  put(playback.cur
-00009d20: 725f 706f 7329 0a20 2020 2020 2020 2020  r_pos).         
-00009d30: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00009d40: 6c69 6620 6320 3d3d 2032 373a 2020 2320  lif c == 27:  # 
-00009d50: 4553 4320 6b65 790a 2020 2020 2020 2020  ESC key.        
-00009d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d70: 2020 2020 706c 6179 6572 5f6f 7574 7075      player_outpu
-00009d80: 742e 7072 6f6d 7074 696e 6720 3d20 4e6f  t.prompting = No
-00009d90: 6e65 0a20 2020 2020 2020 2020 2020 2020  ne.             
-00009da0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00009db0: 7572 7365 732e 6375 7273 5f73 6574 2846  urses.curs_set(F
-00009dc0: 616c 7365 290a 2020 2020 2020 2020 2020  alse).          
-00009dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009de0: 2020 706c 6179 6572 5f6f 7574 7075 742e    player_output.
-00009df0: 7363 726f 6c6c 6572 2e72 6573 697a 6528  scroller.resize(
-00009e00: 7363 7265 656e 5f73 697a 655b 305d 202d  screen_size[0] -
-00009e10: 2032 290a 2020 2020 2020 2020 2020 2020   2).            
+00009c10: 2020 2020 2020 2020 2020 2020 2020 736f                so
+00009c20: 6e67 735f 6669 6c65 2e77 7269 7465 2822  ngs_file.write("
+00009c30: 5c6e 222e 6a6f 696e 286c 696e 6573 2929  \n".join(lines))
+00009c40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c60: 2073 6f6e 6773 5f66 696c 652e 636c 6f73   songs_file.clos
+00009c70: 6528 290a 0a20 2020 2020 2020 2020 2020  e()..           
+00009c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c90: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
+00009ca0: 7574 2e70 726f 6d70 7469 6e67 203d 204e  ut.prompting = N
+00009cb0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+00009cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009cd0: 2020 2020 6375 7273 6573 2e63 7572 735f      curses.curs_
+00009ce0: 7365 7428 4661 6c73 6529 0a20 2020 2020  set(False).     
+00009cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009d00: 2020 2020 2020 2020 2020 2070 6c61 7965             playe
+00009d10: 725f 6f75 7470 7574 2e6f 7574 7075 7428  r_output.output(
+00009d20: 706c 6179 6261 636b 2e63 7572 725f 706f  playback.curr_po
+00009d30: 7329 0a20 2020 2020 2020 2020 2020 2020  s).             
+00009d40: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00009d50: 6320 3d3d 2032 373a 2020 2320 4553 4320  c == 27:  # ESC 
+00009d60: 6b65 790a 2020 2020 2020 2020 2020 2020  key.            
+00009d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009d80: 706c 6179 6572 5f6f 7574 7075 742e 7072  player_output.pr
+00009d90: 6f6d 7074 696e 6720 3d20 4e6f 6e65 0a20  ompting = None. 
+00009da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009db0: 2020 2020 2020 2020 2020 2063 7572 7365             curse
+00009dc0: 732e 6375 7273 5f73 6574 2846 616c 7365  s.curs_set(False
+00009dd0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00009de0: 2020 2020 2020 2020 2020 2020 2020 706c                pl
+00009df0: 6179 6572 5f6f 7574 7075 742e 7363 726f  ayer_output.scro
+00009e00: 6c6c 6572 2e72 6573 697a 6528 7363 7265  ller.resize(scre
+00009e10: 656e 5f73 697a 655b 305d 202d 2032 290a  en_size[0] - 2).
 00009e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e30: 706c 6179 6572 5f6f 7574 7075 742e 6f75  player_output.ou
-00009e40: 7470 7574 2870 6c61 7962 6163 6b2e 6375  tput(playback.cu
-00009e50: 7272 5f70 6f73 290a 2020 2020 2020 2020  rr_pos).        
-00009e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e70: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00009e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e90: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-00009ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009eb0: 2020 2020 2020 2063 203d 2063 6872 2863         c = chr(c
-00009ec0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00009e30: 2020 2020 2020 2020 2020 2020 706c 6179              play
+00009e40: 6572 5f6f 7574 7075 742e 6f75 7470 7574  er_output.output
+00009e50: 2870 6c61 7962 6163 6b2e 6375 7272 5f70  (playback.curr_p
+00009e60: 6f73 290a 2020 2020 2020 2020 2020 2020  os).            
+00009e70: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00009e80: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00009e90: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+00009ea0: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
+00009eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ec0: 2020 2063 203d 2063 6872 2863 290a 2020     c = chr(c).  
 00009ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ee0: 2020 6966 2063 2069 6e20 225c 725c 6e22    if c in "\r\n"
-00009ef0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00009ee0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00009ef0: 2063 2069 6e20 225c 725c 6e22 3a0a 2020   c in "\r\n":.  
 00009f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f10: 2020 2020 2020 2320 7079 6c69 6e74 3a20        # pylint: 
-00009f20: 6469 7361 626c 653d 756e 7375 6273 6372  disable=unsubscr
-00009f30: 6970 7461 626c 652d 6f62 6a65 6374 0a20  iptable-object. 
-00009f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009f20: 2020 2320 7079 6c69 6e74 3a20 6469 7361    # pylint: disa
+00009f30: 626c 653d 756e 7375 6273 6372 6970 7461  ble=unsubscripta
+00009f40: 626c 652d 6f62 6a65 6374 0a20 2020 2020  ble-object.     
 00009f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f60: 2020 2069 6620 706c 6179 6572 5f6f 7574     if player_out
-00009f70: 7075 742e 7072 6f6d 7074 696e 675b 0a20  put.prompting[. 
-00009f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009f60: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00009f70: 6620 706c 6179 6572 5f6f 7574 7075 742e  f player_output.
+00009f80: 7072 6f6d 7074 696e 675b 0a20 2020 2020  prompting[.     
 00009f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009fa0: 2020 2020 2020 2030 0a20 2020 2020 2020         0.       
-00009fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009fc0: 2020 2020 2020 2020 2020 2020 205d 2e69               ].i
-00009fd0: 736e 756d 6572 6963 2829 2061 6e64 2070  snumeric() and p
-00009fe0: 6c61 7965 725f 6f75 7470 7574 2e70 726f  layer_output.pro
-00009ff0: 6d70 7469 6e67 5b0a 2020 2020 2020 2020  mpting[.        
-0000a000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009fb0: 2020 2030 0a20 2020 2020 2020 2020 2020     0.           
+00009fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009fd0: 2020 2020 2020 2020 205d 2e69 736e 756d           ].isnum
+00009fe0: 6572 6963 2829 2061 6e64 2070 6c61 7965  eric() and playe
+00009ff0: 725f 6f75 7470 7574 2e70 726f 6d70 7469  r_output.prompti
+0000a000: 6e67 5b0a 2020 2020 2020 2020 2020 2020  ng[.            
 0000a010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a020: 320a 2020 2020 2020 2020 2020 2020 2020  2.              
+0000a020: 2020 2020 2020 2020 2020 2020 320a 2020              2.  
 0000a030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a040: 2020 2020 2020 5d20 696e 2028 0a20 2020        ] in (.   
-0000a050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a050: 2020 5d20 696e 2028 0a20 2020 2020 2020    ] in (.       
 0000a060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a070: 2020 2020 2050 524f 4d50 545f 4d4f 4445       PROMPT_MODE
-0000a080: 535b 2261 6464 225d 2c0a 2020 2020 2020  S["add"],.      
-0000a090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a080: 2050 524f 4d50 545f 4d4f 4445 535b 2261   PROMPT_MODES["a
+0000a090: 6464 225d 2c0a 2020 2020 2020 2020 2020  dd"],.          
 0000a0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a0b0: 2020 5052 4f4d 5054 5f4d 4f44 4553 5b22    PROMPT_MODES["
-0000a0c0: 696e 7365 7274 225d 2c0a 2020 2020 2020  insert"],.      
-0000a0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a0e0: 2020 2020 2020 2020 2020 2020 2020 293a                ):
-0000a0f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a0b0: 2020 2020 2020 2020 2020 2020 2020 5052                PR
+0000a0c0: 4f4d 5054 5f4d 4f44 4553 5b22 696e 7365  OMPT_MODES["inse
+0000a0d0: 7274 225d 2c0a 2020 2020 2020 2020 2020  rt"],.          
+0000a0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a0f0: 2020 2020 2020 2020 2020 293a 0a20 2020            ):.   
 0000a100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a110: 2020 2020 2020 2020 2066 6f72 2064 6574           for det
-0000a120: 6169 6c73 2069 6e20 706c 6179 6572 5f6f  ails in player_o
-0000a130: 7574 7075 742e 706c 6179 6c69 7374 3a0a  utput.playlist:.
-0000a140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a120: 2020 2020 2066 6f72 2064 6574 6169 6c73       for details
+0000a130: 2069 6e20 706c 6179 6572 5f6f 7574 7075   in player_outpu
+0000a140: 742e 706c 6179 6c69 7374 3a0a 2020 2020  t.playlist:.    
 0000a150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a160: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-0000a170: 6e74 2864 6574 6169 6c73 5b30 5d29 203d  nt(details[0]) =
-0000a180: 3d20 696e 7428 0a20 2020 2020 2020 2020  = int(.         
-0000a190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a170: 2020 2020 2020 2020 6966 2069 6e74 2864          if int(d
+0000a180: 6574 6169 6c73 5b30 5d29 203d 3d20 696e  etails[0]) == in
+0000a190: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
 0000a1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a1b0: 2020 2020 2020 2070 6c61 7965 725f 6f75         player_ou
-0000a1c0: 7470 7574 2e70 726f 6d70 7469 6e67 5b30  tput.prompting[0
-0000a1d0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+0000a1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a1c0: 2020 2070 6c61 7965 725f 6f75 7470 7574     player_output
+0000a1d0: 2e70 726f 6d70 7469 6e67 5b30 5d0a 2020  .prompting[0].  
 0000a1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a1f0: 2020 2020 2020 2020 2020 2020 2020 293a                ):
-0000a200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a200: 2020 2020 2020 2020 2020 293a 0a20 2020            ):.   
 0000a210: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a230: 2062 7265 616b 0a20 2020 2020 2020 2020   break.         
-0000a240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a250: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000a260: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000a270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a230: 2020 2020 2020 2020 2020 2020 2062 7265               bre
+0000a240: 616b 0a20 2020 2020 2020 2020 2020 2020  ak.             
+0000a250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a260: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0000a270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000a280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a290: 2077 6974 6820 6f70 656e 280a 2020 2020   with open(.    
-0000a2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a290: 2020 2020 2020 2020 2020 2020 2077 6974               wit
+0000a2a0: 6820 6f70 656e 280a 2020 2020 2020 2020  h open(.        
 0000a2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a2c0: 2020 2020 2020 2020 2020 2020 534f 4e47              SONG
-0000a2d0: 535f 494e 464f 5f50 4154 482c 0a20 2020  S_INFO_PATH,.   
-0000a2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a2d0: 2020 2020 2020 2020 534f 4e47 535f 494e          SONGS_IN
+0000a2e0: 464f 5f50 4154 482c 0a20 2020 2020 2020  FO_PATH,.       
 0000a2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a300: 2020 2020 2020 2020 2020 2020 2022 7222               "r"
-0000a310: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000a300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a310: 2020 2020 2020 2020 2022 7222 2c0a 2020           "r",.  
 0000a320: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a340: 2020 656e 636f 6469 6e67 3d22 7574 662d    encoding="utf-
-0000a350: 3822 2c0a 2020 2020 2020 2020 2020 2020  8",.            
+0000a340: 2020 2020 2020 2020 2020 2020 2020 656e                en
+0000a350: 636f 6469 6e67 3d22 7574 662d 3822 2c0a  coding="utf-8",.
 0000a360: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a380: 2920 6173 2073 6f6e 6773 5f66 696c 653a  ) as songs_file:
-0000a390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a380: 2020 2020 2020 2020 2020 2020 2920 6173              ) as
+0000a390: 2073 6f6e 6773 5f66 696c 653a 0a20 2020   songs_file:.   
 0000a3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a3c0: 2066 6f72 206c 696e 6520 696e 2073 6f6e   for line in son
-0000a3d0: 6773 5f66 696c 653a 0a20 2020 2020 2020  gs_file:.       
-0000a3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a3c0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0000a3d0: 206c 696e 6520 696e 2073 6f6e 6773 5f66   line in songs_f
+0000a3e0: 696c 653a 0a20 2020 2020 2020 2020 2020  ile:.           
 0000a3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a400: 2020 2020 2020 2020 2020 2020 2064 6574               det
-0000a410: 6169 6c73 203d 2028 0a20 2020 2020 2020  ails = (.       
-0000a420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a410: 2020 2020 2020 2020 2064 6574 6169 6c73           details
+0000a420: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
 0000a430: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a450: 206c 696e 652e 7374 7269 7028 292e 7370   line.strip().sp
-0000a460: 6c69 7428 227c 2229 0a20 2020 2020 2020  lit("|").       
-0000a470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a450: 2020 2020 2020 2020 2020 2020 206c 696e               lin
+0000a460: 652e 7374 7269 7028 292e 7370 6c69 7428  e.strip().split(
+0000a470: 227c 2229 0a20 2020 2020 2020 2020 2020  "|").           
 0000a480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a490: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-0000a4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a4a0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
 0000a4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a4d0: 2020 2073 6f6e 675f 6964 203d 2069 6e74     song_id = int
-0000a4e0: 2864 6574 6169 6c73 5b30 5d29 0a20 2020  (details[0]).   
-0000a4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a4d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000a4e0: 6f6e 675f 6964 203d 2069 6e74 2864 6574  ong_id = int(det
+0000a4f0: 6169 6c73 5b30 5d29 0a20 2020 2020 2020  ails[0]).       
 0000a500: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a520: 2069 6620 736f 6e67 5f69 6420 3d3d 2069   if song_id == i
-0000a530: 6e74 280a 2020 2020 2020 2020 2020 2020  nt(.            
+0000a520: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000a530: 736f 6e67 5f69 6420 3d3d 2069 6e74 280a  song_id == int(.
 0000a540: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a560: 2020 2020 2020 2020 2020 2020 706c 6179              play
-0000a570: 6572 5f6f 7574 7075 742e 7072 6f6d 7074  er_output.prompt
-0000a580: 696e 675b 0a20 2020 2020 2020 2020 2020  ing[.           
-0000a590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a570: 2020 2020 2020 2020 706c 6179 6572 5f6f          player_o
+0000a580: 7574 7075 742e 7072 6f6d 7074 696e 675b  utput.prompting[
+0000a590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000a5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5c0: 2030 0a20 2020 2020 2020 2020 2020 2020   0.             
+0000a5c0: 2020 2020 2020 2020 2020 2020 2030 0a20               0. 
 0000a5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5f0: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
-0000a600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a600: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
 0000a610: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a630: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
+0000a630: 2020 2020 2020 2020 2020 2020 2029 3a0a               ):.
 0000a640: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a660: 2020 2020 2020 2020 2020 2020 736f 6e67              song
-0000a670: 5f64 6174 6120 3d20 280a 2020 2020 2020  _data = (.      
-0000a680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a670: 2020 2020 2020 2020 736f 6e67 5f64 6174          song_dat
+0000a680: 6120 3d20 280a 2020 2020 2020 2020 2020  a = (.          
 0000a690: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a6b0: 2020 2020 2020 6d75 7369 635f 7461 672e        music_tag.
-0000a6c0: 6c6f 6164 5f66 696c 6528 0a20 2020 2020  load_file(.     
-0000a6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a6c0: 2020 6d75 7369 635f 7461 672e 6c6f 6164    music_tag.load
+0000a6d0: 5f66 696c 6528 0a20 2020 2020 2020 2020  _file(.         
 0000a6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a700: 2020 2020 2020 2020 2020 206f 732e 7061             os.pa
-0000a710: 7468 2e6a 6f69 6e28 0a20 2020 2020 2020  th.join(.       
-0000a720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a710: 2020 2020 2020 206f 732e 7061 7468 2e6a         os.path.j
+0000a720: 6f69 6e28 0a20 2020 2020 2020 2020 2020  oin(.           
 0000a730: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a750: 2020 2020 2020 2020 2020 2020 2053 4f4e               SON
-0000a760: 4753 5f44 4952 2c0a 2020 2020 2020 2020  GS_DIR,.        
-0000a770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a760: 2020 2020 2020 2020 2053 4f4e 4753 5f44           SONGS_D
+0000a770: 4952 2c0a 2020 2020 2020 2020 2020 2020  IR,.            
 0000a780: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a7a0: 2020 2020 2020 2020 2020 2020 6465 7461              deta
-0000a7b0: 696c 735b 315d 2c0a 2020 2020 2020 2020  ils[1],.        
-0000a7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a7b0: 2020 2020 2020 2020 6465 7461 696c 735b          details[
+0000a7c0: 315d 2c0a 2020 2020 2020 2020 2020 2020  1],.            
 0000a7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a7f0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000a800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a800: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
 0000a810: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a830: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0000a840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a840: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
 0000a850: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a870: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000a870: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
 0000a880: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a8a0: 2020 2020 2020 2020 2020 6465 7461 696c            detail
-0000a8b0: 7320 2b3d 205b 0a20 2020 2020 2020 2020  s += [.         
-0000a8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a8b0: 2020 2020 2020 6465 7461 696c 7320 2b3d        details +=
+0000a8c0: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
 0000a8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a8f0: 2020 2028 0a20 2020 2020 2020 2020 2020     (.           
-0000a900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a8f0: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+0000a900: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000a910: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a930: 2020 2020 2073 6f6e 675f 6461 7461 5b0a       song_data[.
-0000a940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a940: 2073 6f6e 675f 6461 7461 5b0a 2020 2020   song_data[.    
 0000a950: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a960: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a980: 2020 2020 2261 7274 6973 7422 0a20 2020      "artist".   
-0000a990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a990: 2261 7274 6973 7422 0a20 2020 2020 2020  "artist".       
 0000a9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a9c0: 2020 2020 2020 2020 2020 2020 205d 2e76               ].v
-0000a9d0: 616c 7565 0a20 2020 2020 2020 2020 2020  alue.           
-0000a9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a9d0: 2020 2020 2020 2020 205d 2e76 616c 7565           ].value
+0000a9e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000a9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000aa00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aa10: 2020 2020 206f 7220 2255 6e6b 6e6f 776e       or "Unknown
-0000aa20: 2041 7274 6973 7422 0a20 2020 2020 2020   Artist".       
-0000aa30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa20: 206f 7220 2255 6e6b 6e6f 776e 2041 7274   or "Unknown Art
+0000aa30: 6973 7422 0a20 2020 2020 2020 2020 2020  ist".           
 0000aa40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000aa50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aa60: 2020 2020 2029 2c0a 2020 2020 2020 2020       ),.        
-0000aa70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa70: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
 0000aa80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000aa90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aaa0: 2020 2020 280a 2020 2020 2020 2020 2020      (.          
-0000aab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aaa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aab0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
 0000aac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000aad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aae0: 2020 2020 2020 736f 6e67 5f64 6174 615b        song_data[
-0000aaf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000aae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aaf0: 2020 736f 6e67 5f64 6174 615b 0a20 2020    song_data[.   
 0000ab00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ab10: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ab20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab30: 2020 2020 2022 616c 6275 6d22 0a20 2020       "album".   
-0000ab40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab40: 2022 616c 6275 6d22 0a20 2020 2020 2020   "album".       
 0000ab50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ab60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab70: 2020 2020 2020 2020 2020 2020 205d 2e76               ].v
-0000ab80: 616c 7565 0a20 2020 2020 2020 2020 2020  alue.           
-0000ab90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab80: 2020 2020 2020 2020 205d 2e76 616c 7565           ].value
+0000ab90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000aba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000abb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000abc0: 2020 2020 206f 7220 2255 6e6b 6e6f 776e       or "Unknown
-0000abd0: 2041 6c62 756d 220a 2020 2020 2020 2020   Album".        
-0000abe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000abc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000abd0: 206f 7220 2255 6e6b 6e6f 776e 2041 6c62   or "Unknown Alb
+0000abe0: 756d 220a 2020 2020 2020 2020 2020 2020  um".            
 0000abf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ac00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac10: 2020 2020 292c 0a20 2020 2020 2020 2020      ),.         
-0000ac20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac20: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
 0000ac30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ac40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac50: 2020 2028 0a20 2020 2020 2020 2020 2020     (.           
-0000ac60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac50: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+0000ac60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000ac70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ac80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac90: 2020 2020 2073 6f6e 675f 6461 7461 5b0a       song_data[.
-0000aca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aca0: 2073 6f6e 675f 6461 7461 5b0a 2020 2020   song_data[.    
 0000acb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000acc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000acd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ace0: 2020 2020 2261 6c62 756d 6172 7469 7374      "albumartist
-0000acf0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0000ace0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000acf0: 2261 6c62 756d 6172 7469 7374 220a 2020  "albumartist".  
 0000ad00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ad10: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ad20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad30: 2020 5d2e 7661 6c75 650a 2020 2020 2020    ].value.      
-0000ad40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ad30: 2020 2020 2020 2020 2020 2020 2020 5d2e                ].
+0000ad40: 7661 6c75 650a 2020 2020 2020 2020 2020  value.          
 0000ad50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ad60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad70: 2020 2020 2020 2020 2020 6f72 2022 556e            or "Un
-0000ad80: 6b6e 6f77 6e20 416c 6275 6d20 4172 7469  known Album Arti
-0000ad90: 7374 220a 2020 2020 2020 2020 2020 2020  st".            
+0000ad70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ad80: 2020 2020 2020 6f72 2022 556e 6b6e 6f77        or "Unknow
+0000ad90: 6e20 416c 6275 6d20 4172 7469 7374 220a  n Album Artist".
 0000ada0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000adb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000adc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000add0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+0000add0: 2020 2020 2020 2020 2020 2020 292c 0a20              ),. 
 0000ade0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000adf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae00: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
-0000ae10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae10: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
 0000ae20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ae30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae40: 2020 2020 2069 6620 280a 2020 2020 2020       if (.      
-0000ae50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae50: 2069 6620 280a 2020 2020 2020 2020 2020   if (.          
 0000ae60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ae70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae80: 2020 2020 2020 706c 6179 6572 5f6f 7574        player_out
-0000ae90: 7075 742e 7072 6f6d 7074 696e 675b 0a20  put.prompting[. 
-0000aea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae90: 2020 706c 6179 6572 5f6f 7574 7075 742e    player_output.
+0000aea0: 7072 6f6d 7074 696e 675b 0a20 2020 2020  prompting[.     
 0000aeb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000aec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aed0: 2020 2020 2020 2020 2020 2020 2020 2032                 2
-0000aee0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000aed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aee0: 2020 2020 2020 2020 2020 2032 0a20 2020             2.   
 0000aef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000af00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af10: 2020 2020 2020 2020 2020 2020 205d 0a20               ]. 
-0000af20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000af10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000af20: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
 0000af30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000af40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af50: 2020 2020 2020 2020 2020 203d 3d20 5052             == PR
-0000af60: 4f4d 5054 5f4d 4f44 4553 5b0a 2020 2020  OMPT_MODES[.    
-0000af70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000af50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000af60: 2020 2020 2020 203d 3d20 5052 4f4d 5054         == PROMPT
+0000af70: 5f4d 4f44 4553 5b0a 2020 2020 2020 2020  _MODES[.        
 0000af80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000af90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000afa0: 2020 2020 2020 2020 2020 2020 2269 6e73              "ins
-0000afb0: 6572 7422 0a20 2020 2020 2020 2020 2020  ert".           
-0000afc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000afa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000afb0: 2020 2020 2020 2020 2269 6e73 6572 7422          "insert"
+0000afc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000afd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000afe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aff0: 205d 0a20 2020 2020 2020 2020 2020 2020   ].             
+0000aff0: 2020 2020 2020 2020 2020 2020 205d 0a20               ]. 
 0000b000: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b020: 2020 2020 2020 2020 2020 2029 3a0a 2020             ):.  
-0000b030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b030: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
 0000b040: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b060: 2020 2020 2020 2020 2020 706c 6179 6572            player
-0000b070: 5f6f 7574 7075 742e 706c 6179 6c69 7374  _output.playlist
-0000b080: 2e69 6e73 6572 7428 0a20 2020 2020 2020  .insert(.       
-0000b090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b070: 2020 2020 2020 706c 6179 6572 5f6f 7574        player_out
+0000b080: 7075 742e 706c 6179 6c69 7374 2e69 6e73  put.playlist.ins
+0000b090: 6572 7428 0a20 2020 2020 2020 2020 2020  ert(.           
 0000b0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b0c0: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
-0000b0d0: 6f75 7470 7574 2e73 6372 6f6c 6c65 722e  output.scroller.
-0000b0e0: 706f 730a 2020 2020 2020 2020 2020 2020  pos.            
+0000b0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b0d0: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
+0000b0e0: 7574 2e73 6372 6f6c 6c65 722e 706f 730a  ut.scroller.pos.
 0000b0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b100: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b120: 2020 2020 2b20 312c 0a20 2020 2020 2020      + 1,.       
-0000b130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b130: 2b20 312c 0a20 2020 2020 2020 2020 2020  + 1,.           
 0000b140: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b160: 2020 2020 2020 2020 2064 6574 6169 6c73           details
-0000b170: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000b160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b170: 2020 2020 2064 6574 6169 6c73 2c0a 2020       details,.  
 0000b180: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b1a0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-0000b1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b1b0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
 0000b1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b1e0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000b1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b1f0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
 0000b200: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b220: 2020 2020 2020 2020 2020 706c 6179 6572            player
-0000b230: 5f6f 7574 7075 742e 706c 6179 6c69 7374  _output.playlist
-0000b240: 2e61 7070 656e 6428 0a20 2020 2020 2020  .append(.       
-0000b250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b230: 2020 2020 2020 706c 6179 6572 5f6f 7574        player_out
+0000b240: 7075 742e 706c 6179 6c69 7374 2e61 7070  put.playlist.app
+0000b250: 656e 6428 0a20 2020 2020 2020 2020 2020  end(.           
 0000b260: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b280: 2020 2020 2020 2020 2064 6574 6169 6c73           details
-0000b290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b290: 2020 2020 2064 6574 6169 6c73 0a20 2020       details.   
 0000b2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b2c0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-0000b2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b2d0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
 0000b2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b300: 2020 2020 2020 2069 6620 6c6f 6f70 3a0a         if loop:.
-0000b310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b310: 2020 2069 6620 6c6f 6f70 3a0a 2020 2020     if loop:.    
 0000b320: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b340: 2020 2020 2020 2020 2020 2020 6966 2072              if r
-0000b350: 6573 6875 6666 6c65 3a0a 2020 2020 2020  eshuffle:.      
-0000b360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b350: 2020 2020 2020 2020 6966 2072 6573 6875          if reshu
+0000b360: 6666 6c65 3a0a 2020 2020 2020 2020 2020  ffle:.          
 0000b370: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b390: 2020 2020 2020 2020 2020 6e65 7874 5f70            next_p
-0000b3a0: 6c61 796c 6973 742e 696e 7365 7274 280a  laylist.insert(.
-0000b3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b3a0: 2020 2020 2020 6e65 7874 5f70 6c61 796c        next_playl
+0000b3b0: 6973 742e 696e 7365 7274 280a 2020 2020  ist.insert(.    
 0000b3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b3f0: 2020 2020 7261 6e64 696e 7428 0a20 2020      randint(.   
-0000b400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b400: 7261 6e64 696e 7428 0a20 2020 2020 2020  randint(.       
 0000b410: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b420: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b440: 2020 2020 2030 2c0a 2020 2020 2020 2020       0,.        
-0000b450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b450: 2030 2c0a 2020 2020 2020 2020 2020 2020   0,.            
 0000b460: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b470: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b490: 6c65 6e28 0a20 2020 2020 2020 2020 2020  len(.           
-0000b4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b490: 2020 2020 2020 2020 2020 2020 6c65 6e28              len(
+0000b4a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000b4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b4e0: 206e 6578 745f 706c 6179 6c69 7374 0a20   next_playlist. 
-0000b4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b4e0: 2020 2020 2020 2020 2020 2020 206e 6578               nex
+0000b4f0: 745f 706c 6179 6c69 7374 0a20 2020 2020  t_playlist.     
 0000b500: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b510: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b530: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000b540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b540: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
 0000b550: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b560: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b580: 202d 2031 2c0a 2020 2020 2020 2020 2020   - 1,.          
-0000b590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b580: 2020 2020 2020 2020 2020 2020 202d 2031               - 1
+0000b590: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
 0000b5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b5c0: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
-0000b5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b5d0: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
 0000b5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b610: 2064 6574 6169 6c73 2c0a 2020 2020 2020   details,.      
-0000b620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b610: 2020 2020 2020 2020 2020 2020 2064 6574               det
+0000b620: 6169 6c73 2c0a 2020 2020 2020 2020 2020  ails,.          
 0000b630: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b650: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0000b660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b660: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
 0000b670: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b690: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000b6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b6a0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
 0000b6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b6d0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000b6e0: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+0000b6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b6e0: 2020 2020 2020 2020 2020 6966 2028 0a20            if (. 
 0000b6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b700: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b720: 2020 2020 2020 2070 6c61 7965 725f 6f75         player_ou
-0000b730: 7470 7574 2e70 726f 6d70 7469 6e67 5b0a  tput.prompting[.
-0000b740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b730: 2020 2070 6c61 7965 725f 6f75 7470 7574     player_output
+0000b740: 2e70 726f 6d70 7469 6e67 5b0a 2020 2020  .prompting[.    
 0000b750: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b760: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b780: 2020 2020 2020 2020 320a 2020 2020 2020          2.      
-0000b790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b790: 2020 2020 320a 2020 2020 2020 2020 2020      2.          
 0000b7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b7c0: 2020 2020 2020 2020 2020 2020 2020 5d0a                ].
-0000b7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b7d0: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
 0000b7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b810: 2020 2020 3d3d 2050 524f 4d50 545f 4d4f      == PROMPT_MO
-0000b820: 4445 535b 0a20 2020 2020 2020 2020 2020  DES[.           
-0000b830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b820: 3d3d 2050 524f 4d50 545f 4d4f 4445 535b  == PROMPT_MODES[
+0000b830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000b840: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b860: 2020 2020 2020 2020 2020 2020 2022 696e               "in
-0000b870: 7365 7274 220a 2020 2020 2020 2020 2020  sert".          
-0000b880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b870: 2020 2020 2020 2020 2022 696e 7365 7274           "insert
+0000b880: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
 0000b890: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b8b0: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
-0000b8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b8c0: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
 0000b8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b8f0: 2020 2020 2020 2020 2020 2020 293a 0a20              ):. 
-0000b900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b900: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
 0000b910: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b920: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b940: 2020 206e 6578 745f 706c 6179 6c69 7374     next_playlist
-0000b950: 2e69 6e73 6572 7428 0a20 2020 2020 2020  .insert(.       
-0000b960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b940: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+0000b950: 6578 745f 706c 6179 6c69 7374 2e69 6e73  ext_playlist.ins
+0000b960: 6572 7428 0a20 2020 2020 2020 2020 2020  ert(.           
 0000b970: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b980: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b9a0: 2070 6c61 7965 725f 6f75 7470 7574 2e73   player_output.s
-0000b9b0: 6372 6f6c 6c65 722e 706f 730a 2020 2020  croller.pos.    
-0000b9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b9a0: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
+0000b9b0: 7965 725f 6f75 7470 7574 2e73 6372 6f6c  yer_output.scrol
+0000b9c0: 6c65 722e 706f 730a 2020 2020 2020 2020  ler.pos.        
 0000b9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba00: 2020 2020 2b20 312c 0a20 2020 2020 2020      + 1,.       
-0000ba10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba10: 2b20 312c 0a20 2020 2020 2020 2020 2020  + 1,.           
 0000ba20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ba30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ba40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba50: 2064 6574 6169 6c73 2c0a 2020 2020 2020   details,.      
-0000ba60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba50: 2020 2020 2020 2020 2020 2020 2064 6574               det
+0000ba60: 6169 6c73 2c0a 2020 2020 2020 2020 2020  ails,.          
 0000ba70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ba80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba90: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-0000baa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000baa0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
 0000bab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bae0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000baf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bae0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+0000baf0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
 0000bb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb20: 2020 2020 2020 2020 2020 6e65 7874 5f70            next_p
-0000bb30: 6c61 796c 6973 742e 6170 7065 6e64 280a  laylist.append(.
-0000bb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb30: 2020 2020 2020 6e65 7874 5f70 6c61 796c        next_playl
+0000bb40: 6973 742e 6170 7065 6e64 280a 2020 2020  ist.append(.    
 0000bb50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bb70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb80: 2020 2020 2020 2020 6465 7461 696c 730a          details.
-0000bb90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb90: 2020 2020 6465 7461 696c 730a 2020 2020      details.    
 0000bba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bbd0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-0000bbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bbe0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
 0000bbf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc00: 2020 2020 2020 2020 2020 2020 2020 706c                pl
-0000bc10: 6179 6572 5f6f 7574 7075 742e 7363 726f  ayer_output.scro
-0000bc20: 6c6c 6572 2e6e 756d 5f6c 696e 6573 202b  ller.num_lines +
-0000bc30: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+0000bc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc10: 2020 2020 2020 2020 2020 706c 6179 6572            player
+0000bc20: 5f6f 7574 7075 742e 7363 726f 6c6c 6572  _output.scroller
+0000bc30: 2e6e 756d 5f6c 696e 6573 202b 3d20 280a  .num_lines += (.
 0000bc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc70: 310a 2020 2020 2020 2020 2020 2020 2020  1.              
+0000bc70: 2020 2020 2020 2020 2020 2020 310a 2020              1.  
 0000bc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bca0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0000bcb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bcb0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
 0000bcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bce0: 2020 2020 706c 6179 6572 5f6f 7574 7075      player_outpu
-0000bcf0: 742e 7072 6f6d 7074 696e 6720 3d20 280a  t.prompting = (.
-0000bd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bcf0: 706c 6179 6572 5f6f 7574 7075 742e 7072  player_output.pr
+0000bd00: 6f6d 7074 696e 6720 3d20 280a 2020 2020  ompting = (.    
 0000bd10: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd30: 2020 2020 2020 2020 2020 2020 4e6f 6e65              None
-0000bd40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bd40: 2020 2020 2020 2020 4e6f 6e65 0a20 2020          None.   
 0000bd50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd70: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0000bd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bd70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bd80: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
 0000bd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bdb0: 2020 2063 7572 7365 732e 6375 7273 5f73     curses.curs_s
-0000bdc0: 6574 2846 616c 7365 290a 2020 2020 2020  et(False).      
-0000bdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bdb0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000bdc0: 7572 7365 732e 6375 7273 5f73 6574 2846  urses.curs_set(F
+0000bdd0: 616c 7365 290a 2020 2020 2020 2020 2020  alse).          
 0000bde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be00: 2020 706c 6179 6572 5f6f 7574 7075 742e    player_output.
-0000be10: 7363 726f 6c6c 6572 2e72 6573 697a 6528  scroller.resize(
-0000be20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000be00: 2020 2020 2020 2020 2020 2020 2020 706c                pl
+0000be10: 6179 6572 5f6f 7574 7075 742e 7363 726f  ayer_output.scro
+0000be20: 6c6c 6572 2e72 6573 697a 6528 0a20 2020  ller.resize(.   
 0000be30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000be40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be50: 2020 2020 2020 2020 2020 2020 2073 6372               scr
-0000be60: 6565 6e5f 7369 7a65 5b30 5d20 2d20 320a  een_size[0] - 2.
-0000be70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000be50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000be60: 2020 2020 2020 2020 2073 6372 6565 6e5f           screen_
+0000be70: 7369 7a65 5b30 5d20 2d20 320a 2020 2020  size[0] - 2.    
 0000be80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000be90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bea0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000beb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000beb0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
 0000bec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bee0: 2020 706c 6179 6572 5f6f 7574 7075 742e    player_output.
-0000bef0: 6f75 7470 7574 280a 2020 2020 2020 2020  output(.        
-0000bf00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bee0: 2020 2020 2020 2020 2020 2020 2020 706c                pl
+0000bef0: 6179 6572 5f6f 7574 7075 742e 6f75 7470  ayer_output.outp
+0000bf00: 7574 280a 2020 2020 2020 2020 2020 2020  ut(.            
 0000bf10: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bf20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf30: 2020 2020 706c 6179 6261 636b 2e63 7572      playback.cur
-0000bf40: 725f 706f 730a 2020 2020 2020 2020 2020  r_pos.          
-0000bf50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf40: 706c 6179 6261 636b 2e63 7572 725f 706f  playback.curr_po
+0000bf50: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
 0000bf60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf70: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-0000bf80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf80: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
 0000bf90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bfb0: 2020 2020 2020 2020 6272 6561 6b0a 2020          break.  
-0000bfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bfb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bfc0: 2020 2020 6272 6561 6b0a 2020 2020 2020      break.      
 0000bfd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bfe0: 2020 656c 6966 2028 0a20 2020 2020 2020    elif (.       
-0000bff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bfe0: 2020 2020 2020 2020 2020 2020 2020 656c                el
+0000bff0: 6966 2028 0a20 2020 2020 2020 2020 2020  if (.           
 0000c000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c010: 2022 7c22 206e 6f74 2069 6e20 706c 6179   "|" not in play
-0000c020: 6572 5f6f 7574 7075 742e 7072 6f6d 7074  er_output.prompt
-0000c030: 696e 675b 305d 0a20 2020 2020 2020 2020  ing[0].         
-0000c040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c050: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0000c060: 6e64 2070 6c61 7965 725f 6f75 7470 7574  nd player_output
-0000c070: 2e70 726f 6d70 7469 6e67 5b32 5d0a 2020  .prompting[2].  
-0000c080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c010: 2020 2020 2020 2020 2020 2020 2022 7c22               "|"
+0000c020: 206e 6f74 2069 6e20 706c 6179 6572 5f6f   not in player_o
+0000c030: 7574 7075 742e 7072 6f6d 7074 696e 675b  utput.prompting[
+0000c040: 305d 0a20 2020 2020 2020 2020 2020 2020  0].             
+0000c050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c060: 2020 2020 2020 2020 2020 2061 6e64 2070             and p
+0000c070: 6c61 7965 725f 6f75 7470 7574 2e70 726f  layer_output.pro
+0000c080: 6d70 7469 6e67 5b32 5d0a 2020 2020 2020  mpting[2].      
 0000c090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c0a0: 2020 2020 2020 3d3d 2050 524f 4d50 545f        == PROMPT_
-0000c0b0: 4d4f 4445 535b 2274 6167 225d 0a20 2020  MODES["tag"].   
-0000c0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c0b0: 2020 3d3d 2050 524f 4d50 545f 4d4f 4445    == PROMPT_MODE
+0000c0c0: 535b 2274 6167 225d 0a20 2020 2020 2020  S["tag"].       
 0000c0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c0e0: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
+0000c0e0: 2020 2020 2020 2020 2020 2020 2029 3a0a               ):.
 0000c0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c100: 2020 2020 2020 2020 2020 2020 7461 6773              tags
-0000c110: 203d 2070 6c61 7965 725f 6f75 7470 7574   = player_output
-0000c120: 2e70 726f 6d70 7469 6e67 5b30 5d2e 7370  .prompting[0].sp
-0000c130: 6c69 7428 0a20 2020 2020 2020 2020 2020  lit(.           
-0000c140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c110: 2020 2020 2020 2020 7461 6773 203d 2070          tags = p
+0000c120: 6c61 7965 725f 6f75 7470 7574 2e70 726f  layer_output.pro
+0000c130: 6d70 7469 6e67 5b30 5d2e 7370 6c69 7428  mpting[0].split(
+0000c140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000c150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c160: 2022 2c22 0a20 2020 2020 2020 2020 2020   ",".           
-0000c170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c180: 2020 2020 2020 2020 2020 2020 2029 0a0a               )..
-0000c190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c160: 2020 2020 2020 2020 2020 2020 2022 2c22               ","
+0000c170: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c190: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
 0000c1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c1b0: 2020 2020 2020 2020 7461 6767 696e 675f          tagging_
-0000c1c0: 6964 7320 3d20 7b7d 0a20 2020 2020 2020  ids = {}.       
-0000c1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c1c0: 2020 2020 7461 6767 696e 675f 6964 7320      tagging_ids 
+0000c1d0: 3d20 7b7d 0a20 2020 2020 2020 2020 2020  = {}.           
 0000c1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c1f0: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-0000c200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c1f0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0000c200: 2069 2069 6e20 7261 6e67 6528 0a20 2020   i in range(.   
 0000c210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c220: 2020 2020 2020 2020 2020 2020 206c 656e               len
-0000c230: 2870 6c61 7965 725f 6f75 7470 7574 2e70  (player_output.p
-0000c240: 6c61 796c 6973 7429 0a20 2020 2020 2020  laylist).       
-0000c250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c230: 2020 2020 2020 2020 206c 656e 2870 6c61           len(pla
+0000c240: 7965 725f 6f75 7470 7574 2e70 6c61 796c  yer_output.playl
+0000c250: 6973 7429 0a20 2020 2020 2020 2020 2020  ist).           
 0000c260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c270: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
+0000c270: 2020 2020 2020 2020 2020 2020 2029 3a0a               ):.
 0000c280: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000c290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c2a0: 7461 6767 696e 675f 6964 735b 0a20 2020  tagging_ids[.   
-0000c2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c2a0: 2020 2020 2020 2020 2020 2020 7461 6767              tagg
+0000c2b0: 696e 675f 6964 735b 0a20 2020 2020 2020  ing_ids[.       
 0000c2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c2d0: 2020 2020 2020 2020 2020 2020 2069 6e74               int
-0000c2e0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000c2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c2e0: 2020 2020 2020 2020 2069 6e74 280a 2020           int(.  
 0000c2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000c300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c310: 2020 2020 2020 706c 6179 6572 5f6f 7574        player_out
-0000c320: 7075 742e 706c 6179 6c69 7374 5b69 5d5b  put.playlist[i][
-0000c330: 305d 0a20 2020 2020 2020 2020 2020 2020  0].             
+0000c310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c320: 2020 706c 6179 6572 5f6f 7574 7075 742e    player_output.
+0000c330: 706c 6179 6c69 7374 5b69 5d5b 305d 0a20  playlist[i][0]. 
 0000c340: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000c350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c360: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-0000c370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c360: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+0000c370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000c380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c390: 205d 203d 2069 0a0a 2020 2020 2020 2020   ] = i..        
-0000c3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c390: 2020 2020 2020 2020 2020 2020 205d 203d               ] =
+0000c3a0: 2069 0a0a 2020 2020 2020 2020 2020 2020   i..            
 0000c3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c3c0: 736f 6e67 735f 6669 6c65 203d 206f 7065  songs_file = ope
-0000c3d0: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
+0000c3c0: 2020 2020 2020 2020 2020 2020 736f 6e67              song
+0000c3d0: 735f 6669 6c65 203d 206f 7065 6e28 0a20  s_file = open(. 
 0000c3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c3f0: 2020 2020 2020 2020 2020 2020 2020 2053                 S
-0000c400: 4f4e 4753 5f49 4e46 4f5f 5041 5448 2c0a  ONGS_INFO_PATH,.
-0000c410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c400: 2020 2020 2020 2020 2020 2053 4f4e 4753             SONGS
+0000c410: 5f49 4e46 4f5f 5041 5448 2c0a 2020 2020  _INFO_PATH,.    
 0000c420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c430: 2020 2020 2020 2020 2020 2020 2272 222c              "r",
-0000c440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c440: 2020 2020 2020 2020 2272 222c 0a20 2020          "r",.   
 0000c450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c460: 2020 2020 2020 2020 2020 2020 2065 6e63               enc
-0000c470: 6f64 696e 673d 2275 7466 2d38 222c 0a20  oding="utf-8",. 
-0000c480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c470: 2020 2020 2020 2020 2065 6e63 6f64 696e           encodin
+0000c480: 673d 2275 7466 2d38 222c 0a20 2020 2020  g="utf-8",.     
 0000c490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c4a0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000c4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c4b0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
 0000c4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c4d0: 206c 696e 6573 203d 2073 6f6e 6773 5f66   lines = songs_f
-0000c4e0: 696c 652e 7265 6164 2829 2e73 706c 6974  ile.read().split
-0000c4f0: 6c69 6e65 7328 290a 2020 2020 2020 2020  lines().        
-0000c500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c4d0: 2020 2020 2020 2020 2020 2020 206c 696e               lin
+0000c4e0: 6573 203d 2073 6f6e 6773 5f66 696c 652e  es = songs_file.
+0000c4f0: 7265 6164 2829 2e73 706c 6974 6c69 6e65  read().splitline
+0000c500: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
 0000c510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c520: 666f 7220 6920 696e 2072 616e 6765 286c  for i in range(l
-0000c530: 656e 286c 696e 6573 2929 3a0a 2020 2020  en(lines)):.    
-0000c540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c520: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000c530: 6920 696e 2072 616e 6765 286c 656e 286c  i in range(len(l
+0000c540: 696e 6573 2929 3a0a 2020 2020 2020 2020  ines)):.        
 0000c550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c560: 2020 2020 2020 2020 6465 7461 696c 7320          details 
-0000c570: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+0000c560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c570: 2020 2020 6465 7461 696c 7320 3d20 280a      details = (.
 0000c580: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000c590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c5a0: 2020 2020 6c69 6e65 735b 695d 2e73 7472      lines[i].str
-0000c5b0: 6970 2829 2e73 706c 6974 2822 7c22 290a  ip().split("|").
-0000c5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c5b0: 6c69 6e65 735b 695d 2e73 7472 6970 2829  lines[i].strip()
+0000c5c0: 2e73 706c 6974 2822 7c22 290a 2020 2020  .split("|").    
 0000c5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c5e0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0000c5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c5f0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
 0000c600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c610: 2020 2020 2020 2020 2020 736f 6e67 5f69            song_i
-0000c620: 6420 3d20 696e 7428 6465 7461 696c 735b  d = int(details[
-0000c630: 305d 290a 2020 2020 2020 2020 2020 2020  0]).            
+0000c610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c620: 2020 2020 2020 736f 6e67 5f69 6420 3d20        song_id = 
+0000c630: 696e 7428 6465 7461 696c 735b 305d 290a  int(details[0]).
 0000c640: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000c650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c660: 6966 2073 6f6e 675f 6964 2069 6e20 7461  if song_id in ta
-0000c670: 6767 696e 675f 6964 733a 0a20 2020 2020  gging_ids:.     
-0000c680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c660: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0000c670: 6f6e 675f 6964 2069 6e20 7461 6767 696e  ong_id in taggin
+0000c680: 675f 6964 733a 0a20 2020 2020 2020 2020  g_ids:.         
 0000c690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c6a0: 2020 2020 2020 2020 2020 2069 6620 6465             if de
-0000c6b0: 7461 696c 735b 325d 3a0a 2020 2020 2020  tails[2]:.      
-0000c6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c6b0: 2020 2020 2020 2069 6620 6465 7461 696c         if detail
+0000c6c0: 735b 325d 3a0a 2020 2020 2020 2020 2020  s[2]:.          
 0000c6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c6e0: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
-0000c6f0: 775f 7461 6773 203d 2064 6574 6169 6c73  w_tags = details
-0000c700: 5b32 5d2e 7370 6c69 7428 0a20 2020 2020  [2].split(.     
-0000c710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c6f0: 2020 2020 2020 2020 2020 6e65 775f 7461            new_ta
+0000c700: 6773 203d 2064 6574 6169 6c73 5b32 5d2e  gs = details[2].
+0000c710: 7370 6c69 7428 0a20 2020 2020 2020 2020  split(.         
 0000c720: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000c730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c740: 2020 2022 2c22 0a20 2020 2020 2020 2020     ",".         
-0000c750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c740: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0000c750: 2c22 0a20 2020 2020 2020 2020 2020 2020  ,".             
 0000c760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c770: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0000c780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c780: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
 0000c790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c7a0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-0000c7b0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0000c7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c7b0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
 0000c7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000c7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c7e0: 2020 2020 2020 206e 6577 5f74 6167 7320         new_tags 
-0000c7f0: 3d20 5b5d 0a20 2020 2020 2020 2020 2020  = [].           
-0000c800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c7f0: 2020 206e 6577 5f74 6167 7320 3d20 5b5d     new_tags = []
+0000c800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000c810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c820: 2020 2020 206e 6577 5f74 6167 7320 2b3d       new_tags +=
-0000c830: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
+0000c820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c830: 206e 6577 5f74 6167 7320 2b3d 205b 0a20   new_tags += [. 
 0000c840: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000c850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c860: 2020 2020 2020 2074 6167 0a20 2020 2020         tag.     
-0000c870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c870: 2020 2074 6167 0a20 2020 2020 2020 2020     tag.         
 0000c880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c890: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000c8a0: 6f72 2074 6167 2069 6e20 7461 6773 0a20  or tag in tags. 
-0000c8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c8a0: 2020 2020 2020 2020 2020 2066 6f72 2074             for t
+0000c8b0: 6167 2069 6e20 7461 6773 0a20 2020 2020  ag in tags.     
 0000c8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000c8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c8e0: 2020 2069 6620 7461 6720 6e6f 7420 696e     if tag not in
-0000c8f0: 206e 6577 5f74 6167 730a 2020 2020 2020   new_tags.      
-0000c900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c8e0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000c8f0: 6620 7461 6720 6e6f 7420 696e 206e 6577  f tag not in new
+0000c900: 5f74 6167 730a 2020 2020 2020 2020 2020  _tags.          
 0000c910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c920: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
-0000c930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c930: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
 0000c940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c950: 2020 2020 2020 2020 2020 2020 6465 7461              deta
-0000c960: 696c 735b 325d 203d 2022 2c22 2e6a 6f69  ils[2] = ",".joi
-0000c970: 6e28 6e65 775f 7461 6773 290a 2020 2020  n(new_tags).    
-0000c980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c960: 2020 2020 2020 2020 6465 7461 696c 735b          details[
+0000c970: 325d 203d 2022 2c22 2e6a 6f69 6e28 6e65  2] = ",".join(ne
+0000c980: 775f 7461 6773 290a 2020 2020 2020 2020  w_tags).        
 0000c990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c9a0: 2020 2020 2020 2020 2020 2020 6c69 6e65              line
-0000c9b0: 735b 695d 203d 2022 7c22 2e6a 6f69 6e28  s[i] = "|".join(
-0000c9c0: 6465 7461 696c 7329 0a20 2020 2020 2020  details).       
-0000c9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c9b0: 2020 2020 2020 2020 6c69 6e65 735b 695d          lines[i]
+0000c9c0: 203d 2022 7c22 2e6a 6f69 6e28 6465 7461   = "|".join(deta
+0000c9d0: 696c 7329 0a20 2020 2020 2020 2020 2020  ils).           
 0000c9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c9f0: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
-0000ca00: 6f75 7470 7574 2e70 6c61 796c 6973 745b  output.playlist[
-0000ca10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca00: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
+0000ca10: 7574 2e70 6c61 796c 6973 745b 0a20 2020  ut.playlist[.   
 0000ca20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ca30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca40: 2020 2020 2074 6167 6769 6e67 5f69 6473       tagging_ids
-0000ca50: 5b73 6f6e 675f 6964 5d0a 2020 2020 2020  [song_id].      
-0000ca60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca50: 2074 6167 6769 6e67 5f69 6473 5b73 6f6e   tagging_ids[son
+0000ca60: 675f 6964 5d0a 2020 2020 2020 2020 2020  g_id].          
 0000ca70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca80: 2020 2020 2020 2020 2020 5d5b 325d 203d            ][2] =
-0000ca90: 2064 6574 6169 6c73 5b32 5d0a 2020 2020   details[2].    
-0000caa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca90: 2020 2020 2020 5d5b 325d 203d 2064 6574        ][2] = det
+0000caa0: 6169 6c73 5b32 5d0a 2020 2020 2020 2020  ails[2].        
 0000cab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cac0: 2020 2020 736f 6e67 735f 6669 6c65 2e63      songs_file.c
-0000cad0: 6c6f 7365 2829 0a0a 2020 2020 2020 2020  lose()..        
-0000cae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cad0: 736f 6e67 735f 6669 6c65 2e63 6c6f 7365  songs_file.close
+0000cae0: 2829 0a0a 2020 2020 2020 2020 2020 2020  ()..            
 0000caf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cb00: 736f 6e67 735f 6669 6c65 203d 206f 7065  songs_file = ope
-0000cb10: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
+0000cb00: 2020 2020 2020 2020 2020 2020 736f 6e67              song
+0000cb10: 735f 6669 6c65 203d 206f 7065 6e28 0a20  s_file = open(. 
 0000cb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cb30: 2020 2020 2020 2020 2020 2020 2020 2053                 S
-0000cb40: 4f4e 4753 5f49 4e46 4f5f 5041 5448 2c0a  ONGS_INFO_PATH,.
-0000cb50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cb40: 2020 2020 2020 2020 2020 2053 4f4e 4753             SONGS
+0000cb50: 5f49 4e46 4f5f 5041 5448 2c0a 2020 2020  _INFO_PATH,.    
 0000cb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cb70: 2020 2020 2020 2020 2020 2020 2277 222c              "w",
-0000cb80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cb70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cb80: 2020 2020 2020 2020 2277 222c 0a20 2020          "w",.   
 0000cb90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cba0: 2020 2020 2020 2020 2020 2020 2065 6e63               enc
-0000cbb0: 6f64 696e 673d 2275 7466 2d38 222c 0a20  oding="utf-8",. 
-0000cbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cbb0: 2020 2020 2020 2020 2065 6e63 6f64 696e           encodin
+0000cbc0: 673d 2275 7466 2d38 222c 0a20 2020 2020  g="utf-8",.     
 0000cbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cbe0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000cbf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cbf0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
 0000cc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc10: 2073 6f6e 6773 5f66 696c 652e 7772 6974   songs_file.writ
-0000cc20: 6528 225c 6e22 2e6a 6f69 6e28 6c69 6e65  e("\n".join(line
-0000cc30: 7329 290a 2020 2020 2020 2020 2020 2020  s)).            
+0000cc10: 2020 2020 2020 2020 2020 2020 2073 6f6e               son
+0000cc20: 6773 5f66 696c 652e 7772 6974 6528 225c  gs_file.write("\
+0000cc30: 6e22 2e6a 6f69 6e28 6c69 6e65 7329 290a  n".join(lines)).
 0000cc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc50: 2020 2020 2020 2020 2020 2020 736f 6e67              song
-0000cc60: 735f 6669 6c65 2e63 6c6f 7365 2829 0a0a  s_file.close()..
-0000cc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cc60: 2020 2020 2020 2020 736f 6e67 735f 6669          songs_fi
+0000cc70: 6c65 2e63 6c6f 7365 2829 0a0a 2020 2020  le.close()..    
 0000cc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc90: 2020 2020 2020 2020 706c 6179 6572 5f6f          player_o
-0000cca0: 7574 7075 742e 7072 6f6d 7074 696e 6720  utput.prompting 
-0000ccb0: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
-0000ccc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ccd0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000cce0: 7572 7365 732e 6375 7273 5f73 6574 2846  urses.curs_set(F
-0000ccf0: 616c 7365 290a 2020 2020 2020 2020 2020  alse).          
-0000cd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd10: 2020 2020 2020 2020 2020 2020 2020 706c                pl
-0000cd20: 6179 6572 5f6f 7574 7075 742e 6f75 7470  ayer_output.outp
-0000cd30: 7574 2870 6c61 7962 6163 6b2e 6375 7272  ut(playback.curr
-0000cd40: 5f70 6f73 290a 2020 2020 2020 2020 2020  _pos).          
-0000cd50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd60: 2020 2020 2020 656c 6966 2063 2069 6e20        elif c in 
-0000cd70: 225c 625c 7837 6622 3a0a 2020 2020 2020  "\b\x7f":.      
-0000cd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd90: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0000cda0: 7079 6c69 6e74 3a20 6469 7361 626c 653d  pylint: disable=
-0000cdb0: 756e 7375 6273 6372 6970 7461 626c 652d  unsubscriptable-
-0000cdc0: 6f62 6a65 6374 0a20 2020 2020 2020 2020  object.         
-0000cdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cde0: 2020 2020 2020 2020 2020 2069 6620 706c             if pl
-0000cdf0: 6179 6572 5f6f 7574 7075 742e 7072 6f6d  ayer_output.prom
-0000ce00: 7074 696e 675b 315d 203e 2030 3a0a 2020  pting[1] > 0:.  
-0000ce10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cca0: 2020 2020 706c 6179 6572 5f6f 7574 7075      player_outpu
+0000ccb0: 742e 7072 6f6d 7074 696e 6720 3d20 4e6f  t.prompting = No
+0000ccc0: 6e65 0a20 2020 2020 2020 2020 2020 2020  ne.             
+0000ccd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cce0: 2020 2020 2020 2020 2020 2063 7572 7365             curse
+0000ccf0: 732e 6375 7273 5f73 6574 2846 616c 7365  s.curs_set(False
+0000cd00: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000cd10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cd20: 2020 2020 2020 2020 2020 706c 6179 6572            player
+0000cd30: 5f6f 7574 7075 742e 6f75 7470 7574 2870  _output.output(p
+0000cd40: 6c61 7962 6163 6b2e 6375 7272 5f70 6f73  layback.curr_pos
+0000cd50: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000cd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cd70: 2020 656c 6966 2063 2069 6e20 225c 625c    elif c in "\b\
+0000cd80: 7837 6622 3a0a 2020 2020 2020 2020 2020  x7f":.          
+0000cd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cda0: 2020 2020 2020 2020 2020 2320 7079 6c69            # pyli
+0000cdb0: 6e74 3a20 6469 7361 626c 653d 756e 7375  nt: disable=unsu
+0000cdc0: 6273 6372 6970 7461 626c 652d 6f62 6a65  bscriptable-obje
+0000cdd0: 6374 0a20 2020 2020 2020 2020 2020 2020  ct.             
+0000cde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cdf0: 2020 2020 2020 2069 6620 706c 6179 6572         if player
+0000ce00: 5f6f 7574 7075 742e 7072 6f6d 7074 696e  _output.promptin
+0000ce10: 675b 315d 203e 2030 3a0a 2020 2020 2020  g[1] > 0:.      
 0000ce20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce30: 2020 2020 2020 706c 6179 6572 5f6f 7574        player_out
-0000ce40: 7075 742e 7072 6f6d 7074 696e 6720 3d20  put.prompting = 
-0000ce50: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000ce30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce40: 2020 706c 6179 6572 5f6f 7574 7075 742e    player_output.
+0000ce50: 7072 6f6d 7074 696e 6720 3d20 280a 2020  prompting = (.  
 0000ce60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce70: 2020 2020 2020 2020 2020 2020 2020 706c                pl
-0000ce80: 6179 6572 5f6f 7574 7075 742e 7072 6f6d  ayer_output.prom
-0000ce90: 7074 696e 675b 305d 5b0a 2020 2020 2020  pting[0][.      
-0000cea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce80: 2020 2020 2020 2020 2020 706c 6179 6572            player
+0000ce90: 5f6f 7574 7075 742e 7072 6f6d 7074 696e  _output.promptin
+0000cea0: 675b 305d 5b0a 2020 2020 2020 2020 2020  g[0][.          
 0000ceb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cec0: 2020 2020 2020 2020 2020 3a20 706c 6179            : play
-0000ced0: 6572 5f6f 7574 7075 742e 7072 6f6d 7074  er_output.prompt
-0000cee0: 696e 675b 315d 202d 2031 0a20 2020 2020  ing[1] - 1.     
-0000cef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ced0: 2020 2020 2020 3a20 706c 6179 6572 5f6f        : player_o
+0000cee0: 7574 7075 742e 7072 6f6d 7074 696e 675b  utput.prompting[
+0000cef0: 315d 202d 2031 0a20 2020 2020 2020 2020  1] - 1.         
 0000cf00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf10: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
-0000cf20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf20: 2020 205d 0a20 2020 2020 2020 2020 2020     ].           
 0000cf30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf40: 2020 2020 202b 2070 6c61 7965 725f 6f75       + player_ou
-0000cf50: 7470 7574 2e70 726f 6d70 7469 6e67 5b30  tput.prompting[0
-0000cf60: 5d5b 0a20 2020 2020 2020 2020 2020 2020  ][.             
+0000cf40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf50: 202b 2070 6c61 7965 725f 6f75 7470 7574   + player_output
+0000cf60: 2e70 726f 6d70 7469 6e67 5b30 5d5b 0a20  .prompting[0][. 
 0000cf70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000cf80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf90: 2020 2070 6c61 7965 725f 6f75 7470 7574     player_output
-0000cfa0: 2e70 726f 6d70 7469 6e67 5b31 5d20 3a0a  .prompting[1] :.
-0000cfb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf90: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000cfa0: 6c61 7965 725f 6f75 7470 7574 2e70 726f  layer_output.pro
+0000cfb0: 6d70 7469 6e67 5b31 5d20 3a0a 2020 2020  mpting[1] :.    
 0000cfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cfd0: 2020 2020 2020 2020 2020 2020 5d2c 0a20              ],. 
-0000cfe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cfd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cfe0: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
 0000cff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d000: 2020 2020 2020 2020 2020 2070 6c61 7965             playe
-0000d010: 725f 6f75 7470 7574 2e70 726f 6d70 7469  r_output.prompti
-0000d020: 6e67 5b31 5d20 2d20 312c 0a20 2020 2020  ng[1] - 1,.     
-0000d030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d010: 2020 2020 2020 2070 6c61 7965 725f 6f75         player_ou
+0000d020: 7470 7574 2e70 726f 6d70 7469 6e67 5b31  tput.prompting[1
+0000d030: 5d20 2d20 312c 0a20 2020 2020 2020 2020  ] - 1,.         
 0000d040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d050: 2020 2020 2020 2070 6c61 7965 725f 6f75         player_ou
-0000d060: 7470 7574 2e70 726f 6d70 7469 6e67 5b32  tput.prompting[2
-0000d070: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+0000d050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d060: 2020 2070 6c61 7965 725f 6f75 7470 7574     player_output
+0000d070: 2e70 726f 6d70 7469 6e67 5b32 5d2c 0a20  .prompting[2],. 
 0000d080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d090: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0000d0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0a0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
 0000d0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d0c0: 2070 6c61 7965 725f 6f75 7470 7574 2e6f   player_output.o
-0000d0d0: 7574 7075 7428 706c 6179 6261 636b 2e63  utput(playback.c
-0000d0e0: 7572 725f 706f 7329 0a20 2020 2020 2020  urr_pos).       
-0000d0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d100: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-0000d110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0c0: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
+0000d0d0: 7965 725f 6f75 7470 7574 2e6f 7574 7075  yer_output.outpu
+0000d0e0: 7428 706c 6179 6261 636b 2e63 7572 725f  t(playback.curr_
+0000d0f0: 706f 7329 0a20 2020 2020 2020 2020 2020  pos).           
+0000d100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d110: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
 0000d120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d130: 2020 2070 6c61 7965 725f 6f75 7470 7574     player_output
-0000d140: 2e70 726f 6d70 7469 6e67 203d 2028 0a20  .prompting = (. 
-0000d150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d130: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000d140: 6c61 7965 725f 6f75 7470 7574 2e70 726f  layer_output.pro
+0000d150: 6d70 7469 6e67 203d 2028 0a20 2020 2020  mpting = (.     
 0000d160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d170: 2020 2020 2020 2023 2070 796c 696e 743a         # pylint:
-0000d180: 2064 6973 6162 6c65 3d75 6e73 7562 7363   disable=unsubsc
-0000d190: 7269 7074 6162 6c65 2d6f 626a 6563 740a  riptable-object.
-0000d1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d180: 2020 2023 2070 796c 696e 743a 2064 6973     # pylint: dis
+0000d190: 6162 6c65 3d75 6e73 7562 7363 7269 7074  able=unsubscript
+0000d1a0: 6162 6c65 2d6f 626a 6563 740a 2020 2020  able-object.    
 0000d1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d1c0: 2020 2020 2020 2020 706c 6179 6572 5f6f          player_o
-0000d1d0: 7574 7075 742e 7072 6f6d 7074 696e 675b  utput.prompting[
-0000d1e0: 305d 5b0a 2020 2020 2020 2020 2020 2020  0][.            
+0000d1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d1d0: 2020 2020 706c 6179 6572 5f6f 7574 7075      player_outpu
+0000d1e0: 742e 7072 6f6d 7074 696e 675b 305d 5b0a  t.prompting[0][.
 0000d1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000d200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d210: 3a20 706c 6179 6572 5f6f 7574 7075 742e  : player_output.
-0000d220: 7072 6f6d 7074 696e 675b 315d 0a20 2020  prompting[1].   
-0000d230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d210: 2020 2020 2020 2020 2020 2020 3a20 706c              : pl
+0000d220: 6179 6572 5f6f 7574 7075 742e 7072 6f6d  ayer_output.prom
+0000d230: 7074 696e 675b 315d 0a20 2020 2020 2020  pting[1].       
 0000d240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d250: 2020 2020 205d 0a20 2020 2020 2020 2020       ].         
-0000d260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d270: 2020 2020 2020 2020 2020 2020 2020 202b                 +
-0000d280: 2063 0a20 2020 2020 2020 2020 2020 2020   c.             
+0000d250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d260: 205d 0a20 2020 2020 2020 2020 2020 2020   ].             
+0000d270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d280: 2020 2020 2020 2020 2020 202b 2063 0a20             + c. 
 0000d290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d2a0: 2020 2020 2020 2020 2020 202b 2070 6c61             + pla
-0000d2b0: 7965 725f 6f75 7470 7574 2e70 726f 6d70  yer_output.promp
-0000d2c0: 7469 6e67 5b30 5d5b 0a20 2020 2020 2020  ting[0][.       
-0000d2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d2b0: 2020 2020 2020 202b 2070 6c61 7965 725f         + player_
+0000d2c0: 6f75 7470 7574 2e70 726f 6d70 7469 6e67  output.prompting
+0000d2d0: 5b30 5d5b 0a20 2020 2020 2020 2020 2020  [0][.           
 0000d2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d2f0: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
-0000d300: 7574 2e70 726f 6d70 7469 6e67 5b31 5d20  ut.prompting[1] 
-0000d310: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000d2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d300: 2070 6c61 7965 725f 6f75 7470 7574 2e70   player_output.p
+0000d310: 726f 6d70 7469 6e67 5b31 5d20 3a0a 2020  rompting[1] :.  
 0000d320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d330: 2020 2020 2020 2020 2020 5d2c 0a20 2020            ],.   
-0000d340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d340: 2020 2020 2020 5d2c 0a20 2020 2020 2020        ],.       
 0000d350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d360: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
-0000d370: 7574 2e70 726f 6d70 7469 6e67 5b31 5d20  ut.prompting[1] 
-0000d380: 2b20 312c 0a20 2020 2020 2020 2020 2020  + 1,.           
-0000d390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d3a0: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
-0000d3b0: 7965 725f 6f75 7470 7574 2e70 726f 6d70  yer_output.promp
-0000d3c0: 7469 6e67 5b32 5d2c 0a20 2020 2020 2020  ting[2],.       
-0000d3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d3e0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-0000d3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d370: 2070 6c61 7965 725f 6f75 7470 7574 2e70   player_output.p
+0000d380: 726f 6d70 7469 6e67 5b31 5d20 2b20 312c  rompting[1] + 1,
+0000d390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d3b0: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
+0000d3c0: 6f75 7470 7574 2e70 726f 6d70 7469 6e67  output.prompting
+0000d3d0: 5b32 5d2c 0a20 2020 2020 2020 2020 2020  [2],.           
+0000d3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d3f0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
 0000d400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d410: 2020 2070 6c61 7965 725f 6f75 7470 7574     player_output
-0000d420: 2e6f 7574 7075 7428 706c 6179 6261 636b  .output(playback
-0000d430: 2e63 7572 725f 706f 7329 0a20 2020 2020  .curr_pos).     
-0000d440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d450: 2020 2020 2020 2065 7863 6570 7420 2856         except (V
-0000d460: 616c 7565 4572 726f 722c 204f 7665 7266  alueError, Overf
-0000d470: 6c6f 7745 7272 6f72 293a 0a20 2020 2020  lowError):.     
-0000d480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d490: 2020 2020 2020 2020 2020 2070 6173 730a             pass.
-0000d4a0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000d4b0: 7379 732e 706c 6174 666f 726d 203d 3d20  sys.platform == 
-0000d4c0: 2264 6172 7769 6e22 2061 6e64 2063 616e  "darwin" and can
-0000d4d0: 5f6d 6163 5f6e 6f77 5f70 6c61 7969 6e67  _mac_now_playing
-0000d4e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000d4f0: 2020 6966 2061 6273 286d 6163 5f6e 6f77    if abs(mac_now
-0000d500: 5f70 6c61 7969 6e67 2e70 6f73 202d 2070  _playing.pos - p
-0000d510: 6c61 7962 6163 6b2e 6375 7272 5f70 6f73  layback.curr_pos
-0000d520: 2920 3e20 323a 0a20 2020 2020 2020 2020  ) > 2:.         
-0000d530: 2020 2020 2020 2020 2020 2070 6c61 7962             playb
-0000d540: 6163 6b2e 7365 656b 286d 6163 5f6e 6f77  ack.seek(mac_now
-0000d550: 5f70 6c61 7969 6e67 2e70 6f73 290a 2020  _playing.pos).  
-0000d560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d570: 2020 6c61 7374 5f74 696d 6573 7461 6d70    last_timestamp
-0000d580: 203d 206d 6163 5f6e 6f77 5f70 6c61 7969   = mac_now_playi
-0000d590: 6e67 2e70 6f73 0a20 2020 2020 2020 2020  ng.pos.         
-0000d5a0: 2020 2020 2020 2020 2020 2075 7064 6174             updat
-0000d5b0: 655f 6e6f 775f 706c 6179 696e 6720 3d20  e_now_playing = 
-0000d5c0: 5472 7565 0a20 2020 2020 2020 2020 2020  True.           
-0000d5d0: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
-0000d5e0: 6f75 7470 7574 2e6f 7574 7075 7428 706c  output.output(pl
-0000d5f0: 6179 6261 636b 2e63 7572 725f 706f 7329  ayback.curr_pos)
-0000d600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d610: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000d620: 2020 2020 2020 2020 2020 206d 6163 5f6e             mac_n
-0000d630: 6f77 5f70 6c61 7969 6e67 2e70 6f73 203d  ow_playing.pos =
-0000d640: 2072 6f75 6e64 2870 6c61 7962 6163 6b2e   round(playback.
-0000d650: 6375 7272 5f70 6f73 290a 0a20 2020 2020  curr_pos)..     
-0000d660: 2020 2020 2020 2070 726f 6772 6573 735f         progress_
-0000d670: 6261 725f 7769 6474 6820 3d20 7374 6473  bar_width = stds
-0000d680: 6372 2e67 6574 6d61 7879 7828 295b 315d  cr.getmaxyx()[1]
-0000d690: 202d 2031 380a 2020 2020 2020 2020 2020   - 18.          
-0000d6a0: 2020 6672 616d 655f 6475 7261 7469 6f6e    frame_duration
-0000d6b0: 203d 206d 696e 280a 2020 2020 2020 2020   = min(.        
-0000d6c0: 2020 2020 2020 2020 280a 2020 2020 2020          (.      
-0000d6d0: 2020 2020 2020 2020 2020 2020 2020 310a                1.
-0000d6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d6f0: 2020 2020 6966 2070 726f 6772 6573 735f      if progress_
-0000d700: 6261 725f 7769 6474 6820 3c20 4d49 4e5f  bar_width < MIN_
-0000d710: 5052 4f47 5245 5353 5f42 4152 5f57 4944  PROGRESS_BAR_WID
-0000d720: 5448 0a20 2020 2020 2020 2020 2020 2020  TH.             
-0000d730: 2020 2020 2020 2065 6c73 6520 706c 6179         else play
-0000d740: 6572 5f6f 7574 7075 742e 6475 7261 7469  er_output.durati
-0000d750: 6f6e 202f 2028 7072 6f67 7265 7373 5f62  on / (progress_b
-0000d760: 6172 5f77 6964 7468 202a 2038 290a 2020  ar_width * 8).  
-0000d770: 2020 2020 2020 2020 2020 2020 2020 292c                ),
-0000d780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d790: 2031 202f 2046 5053 2069 6620 706c 6179   1 / FPS if play
-0000d7a0: 6572 5f6f 7574 7075 742e 7669 7375 616c  er_output.visual
-0000d7b0: 697a 6520 656c 7365 2031 2c0a 2020 2020  ize else 1,.    
-0000d7c0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000d7d0: 2020 2020 2020 6966 2061 6273 2870 6c61        if abs(pla
-0000d7e0: 7962 6163 6b2e 6375 7272 5f70 6f73 202d  yback.curr_pos -
-0000d7f0: 206c 6173 745f 7469 6d65 7374 616d 7029   last_timestamp)
-0000d800: 203e 2066 7261 6d65 5f64 7572 6174 696f   > frame_duratio
-0000d810: 6e3a 0a20 2020 2020 2020 2020 2020 2020  n:.             
-0000d820: 2020 206c 6173 745f 7469 6d65 7374 616d     last_timestam
-0000d830: 7020 3d20 706c 6179 6261 636b 2e63 7572  p = playback.cur
-0000d840: 725f 706f 730a 2020 2020 2020 2020 2020  r_pos.          
-0000d850: 2020 2020 2020 706c 6179 6572 5f6f 7574        player_out
-0000d860: 7075 742e 6f75 7470 7574 2870 6c61 7962  put.output(playb
-0000d870: 6163 6b2e 6375 7272 5f70 6f73 290a 0a20  ack.curr_pos).. 
-0000d880: 2020 2020 2020 2020 2020 2023 2073 6c65             # sle
-0000d890: 6570 2830 2e30 3129 2020 2320 4e4f 5445  ep(0.01)  # NOTE
-0000d8a0: 3a20 736f 2043 5055 2075 7361 6765 2064  : so CPU usage d
-0000d8b0: 6f65 736e 2774 2066 6c79 2074 6872 6f75  oesn't fly throu
-0000d8c0: 6768 2074 6865 2072 6f6f 660a 0a20 2020  gh the roof..   
-0000d8d0: 2020 2020 2023 2072 6567 696f 6e20 7374       # region st
-0000d8e0: 6174 730a 2020 2020 2020 2020 7469 6d65  ats.        time
-0000d8f0: 5f6c 6973 7465 6e65 6420 3d20 7469 6d65  _listened = time
-0000d900: 2829 202d 2073 7461 7274 5f74 696d 650a  () - start_time.
-0000d910: 2020 2020 2020 2020 6966 2070 6c61 7965          if playe
-0000d920: 725f 6f75 7470 7574 2e70 6175 7365 643a  r_output.paused:
-0000d930: 0a20 2020 2020 2020 2020 2020 2074 696d  .            tim
-0000d940: 655f 6c69 7374 656e 6564 202d 3d20 7469  e_listened -= ti
-0000d950: 6d65 2829 202d 2070 6175 7365 5f73 7461  me() - pause_sta
-0000d960: 7274 0a0a 2020 2020 2020 2020 7769 7468  rt..        with
-0000d970: 206f 7065 6e28 544f 5441 4c5f 5354 4154   open(TOTAL_STAT
-0000d980: 535f 5041 5448 2c20 2272 2b22 2c20 656e  S_PATH, "r+", en
-0000d990: 636f 6469 6e67 3d22 7574 662d 3822 2920  coding="utf-8") 
-0000d9a0: 6173 2073 7461 7473 5f66 696c 653a 0a20  as stats_file:. 
-0000d9b0: 2020 2020 2020 2020 2020 206c 696e 6573             lines
-0000d9c0: 203d 2073 7461 7473 5f66 696c 652e 7265   = stats_file.re
-0000d9d0: 6164 6c69 6e65 7328 290a 2020 2020 2020  adlines().      
-0000d9e0: 2020 2020 2020 666f 7220 6a20 696e 2072        for j in r
-0000d9f0: 616e 6765 286c 656e 286c 696e 6573 2929  ange(len(lines))
-0000da00: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000da10: 2020 736f 6e67 5f69 642c 206c 6973 7465    song_id, liste
-0000da20: 6e65 6420 3d20 6c69 6e65 735b 6a5d 2e73  ned = lines[j].s
-0000da30: 7472 6970 2829 2e73 706c 6974 2822 7c22  trip().split("|"
-0000da40: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000da50: 2020 6966 2073 6f6e 675f 6964 203d 3d20    if song_id == 
-0000da60: 706c 6179 6572 5f6f 7574 7075 742e 706c  player_output.pl
-0000da70: 6179 6c69 7374 5b70 6c61 7965 725f 6f75  aylist[player_ou
-0000da80: 7470 7574 2e69 5d5b 305d 3a0a 2020 2020  tput.i][0]:.    
-0000da90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000daa0: 6c69 7374 656e 6564 203d 2066 6c6f 6174  listened = float
-0000dab0: 286c 6973 7465 6e65 6429 202b 2074 696d  (listened) + tim
-0000dac0: 655f 6c69 7374 656e 6564 0a20 2020 2020  e_listened.     
-0000dad0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-0000dae0: 696e 6573 5b6a 5d20 3d20 6622 7b73 6f6e  ines[j] = f"{son
-0000daf0: 675f 6964 7d7c 7b6c 6973 7465 6e65 647d  g_id}|{listened}
-0000db00: 5c6e 220a 2020 2020 2020 2020 2020 2020  \n".            
-0000db10: 2020 2020 2020 2020 6272 6561 6b0a 0a20          break.. 
-0000db20: 2020 2020 2020 2020 2020 2023 2077 7269             # wri
-0000db30: 7465 206f 7574 0a20 2020 2020 2020 2020  te out.         
-0000db40: 2020 2073 7461 7473 5f66 696c 652e 7365     stats_file.se
-0000db50: 656b 2830 290a 2020 2020 2020 2020 2020  ek(0).          
-0000db60: 2020 7374 6174 735f 6669 6c65 2e77 7269    stats_file.wri
-0000db70: 7465 2822 222e 6a6f 696e 286c 696e 6573  te("".join(lines
-0000db80: 2929 0a20 2020 2020 2020 2020 2020 2073  )).            s
-0000db90: 7461 7473 5f66 696c 652e 7472 756e 6361  tats_file.trunca
-0000dba0: 7465 2829 0a0a 2020 2020 2020 2020 7769  te()..        wi
-0000dbb0: 7468 206f 7065 6e28 4355 525f 5945 4152  th open(CUR_YEAR
-0000dbc0: 5f53 5441 5453 5f50 4154 482c 2022 722b  _STATS_PATH, "r+
-0000dbd0: 222c 2065 6e63 6f64 696e 673d 2275 7466  ", encoding="utf
-0000dbe0: 2d38 2229 2061 7320 7374 6174 735f 6669  -8") as stats_fi
-0000dbf0: 6c65 3a0a 2020 2020 2020 2020 2020 2020  le:.            
-0000dc00: 6c69 6e65 7320 3d20 7374 6174 735f 6669  lines = stats_fi
-0000dc10: 6c65 2e72 6561 646c 696e 6573 2829 0a20  le.readlines(). 
-0000dc20: 2020 2020 2020 2020 2020 2066 6f72 206a             for j
-0000dc30: 2069 6e20 7261 6e67 6528 6c65 6e28 6c69   in range(len(li
-0000dc40: 6e65 7329 293a 0a20 2020 2020 2020 2020  nes)):.         
-0000dc50: 2020 2020 2020 2073 6f6e 675f 6964 2c20         song_id, 
-0000dc60: 6c69 7374 656e 6564 203d 206c 696e 6573  listened = lines
-0000dc70: 5b6a 5d2e 7374 7269 7028 292e 7370 6c69  [j].strip().spli
-0000dc80: 7428 227c 2229 0a20 2020 2020 2020 2020  t("|").         
-0000dc90: 2020 2020 2020 2069 6620 736f 6e67 5f69         if song_i
-0000dca0: 6420 3d3d 2070 6c61 7965 725f 6f75 7470  d == player_outp
-0000dcb0: 7574 2e70 6c61 796c 6973 745b 706c 6179  ut.playlist[play
-0000dcc0: 6572 5f6f 7574 7075 742e 695d 5b30 5d3a  er_output.i][0]:
-0000dcd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000dce0: 2020 2020 206c 6973 7465 6e65 6420 3d20       listened = 
-0000dcf0: 666c 6f61 7428 6c69 7374 656e 6564 2920  float(listened) 
-0000dd00: 2b20 7469 6d65 5f6c 6973 7465 6e65 640a  + time_listened.
-0000dd10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd20: 2020 2020 6c69 6e65 735b 6a5d 203d 2066      lines[j] = f
-0000dd30: 227b 736f 6e67 5f69 647d 7c7b 6c69 7374  "{song_id}|{list
-0000dd40: 656e 6564 7d5c 6e22 0a20 2020 2020 2020  ened}\n".       
-0000dd50: 2020 2020 2020 2020 2020 2020 2062 7265               bre
-0000dd60: 616b 0a0a 2020 2020 2020 2020 2020 2020  ak..            
-0000dd70: 2320 7772 6974 6520 6f75 740a 2020 2020  # write out.    
-0000dd80: 2020 2020 2020 2020 7374 6174 735f 6669          stats_fi
-0000dd90: 6c65 2e73 6565 6b28 3029 0a20 2020 2020  le.seek(0).     
-0000dda0: 2020 2020 2020 2073 7461 7473 5f66 696c         stats_fil
-0000ddb0: 652e 7772 6974 6528 2222 2e6a 6f69 6e28  e.write("".join(
-0000ddc0: 6c69 6e65 7329 290a 2020 2020 2020 2020  lines)).        
-0000ddd0: 2020 2020 7374 6174 735f 6669 6c65 2e74      stats_file.t
-0000dde0: 7275 6e63 6174 6528 290a 2020 2020 2020  runcate().      
-0000ddf0: 2020 2320 656e 6472 6567 696f 6e0a 0a20    # endregion.. 
-0000de00: 2020 2020 2020 2069 6620 706c 6179 6572         if player
-0000de10: 5f6f 7574 7075 742e 656e 6469 6e67 3a0a  _output.ending:.
-0000de20: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000de30: 726e 0a0a 2020 2020 2020 2020 6966 206e  rn..        if n
-0000de40: 6578 745f 736f 6e67 203d 3d20 2d31 3a0a  ext_song == -1:.
-0000de50: 2020 2020 2020 2020 2020 2020 6966 2070              if p
-0000de60: 6c61 7965 725f 6f75 7470 7574 2e69 203d  layer_output.i =
-0000de70: 3d20 706c 6179 6572 5f6f 7574 7075 742e  = player_output.
-0000de80: 7363 726f 6c6c 6572 2e70 6f73 3a0a 2020  scroller.pos:.  
-0000de90: 2020 2020 2020 2020 2020 2020 2020 706c                pl
-0000dea0: 6179 6572 5f6f 7574 7075 742e 7363 726f  ayer_output.scro
-0000deb0: 6c6c 6572 2e73 6372 6f6c 6c5f 6261 636b  ller.scroll_back
-0000dec0: 7761 7264 2829 0a20 2020 2020 2020 2020  ward().         
-0000ded0: 2020 2070 6c61 7965 725f 6f75 7470 7574     player_output
-0000dee0: 2e69 202d 3d20 310a 2020 2020 2020 2020  .i -= 1.        
-0000def0: 656c 6966 206e 6578 745f 736f 6e67 203d  elif next_song =
-0000df00: 3d20 313a 0a20 2020 2020 2020 2020 2020  = 1:.           
-0000df10: 2069 6620 706c 6179 6572 5f6f 7574 7075   if player_outpu
-0000df20: 742e 6920 3d3d 206c 656e 2870 6c61 7965  t.i == len(playe
-0000df30: 725f 6f75 7470 7574 2e70 6c61 796c 6973  r_output.playlis
-0000df40: 7429 202d 2031 3a0a 2020 2020 2020 2020  t) - 1:.        
-0000df50: 2020 2020 2020 2020 6966 206c 6f6f 703a          if loop:
-0000df60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000df70: 2020 2020 206e 6578 745f 6e65 7874 5f70       next_next_p
-0000df80: 6c61 796c 6973 7420 3d20 6e65 7874 5f70  laylist = next_p
-0000df90: 6c61 796c 6973 745b 3a5d 0a20 2020 2020  laylist[:].     
-0000dfa0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000dfb0: 6620 7265 7368 7566 666c 653a 0a20 2020  f reshuffle:.   
-0000dfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dfd0: 2020 2020 2073 6875 6666 6c65 286e 6578       shuffle(nex
-0000dfe0: 745f 6e65 7874 5f70 6c61 796c 6973 7429  t_next_playlist)
-0000dff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e000: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
-0000e010: 7574 2e70 6c61 796c 6973 742c 206e 6578  ut.playlist, nex
-0000e020: 745f 706c 6179 6c69 7374 203d 2028 0a20  t_playlist = (. 
-0000e030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e040: 2020 2020 2020 206e 6578 745f 706c 6179         next_play
-0000e050: 6c69 7374 2c0a 2020 2020 2020 2020 2020  list,.          
-0000e060: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
-0000e070: 7874 5f6e 6578 745f 706c 6179 6c69 7374  xt_next_playlist
-0000e080: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000e090: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0000e0a0: 2020 2020 2020 2020 2020 2020 706c 6179              play
-0000e0b0: 6572 5f6f 7574 7075 742e 6920 3d20 2d31  er_output.i = -1
-0000e0c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e0d0: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
-0000e0e0: 7574 2e73 6372 6f6c 6c65 722e 706f 7320  ut.scroller.pos 
-0000e0f0: 3d20 300a 2020 2020 2020 2020 2020 2020  = 0.            
-0000e100: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000e110: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0000e120: 7475 726e 0a20 2020 2020 2020 2020 2020  turn.           
-0000e130: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000e140: 2020 2020 2020 2069 6620 706c 6179 6572         if player
-0000e150: 5f6f 7574 7075 742e 6920 3d3d 2070 6c61  _output.i == pla
-0000e160: 7965 725f 6f75 7470 7574 2e73 6372 6f6c  yer_output.scrol
-0000e170: 6c65 722e 706f 733a 0a20 2020 2020 2020  ler.pos:.       
-0000e180: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
-0000e190: 7965 725f 6f75 7470 7574 2e73 6372 6f6c  yer_output.scrol
-0000e1a0: 6c65 722e 7363 726f 6c6c 5f66 6f72 7761  ler.scroll_forwa
-0000e1b0: 7264 2829 0a20 2020 2020 2020 2020 2020  rd().           
-0000e1c0: 2070 6c61 7965 725f 6f75 7470 7574 2e69   player_output.i
-0000e1d0: 202b 3d20 310a 2020 2020 2020 2020 656c   += 1.        el
-0000e1e0: 6966 206e 6578 745f 736f 6e67 203d 3d20  if next_song == 
-0000e1f0: 303a 0a20 2020 2020 2020 2020 2020 2069  0:.            i
-0000e200: 6620 706c 6179 6572 5f6f 7574 7075 742e  f player_output.
-0000e210: 6c6f 6f70 696e 675f 6375 7272 656e 745f  looping_current_
-0000e220: 736f 6e67 203d 3d20 4c4f 4f50 5f4d 4f44  song == LOOP_MOD
-0000e230: 4553 5b22 6f6e 6522 5d3a 0a20 2020 2020  ES["one"]:.     
-0000e240: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-0000e250: 5f74 6f5f 6c6f 6766 696c 6528 0a20 2020  _to_logfile(.   
-0000e260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e270: 2070 6c61 7965 725f 6f75 7470 7574 2e6c   player_output.l
-0000e280: 6f6f 7069 6e67 5f63 7572 7265 6e74 5f73  ooping_current_s
-0000e290: 6f6e 672c 204c 4f4f 505f 4d4f 4445 535b  ong, LOOP_MODES[
-0000e2a0: 226f 6e65 225d 0a20 2020 2020 2020 2020  "one"].         
-0000e2b0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000e2c0: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
-0000e2d0: 6f75 7470 7574 2e6c 6f6f 7069 6e67 5f63  output.looping_c
-0000e2e0: 7572 7265 6e74 5f73 6f6e 6720 3d20 4c4f  urrent_song = LO
-0000e2f0: 4f50 5f4d 4f44 4553 5b22 6e6f 6e65 225d  OP_MODES["none"]
-0000e300: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e310: 2070 7269 6e74 5f74 6f5f 6c6f 6766 696c   print_to_logfil
-0000e320: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
-0000e330: 2020 2020 2020 2070 6c61 7965 725f 6f75         player_ou
-0000e340: 7470 7574 2e6c 6f6f 7069 6e67 5f63 7572  tput.looping_cur
-0000e350: 7265 6e74 5f73 6f6e 672c 204c 4f4f 505f  rent_song, LOOP_
-0000e360: 4d4f 4445 535b 226e 6f6e 6522 5d0a 2020  MODES["none"].  
-0000e370: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-0000e380: 0a0a 2320 656e 6472 6567 696f 6e0a 0a0a  ..# endregion...
-0000e390: 4063 6c69 636b 2e67 726f 7570 2863 6f6e  @click.group(con
-0000e3a0: 7465 7874 5f73 6574 7469 6e67 733d 6469  text_settings=di
-0000e3b0: 6374 2868 656c 705f 6f70 7469 6f6e 5f6e  ct(help_option_n
-0000e3c0: 616d 6573 3d5b 222d 6822 2c20 222d 2d68  ames=["-h", "--h
-0000e3d0: 656c 7022 5d29 290a 6465 6620 636c 6928  elp"])).def cli(
-0000e3e0: 293a 0a20 2020 2022 2222 4120 636f 6d6d  ):.    """A comm
-0000e3f0: 616e 6420 6c69 6e65 2069 6e74 6572 6661  and line interfa
-0000e400: 6365 2066 6f72 2070 6c61 7969 6e67 206d  ce for playing m
-0000e410: 7573 6963 2e22 2222 0a20 2020 2069 6620  usic.""".    if 
-0000e420: 6e6f 7420 6f73 2e70 6174 682e 6578 6973  not os.path.exis
-0000e430: 7473 2853 4f4e 4753 5f44 4952 293a 0a20  ts(SONGS_DIR):. 
-0000e440: 2020 2020 2020 206f 732e 6d61 6b65 6469         os.makedi
-0000e450: 7273 2853 4f4e 4753 5f44 4952 290a 0a20  rs(SONGS_DIR).. 
+0000d410: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000d420: 6c61 7965 725f 6f75 7470 7574 2e6f 7574  layer_output.out
+0000d430: 7075 7428 706c 6179 6261 636b 2e63 7572  put(playback.cur
+0000d440: 725f 706f 7329 0a20 2020 2020 2020 2020  r_pos).         
+0000d450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d460: 2020 2065 7863 6570 7420 2856 616c 7565     except (Value
+0000d470: 4572 726f 722c 204f 7665 7266 6c6f 7745  Error, OverflowE
+0000d480: 7272 6f72 293a 0a20 2020 2020 2020 2020  rror):.         
+0000d490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d4a0: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
+0000d4b0: 2020 2020 2020 2020 2069 6620 7379 732e           if sys.
+0000d4c0: 706c 6174 666f 726d 203d 3d20 2264 6172  platform == "dar
+0000d4d0: 7769 6e22 2061 6e64 2063 616e 5f6d 6163  win" and can_mac
+0000d4e0: 5f6e 6f77 5f70 6c61 7969 6e67 3a0a 2020  _now_playing:.  
+0000d4f0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000d500: 2061 6273 286d 6163 5f6e 6f77 5f70 6c61   abs(mac_now_pla
+0000d510: 7969 6e67 2e70 6f73 202d 2070 6c61 7962  ying.pos - playb
+0000d520: 6163 6b2e 6375 7272 5f70 6f73 2920 3e20  ack.curr_pos) > 
+0000d530: 323a 0a20 2020 2020 2020 2020 2020 2020  2:.             
+0000d540: 2020 2020 2020 2070 6c61 7962 6163 6b2e         playback.
+0000d550: 7365 656b 286d 6163 5f6e 6f77 5f70 6c61  seek(mac_now_pla
+0000d560: 7969 6e67 2e70 6f73 290a 2020 2020 2020  ying.pos).      
+0000d570: 2020 2020 2020 2020 2020 2020 2020 6c61                la
+0000d580: 7374 5f74 696d 6573 7461 6d70 203d 206d  st_timestamp = m
+0000d590: 6163 5f6e 6f77 5f70 6c61 7969 6e67 2e70  ac_now_playing.p
+0000d5a0: 6f73 0a20 2020 2020 2020 2020 2020 2020  os.             
+0000d5b0: 2020 2020 2020 2075 7064 6174 655f 6e6f         update_no
+0000d5c0: 775f 706c 6179 696e 6720 3d20 5472 7565  w_playing = True
+0000d5d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d5e0: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
+0000d5f0: 7574 2e6f 7574 7075 7428 706c 6179 6261  ut.output(playba
+0000d600: 636b 2e63 7572 725f 706f 7329 0a20 2020  ck.curr_pos).   
+0000d610: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+0000d620: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0000d630: 2020 2020 2020 206d 6163 5f6e 6f77 5f70         mac_now_p
+0000d640: 6c61 7969 6e67 2e70 6f73 203d 2072 6f75  laying.pos = rou
+0000d650: 6e64 2870 6c61 7962 6163 6b2e 6375 7272  nd(playback.curr
+0000d660: 5f70 6f73 290a 0a20 2020 2020 2020 2020  _pos)..         
+0000d670: 2020 2070 726f 6772 6573 735f 6261 725f     progress_bar_
+0000d680: 7769 6474 6820 3d20 7374 6473 6372 2e67  width = stdscr.g
+0000d690: 6574 6d61 7879 7828 295b 315d 202d 2031  etmaxyx()[1] - 1
+0000d6a0: 380a 2020 2020 2020 2020 2020 2020 6672  8.            fr
+0000d6b0: 616d 655f 6475 7261 7469 6f6e 203d 206d  ame_duration = m
+0000d6c0: 696e 280a 2020 2020 2020 2020 2020 2020  in(.            
+0000d6d0: 2020 2020 280a 2020 2020 2020 2020 2020      (.          
+0000d6e0: 2020 2020 2020 2020 2020 310a 2020 2020            1.    
+0000d6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d700: 6966 2070 726f 6772 6573 735f 6261 725f  if progress_bar_
+0000d710: 7769 6474 6820 3c20 4d49 4e5f 5052 4f47  width < MIN_PROG
+0000d720: 5245 5353 5f42 4152 5f57 4944 5448 0a20  RESS_BAR_WIDTH. 
+0000d730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d740: 2020 2065 6c73 6520 706c 6179 6572 5f6f     else player_o
+0000d750: 7574 7075 742e 6475 7261 7469 6f6e 202f  utput.duration /
+0000d760: 2028 7072 6f67 7265 7373 5f62 6172 5f77   (progress_bar_w
+0000d770: 6964 7468 202a 2038 290a 2020 2020 2020  idth * 8).      
+0000d780: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
+0000d790: 2020 2020 2020 2020 2020 2020 2031 202f               1 /
+0000d7a0: 2046 5053 2069 6620 706c 6179 6572 5f6f   FPS if player_o
+0000d7b0: 7574 7075 742e 7669 7375 616c 697a 6520  utput.visualize 
+0000d7c0: 656c 7365 2031 2c0a 2020 2020 2020 2020  else 1,.        
+0000d7d0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0000d7e0: 2020 6966 2061 6273 2870 6c61 7962 6163    if abs(playbac
+0000d7f0: 6b2e 6375 7272 5f70 6f73 202d 206c 6173  k.curr_pos - las
+0000d800: 745f 7469 6d65 7374 616d 7029 203e 2066  t_timestamp) > f
+0000d810: 7261 6d65 5f64 7572 6174 696f 6e3a 0a20  rame_duration:. 
+0000d820: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+0000d830: 6173 745f 7469 6d65 7374 616d 7020 3d20  ast_timestamp = 
+0000d840: 706c 6179 6261 636b 2e63 7572 725f 706f  playback.curr_po
+0000d850: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+0000d860: 2020 706c 6179 6572 5f6f 7574 7075 742e    player_output.
+0000d870: 6f75 7470 7574 2870 6c61 7962 6163 6b2e  output(playback.
+0000d880: 6375 7272 5f70 6f73 290a 0a20 2020 2020  curr_pos)..     
+0000d890: 2020 2020 2020 2023 2073 6c65 6570 2830         # sleep(0
+0000d8a0: 2e30 3129 2020 2320 4e4f 5445 3a20 736f  .01)  # NOTE: so
+0000d8b0: 2043 5055 2075 7361 6765 2064 6f65 736e   CPU usage doesn
+0000d8c0: 2774 2066 6c79 2074 6872 6f75 6768 2074  't fly through t
+0000d8d0: 6865 2072 6f6f 660a 0a20 2020 2020 2020  he roof..       
+0000d8e0: 2023 2072 6567 696f 6e20 7374 6174 730a   # region stats.
+0000d8f0: 2020 2020 2020 2020 7469 6d65 5f6c 6973          time_lis
+0000d900: 7465 6e65 6420 3d20 7469 6d65 2829 202d  tened = time() -
+0000d910: 2073 7461 7274 5f74 696d 650a 2020 2020   start_time.    
+0000d920: 2020 2020 6966 2070 6c61 7965 725f 6f75      if player_ou
+0000d930: 7470 7574 2e70 6175 7365 643a 0a20 2020  tput.paused:.   
+0000d940: 2020 2020 2020 2020 2074 696d 655f 6c69           time_li
+0000d950: 7374 656e 6564 202d 3d20 7469 6d65 2829  stened -= time()
+0000d960: 202d 2070 6175 7365 5f73 7461 7274 0a0a   - pause_start..
+0000d970: 2020 2020 2020 2020 7769 7468 206f 7065          with ope
+0000d980: 6e28 544f 5441 4c5f 5354 4154 535f 5041  n(TOTAL_STATS_PA
+0000d990: 5448 2c20 2272 2b22 2c20 656e 636f 6469  TH, "r+", encodi
+0000d9a0: 6e67 3d22 7574 662d 3822 2920 6173 2073  ng="utf-8") as s
+0000d9b0: 7461 7473 5f66 696c 653a 0a20 2020 2020  tats_file:.     
+0000d9c0: 2020 2020 2020 206c 696e 6573 203d 2073         lines = s
+0000d9d0: 7461 7473 5f66 696c 652e 7265 6164 6c69  tats_file.readli
+0000d9e0: 6e65 7328 290a 2020 2020 2020 2020 2020  nes().          
+0000d9f0: 2020 666f 7220 6a20 696e 2072 616e 6765    for j in range
+0000da00: 286c 656e 286c 696e 6573 2929 3a0a 2020  (len(lines)):.  
+0000da10: 2020 2020 2020 2020 2020 2020 2020 736f                so
+0000da20: 6e67 5f69 642c 206c 6973 7465 6e65 6420  ng_id, listened 
+0000da30: 3d20 6c69 6e65 735b 6a5d 2e73 7472 6970  = lines[j].strip
+0000da40: 2829 2e73 706c 6974 2822 7c22 290a 2020  ().split("|").  
+0000da50: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000da60: 2073 6f6e 675f 6964 203d 3d20 706c 6179   song_id == play
+0000da70: 6572 5f6f 7574 7075 742e 706c 6179 6c69  er_output.playli
+0000da80: 7374 5b70 6c61 7965 725f 6f75 7470 7574  st[player_output
+0000da90: 2e69 5d5b 305d 3a0a 2020 2020 2020 2020  .i][0]:.        
+0000daa0: 2020 2020 2020 2020 2020 2020 6c69 7374              list
+0000dab0: 656e 6564 203d 2066 6c6f 6174 286c 6973  ened = float(lis
+0000dac0: 7465 6e65 6429 202b 2074 696d 655f 6c69  tened) + time_li
+0000dad0: 7374 656e 6564 0a20 2020 2020 2020 2020  stened.         
+0000dae0: 2020 2020 2020 2020 2020 206c 696e 6573             lines
+0000daf0: 5b6a 5d20 3d20 6622 7b73 6f6e 675f 6964  [j] = f"{song_id
+0000db00: 7d7c 7b6c 6973 7465 6e65 647d 5c6e 220a  }|{listened}\n".
+0000db10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db20: 2020 2020 6272 6561 6b0a 0a20 2020 2020      break..     
+0000db30: 2020 2020 2020 2023 2077 7269 7465 206f         # write o
+0000db40: 7574 0a20 2020 2020 2020 2020 2020 2073  ut.            s
+0000db50: 7461 7473 5f66 696c 652e 7365 656b 2830  tats_file.seek(0
+0000db60: 290a 2020 2020 2020 2020 2020 2020 7374  ).            st
+0000db70: 6174 735f 6669 6c65 2e77 7269 7465 2822  ats_file.write("
+0000db80: 222e 6a6f 696e 286c 696e 6573 2929 0a20  ".join(lines)). 
+0000db90: 2020 2020 2020 2020 2020 2073 7461 7473             stats
+0000dba0: 5f66 696c 652e 7472 756e 6361 7465 2829  _file.truncate()
+0000dbb0: 0a0a 2020 2020 2020 2020 7769 7468 206f  ..        with o
+0000dbc0: 7065 6e28 4355 525f 5945 4152 5f53 5441  pen(CUR_YEAR_STA
+0000dbd0: 5453 5f50 4154 482c 2022 722b 222c 2065  TS_PATH, "r+", e
+0000dbe0: 6e63 6f64 696e 673d 2275 7466 2d38 2229  ncoding="utf-8")
+0000dbf0: 2061 7320 7374 6174 735f 6669 6c65 3a0a   as stats_file:.
+0000dc00: 2020 2020 2020 2020 2020 2020 6c69 6e65              line
+0000dc10: 7320 3d20 7374 6174 735f 6669 6c65 2e72  s = stats_file.r
+0000dc20: 6561 646c 696e 6573 2829 0a20 2020 2020  eadlines().     
+0000dc30: 2020 2020 2020 2066 6f72 206a 2069 6e20         for j in 
+0000dc40: 7261 6e67 6528 6c65 6e28 6c69 6e65 7329  range(len(lines)
+0000dc50: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000dc60: 2020 2073 6f6e 675f 6964 2c20 6c69 7374     song_id, list
+0000dc70: 656e 6564 203d 206c 696e 6573 5b6a 5d2e  ened = lines[j].
+0000dc80: 7374 7269 7028 292e 7370 6c69 7428 227c  strip().split("|
+0000dc90: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+0000dca0: 2020 2069 6620 736f 6e67 5f69 6420 3d3d     if song_id ==
+0000dcb0: 2070 6c61 7965 725f 6f75 7470 7574 2e70   player_output.p
+0000dcc0: 6c61 796c 6973 745b 706c 6179 6572 5f6f  laylist[player_o
+0000dcd0: 7574 7075 742e 695d 5b30 5d3a 0a20 2020  utput.i][0]:.   
+0000dce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dcf0: 206c 6973 7465 6e65 6420 3d20 666c 6f61   listened = floa
+0000dd00: 7428 6c69 7374 656e 6564 2920 2b20 7469  t(listened) + ti
+0000dd10: 6d65 5f6c 6973 7465 6e65 640a 2020 2020  me_listened.    
+0000dd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd30: 6c69 6e65 735b 6a5d 203d 2066 227b 736f  lines[j] = f"{so
+0000dd40: 6e67 5f69 647d 7c7b 6c69 7374 656e 6564  ng_id}|{listened
+0000dd50: 7d5c 6e22 0a20 2020 2020 2020 2020 2020  }\n".           
+0000dd60: 2020 2020 2020 2020 2062 7265 616b 0a0a           break..
+0000dd70: 2020 2020 2020 2020 2020 2020 2320 7772              # wr
+0000dd80: 6974 6520 6f75 740a 2020 2020 2020 2020  ite out.        
+0000dd90: 2020 2020 7374 6174 735f 6669 6c65 2e73      stats_file.s
+0000dda0: 6565 6b28 3029 0a20 2020 2020 2020 2020  eek(0).         
+0000ddb0: 2020 2073 7461 7473 5f66 696c 652e 7772     stats_file.wr
+0000ddc0: 6974 6528 2222 2e6a 6f69 6e28 6c69 6e65  ite("".join(line
+0000ddd0: 7329 290a 2020 2020 2020 2020 2020 2020  s)).            
+0000dde0: 7374 6174 735f 6669 6c65 2e74 7275 6e63  stats_file.trunc
+0000ddf0: 6174 6528 290a 2020 2020 2020 2020 2320  ate().        # 
+0000de00: 656e 6472 6567 696f 6e0a 0a20 2020 2020  endregion..     
+0000de10: 2020 2069 6620 706c 6179 6572 5f6f 7574     if player_out
+0000de20: 7075 742e 656e 6469 6e67 3a0a 2020 2020  put.ending:.    
+0000de30: 2020 2020 2020 2020 7265 7475 726e 0a0a          return..
+0000de40: 2020 2020 2020 2020 6966 206e 6578 745f          if next_
+0000de50: 736f 6e67 203d 3d20 2d31 3a0a 2020 2020  song == -1:.    
+0000de60: 2020 2020 2020 2020 6966 2070 6c61 7965          if playe
+0000de70: 725f 6f75 7470 7574 2e69 203d 3d20 706c  r_output.i == pl
+0000de80: 6179 6572 5f6f 7574 7075 742e 7363 726f  ayer_output.scro
+0000de90: 6c6c 6572 2e70 6f73 3a0a 2020 2020 2020  ller.pos:.      
+0000dea0: 2020 2020 2020 2020 2020 706c 6179 6572            player
+0000deb0: 5f6f 7574 7075 742e 7363 726f 6c6c 6572  _output.scroller
+0000dec0: 2e73 6372 6f6c 6c5f 6261 636b 7761 7264  .scroll_backward
+0000ded0: 2829 0a20 2020 2020 2020 2020 2020 2070  ().            p
+0000dee0: 6c61 7965 725f 6f75 7470 7574 2e69 202d  layer_output.i -
+0000def0: 3d20 310a 2020 2020 2020 2020 656c 6966  = 1.        elif
+0000df00: 206e 6578 745f 736f 6e67 203d 3d20 313a   next_song == 1:
+0000df10: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000df20: 706c 6179 6572 5f6f 7574 7075 742e 6920  player_output.i 
+0000df30: 3d3d 206c 656e 2870 6c61 7965 725f 6f75  == len(player_ou
+0000df40: 7470 7574 2e70 6c61 796c 6973 7429 202d  tput.playlist) -
+0000df50: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
+0000df60: 2020 2020 6966 206c 6f6f 703a 0a20 2020      if loop:.   
+0000df70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000df80: 206e 6578 745f 6e65 7874 5f70 6c61 796c   next_next_playl
+0000df90: 6973 7420 3d20 6e65 7874 5f70 6c61 796c  ist = next_playl
+0000dfa0: 6973 745b 3a5d 0a20 2020 2020 2020 2020  ist[:].         
+0000dfb0: 2020 2020 2020 2020 2020 2069 6620 7265             if re
+0000dfc0: 7368 7566 666c 653a 0a20 2020 2020 2020  shuffle:.       
+0000dfd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dfe0: 2073 6875 6666 6c65 286e 6578 745f 6e65   shuffle(next_ne
+0000dff0: 7874 5f70 6c61 796c 6973 7429 0a20 2020  xt_playlist).   
+0000e000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e010: 2070 6c61 7965 725f 6f75 7470 7574 2e70   player_output.p
+0000e020: 6c61 796c 6973 742c 206e 6578 745f 706c  laylist, next_pl
+0000e030: 6179 6c69 7374 203d 2028 0a20 2020 2020  aylist = (.     
+0000e040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e050: 2020 206e 6578 745f 706c 6179 6c69 7374     next_playlist
+0000e060: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000e070: 2020 2020 2020 2020 2020 6e65 7874 5f6e            next_n
+0000e080: 6578 745f 706c 6179 6c69 7374 2c0a 2020  ext_playlist,.  
+0000e090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e0a0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+0000e0b0: 2020 2020 2020 2020 706c 6179 6572 5f6f          player_o
+0000e0c0: 7574 7075 742e 6920 3d20 2d31 0a20 2020  utput.i = -1.   
+0000e0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e0e0: 2070 6c61 7965 725f 6f75 7470 7574 2e73   player_output.s
+0000e0f0: 6372 6f6c 6c65 722e 706f 7320 3d20 300a  croller.pos = 0.
+0000e100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e110: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000e120: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000e130: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+0000e140: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0000e150: 2020 2069 6620 706c 6179 6572 5f6f 7574     if player_out
+0000e160: 7075 742e 6920 3d3d 2070 6c61 7965 725f  put.i == player_
+0000e170: 6f75 7470 7574 2e73 6372 6f6c 6c65 722e  output.scroller.
+0000e180: 706f 733a 0a20 2020 2020 2020 2020 2020  pos:.           
+0000e190: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
+0000e1a0: 6f75 7470 7574 2e73 6372 6f6c 6c65 722e  output.scroller.
+0000e1b0: 7363 726f 6c6c 5f66 6f72 7761 7264 2829  scroll_forward()
+0000e1c0: 0a20 2020 2020 2020 2020 2020 2070 6c61  .            pla
+0000e1d0: 7965 725f 6f75 7470 7574 2e69 202b 3d20  yer_output.i += 
+0000e1e0: 310a 2020 2020 2020 2020 656c 6966 206e  1.        elif n
+0000e1f0: 6578 745f 736f 6e67 203d 3d20 303a 0a20  ext_song == 0:. 
+0000e200: 2020 2020 2020 2020 2020 2069 6620 706c             if pl
+0000e210: 6179 6572 5f6f 7574 7075 742e 6c6f 6f70  ayer_output.loop
+0000e220: 696e 675f 6375 7272 656e 745f 736f 6e67  ing_current_song
+0000e230: 203d 3d20 4c4f 4f50 5f4d 4f44 4553 5b22   == LOOP_MODES["
+0000e240: 6f6e 6522 5d3a 0a20 2020 2020 2020 2020  one"]:.         
+0000e250: 2020 2020 2020 2070 7269 6e74 5f74 6f5f         print_to_
+0000e260: 6c6f 6766 696c 6528 0a20 2020 2020 2020  logfile(.       
+0000e270: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
+0000e280: 7965 725f 6f75 7470 7574 2e6c 6f6f 7069  yer_output.loopi
+0000e290: 6e67 5f63 7572 7265 6e74 5f73 6f6e 672c  ng_current_song,
+0000e2a0: 204c 4f4f 505f 4d4f 4445 535b 226f 6e65   LOOP_MODES["one
+0000e2b0: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
+0000e2c0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+0000e2d0: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
+0000e2e0: 7574 2e6c 6f6f 7069 6e67 5f63 7572 7265  ut.looping_curre
+0000e2f0: 6e74 5f73 6f6e 6720 3d20 4c4f 4f50 5f4d  nt_song = LOOP_M
+0000e300: 4f44 4553 5b22 6e6f 6e65 225d 0a20 2020  ODES["none"].   
+0000e310: 2020 2020 2020 2020 2020 2020 2070 7269               pri
+0000e320: 6e74 5f74 6f5f 6c6f 6766 696c 6528 0a20  nt_to_logfile(. 
+0000e330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e340: 2020 2070 6c61 7965 725f 6f75 7470 7574     player_output
+0000e350: 2e6c 6f6f 7069 6e67 5f63 7572 7265 6e74  .looping_current
+0000e360: 5f73 6f6e 672c 204c 4f4f 505f 4d4f 4445  _song, LOOP_MODE
+0000e370: 535b 226e 6f6e 6522 5d0a 2020 2020 2020  S["none"].      
+0000e380: 2020 2020 2020 2020 2020 290a 0a0a 2320            )...# 
+0000e390: 656e 6472 6567 696f 6e0a 0a0a 4063 6c69  endregion...@cli
+0000e3a0: 636b 2e67 726f 7570 2863 6f6e 7465 7874  ck.group(context
+0000e3b0: 5f73 6574 7469 6e67 733d 6469 6374 2868  _settings=dict(h
+0000e3c0: 656c 705f 6f70 7469 6f6e 5f6e 616d 6573  elp_option_names
+0000e3d0: 3d5b 222d 6822 2c20 222d 2d68 656c 7022  =["-h", "--help"
+0000e3e0: 5d29 290a 6465 6620 636c 6928 293a 0a20  ])).def cli():. 
+0000e3f0: 2020 2022 2222 4120 636f 6d6d 616e 6420     """A command 
+0000e400: 6c69 6e65 2069 6e74 6572 6661 6365 2066  line interface f
+0000e410: 6f72 2070 6c61 7969 6e67 206d 7573 6963  or playing music
+0000e420: 2e22 2222 0a20 2020 2067 6c6f 6261 6c20  .""".    global 
+0000e430: 534f 4e47 535f 4449 5220 2023 2070 796c  SONGS_DIR  # pyl
+0000e440: 696e 743a 2064 6973 6162 6c65 3d67 6c6f  int: disable=glo
+0000e450: 6261 6c2d 7374 6174 656d 656e 740a 0a20  bal-statement.. 
 0000e460: 2020 2069 6620 6e6f 7420 6f73 2e70 6174     if not os.pat
-0000e470: 682e 6578 6973 7473 2853 4f4e 4753 5f49  h.exists(SONGS_I
-0000e480: 4e46 4f5f 5041 5448 293a 0a20 2020 2020  NFO_PATH):.     
-0000e490: 2020 2077 6974 6820 6f70 656e 2853 4f4e     with open(SON
-0000e4a0: 4753 5f49 4e46 4f5f 5041 5448 2c20 2278  GS_INFO_PATH, "x
-0000e4b0: 222c 2065 6e63 6f64 696e 673d 2275 7466  ", encoding="utf
-0000e4c0: 2d38 2229 2061 7320 5f3a 0a20 2020 2020  -8") as _:.     
-0000e4d0: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
-0000e4e0: 2069 6620 6e6f 7420 6f73 2e70 6174 682e   if not os.path.
-0000e4f0: 6578 6973 7473 2853 5441 5453 5f44 4952  exists(STATS_DIR
-0000e500: 293a 0a20 2020 2020 2020 206f 732e 6d61  ):.        os.ma
-0000e510: 6b65 6469 7273 2853 5441 5453 5f44 4952  kedirs(STATS_DIR
-0000e520: 290a 2020 2020 6966 206e 6f74 206f 732e  ).    if not os.
-0000e530: 7061 7468 2e65 7869 7374 7328 544f 5441  path.exists(TOTA
-0000e540: 4c5f 5354 4154 535f 5041 5448 293a 0a20  L_STATS_PATH):. 
-0000e550: 2020 2020 2020 2077 6974 6820 280a 2020         with (.  
-0000e560: 2020 2020 2020 2020 2020 6f70 656e 2854            open(T
-0000e570: 4f54 414c 5f53 5441 5453 5f50 4154 482c  OTAL_STATS_PATH,
-0000e580: 2022 7722 2c20 656e 636f 6469 6e67 3d22   "w", encoding="
-0000e590: 7574 662d 3822 2920 6173 2066 2c0a 2020  utf-8") as f,.  
-0000e5a0: 2020 2020 2020 2020 2020 6f70 656e 2853            open(S
-0000e5b0: 4f4e 4753 5f49 4e46 4f5f 5041 5448 2c20  ONGS_INFO_PATH, 
-0000e5c0: 2272 222c 2065 6e63 6f64 696e 673d 2275  "r", encoding="u
-0000e5d0: 7466 2d38 2229 2061 7320 672c 0a20 2020  tf-8") as g,.   
-0000e5e0: 2020 2020 2029 3a0a 2020 2020 2020 2020       ):.        
-0000e5f0: 2020 2020 666f 7220 6c69 6e65 2069 6e20      for line in 
-0000e600: 673a 0a20 2020 2020 2020 2020 2020 2020  g:.             
-0000e610: 2020 2066 2e77 7269 7465 2866 227b 6c69     f.write(f"{li
-0000e620: 6e65 2e73 7472 6970 2829 2e73 706c 6974  ne.strip().split
-0000e630: 2827 7c27 295b 305d 7d7c 305c 6e22 290a  ('|')[0]}|0\n").
-0000e640: 2020 2020 6966 206e 6f74 206f 732e 7061      if not os.pa
-0000e650: 7468 2e65 7869 7374 7328 4355 525f 5945  th.exists(CUR_YE
-0000e660: 4152 5f53 5441 5453 5f50 4154 4829 3a0a  AR_STATS_PATH):.
-0000e670: 2020 2020 2020 2020 7769 7468 2028 0a20          with (. 
-0000e680: 2020 2020 2020 2020 2020 206f 7065 6e28             open(
-0000e690: 4355 525f 5945 4152 5f53 5441 5453 5f50  CUR_YEAR_STATS_P
-0000e6a0: 4154 482c 2022 7722 2c20 656e 636f 6469  ATH, "w", encodi
-0000e6b0: 6e67 3d22 7574 662d 3822 2920 6173 2066  ng="utf-8") as f
-0000e6c0: 2c0a 2020 2020 2020 2020 2020 2020 6f70  ,.            op
-0000e6d0: 656e 2853 4f4e 4753 5f49 4e46 4f5f 5041  en(SONGS_INFO_PA
-0000e6e0: 5448 2c20 2272 222c 2065 6e63 6f64 696e  TH, "r", encodin
-0000e6f0: 673d 2275 7466 2d38 2229 2061 7320 672c  g="utf-8") as g,
-0000e700: 0a20 2020 2020 2020 2029 3a0a 2020 2020  .        ):.    
-0000e710: 2020 2020 2020 2020 666f 7220 6c69 6e65          for line
-0000e720: 2069 6e20 673a 0a20 2020 2020 2020 2020   in g:.         
-0000e730: 2020 2020 2020 2066 2e77 7269 7465 2866         f.write(f
-0000e740: 227b 6c69 6e65 2e73 7472 6970 2829 2e73  "{line.strip().s
-0000e750: 706c 6974 2827 7c27 295b 305d 7d7c 305c  plit('|')[0]}|0\
-0000e760: 6e22 290a 0a0a 4063 6c69 2e63 6f6d 6d61  n")...@cli.comma
-0000e770: 6e64 2829 0a40 636c 6963 6b2e 6172 6775  nd().@click.argu
-0000e780: 6d65 6e74 2822 7061 7468 5f22 2c20 6d65  ment("path_", me
-0000e790: 7461 7661 723d 2250 4154 485f 4f52 5f55  tavar="PATH_OR_U
-0000e7a0: 524c 2229 0a40 636c 6963 6b2e 6172 6775  RL").@click.argu
-0000e7b0: 6d65 6e74 2822 7461 6773 222c 206e 6172  ment("tags", nar
-0000e7c0: 6773 3d2d 3129 0a40 636c 6963 6b2e 6f70  gs=-1).@click.op
-0000e7d0: 7469 6f6e 280a 2020 2020 222d 4d2f 2d6e  tion(.    "-M/-n
-0000e7e0: 4d22 2c0a 2020 2020 222d 2d6d 6f76 652f  M",.    "--move/
-0000e7f0: 2d2d 6e6f 2d6d 6f76 6522 2c0a 2020 2020  --no-move",.    
-0000e800: 226d 6f76 655f 222c 0a20 2020 2064 6566  "move_",.    def
-0000e810: 6175 6c74 3d46 616c 7365 2c0a 2020 2020  ault=False,.    
-0000e820: 6865 6c70 3d22 4d6f 7665 2066 696c 6520  help="Move file 
-0000e830: 6672 6f6d 2050 4154 4820 746f 206d 6165  from PATH to mae
-0000e840: 7374 726f 2773 2069 6e74 6572 6e61 6c20  stro's internal 
-0000e850: 736f 6e67 2064 6174 6162 6173 6520 696e  song database in
-0000e860: 7374 6561 6420 6f66 2063 6f70 7969 6e67  stead of copying
-0000e870: 2e22 2c0a 290a 4063 6c69 636b 2e6f 7074  .",.).@click.opt
-0000e880: 696f 6e28 0a20 2020 2022 2d6e 222c 0a20  ion(.    "-n",. 
-0000e890: 2020 2022 2d2d 6e61 6d65 222c 0a20 2020     "--name",.   
-0000e8a0: 2074 7970 653d 7374 722c 0a20 2020 2068   type=str,.    h
-0000e8b0: 656c 703d 2257 6861 7420 746f 206e 616d  elp="What to nam
-0000e8c0: 6520 7468 6520 736f 6e67 2c20 6966 2079  e the song, if y
-0000e8d0: 6f75 2064 6f6e 2774 2077 616e 7420 746f  ou don't want to
-0000e8e0: 2075 7365 2074 6865 2074 6974 6c65 2066   use the title f
-0000e8f0: 726f 6d20 596f 7574 7562 652f 5370 6f74  rom Youtube/Spot
-0000e900: 6966 7920 6f72 2066 696c 656e 616d 652e  ify or filename.
-0000e910: 2044 6f20 6e6f 7420 696e 636c 7564 6520   Do not include 
-0000e920: 616e 2065 7874 656e 7369 6f6e 2028 652e  an extension (e.
-0000e930: 672e 2027 2e77 6176 2729 2e20 4967 6e6f  g. '.wav'). Igno
-0000e940: 7265 6420 6966 2061 6464 696e 6720 6d75  red if adding mu
-0000e950: 6c74 6970 6c65 2073 6f6e 6773 2e22 2c0a  ltiple songs.",.
-0000e960: 290a 4063 6c69 636b 2e6f 7074 696f 6e28  ).@click.option(
-0000e970: 0a20 2020 2022 2d52 2c20 2d6e 5222 2c0a  .    "-R, -nR",.
-0000e980: 2020 2020 222d 2d72 6563 7572 7369 7665      "--recursive
-0000e990: 2f2d 2d6e 6f2d 7265 6375 7273 6976 6522  /--no-recursive"
-0000e9a0: 2c0a 2020 2020 2272 6563 7572 7365 222c  ,.    "recurse",
-0000e9b0: 0a20 2020 2064 6566 6175 6c74 3d46 616c  .    default=Fal
-0000e9c0: 7365 2c0a 2020 2020 6865 6c70 3d22 4966  se,.    help="If
-0000e9d0: 2050 4154 4820 6973 2061 2066 6f6c 6465   PATH is a folde
-0000e9e0: 722c 2061 6464 2073 6f6e 6773 2069 6e20  r, add songs in 
-0000e9f0: 7375 6266 6f6c 6465 7273 2e22 2c0a 290a  subfolders.",.).
-0000ea00: 4063 6c69 636b 2e6f 7074 696f 6e28 0a20  @click.option(. 
-0000ea10: 2020 2022 2d59 2f2d 6e59 222c 0a20 2020     "-Y/-nY",.   
-0000ea20: 2022 2d2d 796f 7574 7562 652f 2d2d 6e6f   "--youtube/--no
-0000ea30: 2d79 6f75 7475 6265 222c 0a20 2020 2064  -youtube",.    d
-0000ea40: 6566 6175 6c74 3d46 616c 7365 2c0a 2020  efault=False,.  
-0000ea50: 2020 6865 6c70 3d22 4164 6420 6120 736f    help="Add a so
-0000ea60: 6e67 2066 726f 6d20 6120 596f 7554 7562  ng from a YouTub
-0000ea70: 6520 6f72 2059 6f75 5475 6265 204d 7573  e or YouTube Mus
-0000ea80: 6963 2055 524c 2e22 2c0a 290a 4063 6c69  ic URL.",.).@cli
-0000ea90: 636b 2e6f 7074 696f 6e28 0a20 2020 2022  ck.option(.    "
-0000eaa0: 2d53 2f2d 6e53 222c 0a20 2020 2022 2d2d  -S/-nS",.    "--
-0000eab0: 7370 6f74 6966 792f 2d2d 6e6f 2d73 706f  spotify/--no-spo
-0000eac0: 7469 6679 222c 0a20 2020 2064 6566 6175  tify",.    defau
-0000ead0: 6c74 3d46 616c 7365 2c0a 2020 2020 6865  lt=False,.    he
-0000eae0: 6c70 3d22 4164 6420 6120 736f 6e67 2066  lp="Add a song f
-0000eaf0: 726f 6d20 5370 6f74 6966 7920 2874 7261  rom Spotify (tra
-0000eb00: 636b 2055 524c 2c20 616c 6275 6d20 5552  ck URL, album UR
-0000eb10: 4c2c 2070 6c61 796c 6973 7420 5552 4c2c  L, playlist URL,
-0000eb20: 2061 7274 6973 7420 5552 4c2c 206f 7220   artist URL, or 
-0000eb30: 7365 6172 6368 2071 7565 7279 292e 222c  search query).",
-0000eb40: 0a29 0a40 636c 6963 6b2e 6f70 7469 6f6e  .).@click.option
-0000eb50: 280a 2020 2020 222d 6622 2c0a 2020 2020  (.    "-f",.    
-0000eb60: 222d 2d66 6f72 6d61 7422 2c0a 2020 2020  "--format",.    
-0000eb70: 2266 6f72 6d61 745f 222c 0a20 2020 2074  "format_",.    t
-0000eb80: 7970 653d 636c 6963 6b2e 4368 6f69 6365  ype=click.Choice
-0000eb90: 285b 2277 6176 222c 2022 6d70 3322 2c20  (["wav", "mp3", 
-0000eba0: 2266 6c61 6322 2c20 226f 6767 225d 292c  "flac", "ogg"]),
-0000ebb0: 0a20 2020 2068 656c 703d 2253 7065 6369  .    help="Speci
-0000ebc0: 6679 2074 6865 2066 6f72 6d61 7420 6f66  fy the format of
-0000ebd0: 2074 6865 2073 6f6e 6720 6966 2064 6f77   the song if dow
-0000ebe0: 6e6c 6f61 6469 6e67 2066 726f 6d20 596f  nloading from Yo
-0000ebf0: 7554 7562 652c 2059 6f75 5475 6265 204d  uTube, YouTube M
-0000ec00: 7573 6963 2c20 6f72 2053 706f 7469 6679  usic, or Spotify
-0000ec10: 2055 524c 2e22 2c0a 2020 2020 6465 6661   URL.",.    defa
-0000ec20: 756c 743d 2266 6c61 6322 2c0a 2020 2020  ult="flac",.    
-0000ec30: 7368 6f77 5f64 6566 6175 6c74 3d54 7275  show_default=Tru
-0000ec40: 652c 0a29 0a40 636c 6963 6b2e 6f70 7469  e,.).@click.opti
-0000ec50: 6f6e 280a 2020 2020 222d 6322 2c0a 2020  on(.    "-c",.  
-0000ec60: 2020 222d 2d63 6c69 7022 2c0a 2020 2020    "--clip",.    
-0000ec70: 6e61 7267 733d 322c 0a20 2020 2074 7970  nargs=2,.    typ
-0000ec80: 653d 666c 6f61 742c 0a20 2020 2068 656c  e=float,.    hel
-0000ec90: 703d 2241 6464 2061 2063 6c69 702e 2049  p="Add a clip. I
-0000eca0: 676e 6f72 6564 2069 6620 6164 6469 6e67  gnored if adding
-0000ecb0: 206d 756c 7469 706c 6520 736f 6e67 732e   multiple songs.
-0000ecc0: 222c 0a29 0a40 636c 6963 6b2e 6f70 7469  ",.).@click.opti
-0000ecd0: 6f6e 280a 2020 2020 222d 502f 2d6e 5022  on(.    "-P/-nP"
-0000ece0: 2c0a 2020 2020 222d 2d70 6c61 796c 6973  ,.    "--playlis
-0000ecf0: 742f 2d2d 6e6f 2d70 6c61 796c 6973 7422  t/--no-playlist"
-0000ed00: 2c0a 2020 2020 2270 6c61 796c 6973 745f  ,.    "playlist_
-0000ed10: 222c 0a20 2020 2064 6566 6175 6c74 3d46  ",.    default=F
-0000ed20: 616c 7365 2c0a 2020 2020 6865 6c70 3d22  alse,.    help="
-0000ed30: 4966 2073 6f6e 6720 5552 4c20 7061 7373  If song URL pass
-0000ed40: 6564 2069 7320 6672 6f6d 2061 2059 6f75  ed is from a You
-0000ed50: 5475 6265 2070 6c61 796c 6973 742c 2064  Tube playlist, d
-0000ed60: 6f77 6e6c 6f61 6420 616c 6c20 7468 6520  ownload all the 
-0000ed70: 736f 6e67 732e 2049 6620 7468 6520 5552  songs. If the UR
-0000ed80: 4c20 706f 696e 7473 2064 6972 6563 746c  L points directl
-0000ed90: 7920 746f 2061 2070 6c61 796c 6973 742c  y to a playlist,
-0000eda0: 2074 6869 7320 666c 6167 2069 7320 756e   this flag is un
-0000edb0: 6e63 6573 7361 7279 2e22 2c0a 290a 4063  ncessary.",.).@c
-0000edc0: 6c69 636b 2e6f 7074 696f 6e28 0a20 2020  lick.option(.   
-0000edd0: 2022 2d6d 222c 0a20 2020 2022 2d2d 6d65   "-m",.    "--me
-0000ede0: 7461 6461 7461 222c 0a20 2020 2022 6d65  tadata",.    "me
-0000edf0: 7461 6461 7461 5f70 6169 7273 222c 0a20  tadata_pairs",. 
-0000ee00: 2020 2064 6566 6175 6c74 3d4e 6f6e 652c     default=None,
-0000ee10: 0a20 2020 2068 656c 703d 2241 6464 206d  .    help="Add m
-0000ee20: 6574 6164 6174 6120 746f 2074 6865 2073  etadata to the s
-0000ee30: 6f6e 672e 2049 676e 6f72 6564 2069 6620  ong. Ignored if 
-0000ee40: 6164 6469 6e67 206d 756c 7469 706c 6520  adding multiple 
-0000ee50: 736f 6e67 732e 2054 6865 2066 6f72 6d61  songs. The forma
-0000ee60: 7420 6973 2027 6b65 7931 3a76 616c 7565  t is 'key1:value
-0000ee70: 317c 6b65 7932 3a76 616c 7565 327c 2e2e  1|key2:value2|..
-0000ee80: 2e27 2e22 2c0a 290a 6465 6620 6164 6428  .'.",.).def add(
-0000ee90: 0a20 2020 2070 6174 685f 2c0a 2020 2020  .    path_,.    
-0000eea0: 7461 6773 2c0a 2020 2020 6d6f 7665 5f2c  tags,.    move_,
-0000eeb0: 0a20 2020 206e 616d 652c 0a20 2020 2072  .    name,.    r
-0000eec0: 6563 7572 7365 2c0a 2020 2020 796f 7574  ecurse,.    yout
-0000eed0: 7562 652c 0a20 2020 2073 706f 7469 6679  ube,.    spotify
-0000eee0: 2c0a 2020 2020 666f 726d 6174 5f2c 0a20  ,.    format_,. 
-0000eef0: 2020 2063 6c69 702c 0a20 2020 2070 6c61     clip,.    pla
-0000ef00: 796c 6973 745f 2c0a 2020 2020 6d65 7461  ylist_,.    meta
-0000ef10: 6461 7461 5f70 6169 7273 2c0a 293a 0a20  data_pairs,.):. 
-0000ef20: 2020 2022 2222 0a20 2020 2041 6464 2061     """.    Add a
-0000ef30: 206e 6577 2073 6f6e 672e 0a0a 2020 2020   new song...    
-0000ef40: 4164 6473 2074 6865 2061 7564 696f 2066  Adds the audio f
-0000ef50: 696c 6520 6c6f 6361 7465 6420 6174 2050  ile located at P
-0000ef60: 4154 482e 2049 6620 5041 5448 2069 7320  ATH. If PATH is 
-0000ef70: 6120 666f 6c64 6572 2c20 6164 6473 2061  a folder, adds a
-0000ef80: 6c6c 2066 696c 6573 0a20 2020 2069 6e20  ll files.    in 
-0000ef90: 5041 5448 2028 696e 636c 7564 696e 6720  PATH (including 
-0000efa0: 6669 6c65 7320 696e 2073 7562 666f 6c64  files in subfold
-0000efb0: 6572 7320 6966 2027 2d72 2720 6973 2070  ers if '-r' is p
-0000efc0: 6173 7365 6429 2e20 5468 6520 6e61 6d65  assed). The name
-0000efd0: 206f 6620 6561 6368 0a20 2020 2073 6f6e   of each.    son
-0000efe0: 6720 7769 6c6c 2062 6520 7468 6520 6669  g will be the fi
-0000eff0: 6c65 6e61 6d65 2028 756e 6c65 7373 2027  lename (unless '
-0000f000: 2d6e 2720 6973 2070 6173 7365 6429 2e20  -n' is passed). 
-0000f010: 4669 6c65 6e61 6d65 7320 616e 6420 7461  Filenames and ta
-0000f020: 6773 2063 616e 6e6f 740a 2020 2020 636f  gs cannot.    co
-0000f030: 6e74 6169 6e20 7468 6520 6368 6172 6163  ntain the charac
-0000f040: 7465 7220 277c 272c 2061 6e64 2074 6167  ter '|', and tag
-0000f050: 7320 6361 6e6e 6f74 2063 6f6e 7461 696e  s cannot contain
-0000f060: 2027 2c27 2e0a 0a20 2020 2049 6620 7468   ','...    If th
-0000f070: 6520 272d 5927 206f 7220 272d 2d79 6f75  e '-Y' or '--you
-0000f080: 7475 6265 2720 666c 6167 2069 7320 7061  tube' flag is pa
-0000f090: 7373 6564 2c20 5041 5448 2069 7320 7472  ssed, PATH is tr
-0000f0a0: 6561 7465 6420 6173 2061 2059 6f75 5475  eated as a YouTu
-0000f0b0: 6265 206f 720a 2020 2020 596f 7554 7562  be or.    YouTub
-0000f0c0: 6520 4d75 7369 6320 5552 4c20 696e 7374  e Music URL inst
-0000f0d0: 6561 6420 6f66 2061 2066 696c 6520 7061  ead of a file pa
-0000f0e0: 7468 2e0a 0a20 2020 2049 6620 7468 6520  th...    If the 
-0000f0f0: 272d 5327 206f 7220 272d 2d73 706f 7469  '-S' or '--spoti
-0000f100: 6679 2720 666c 6167 2069 7320 7061 7373  fy' flag is pass
-0000f110: 6564 2c20 5041 5448 2069 7320 7472 6561  ed, PATH is trea
-0000f120: 7465 6420 6173 2061 2053 706f 7469 6679  ted as a Spotify
-0000f130: 0a20 2020 2074 7261 636b 2055 524c 2c20  .    track URL, 
-0000f140: 616c 6275 6d20 5552 4c2c 2070 6c61 796c  album URL, playl
-0000f150: 6973 7420 5552 4c2c 2061 7274 6973 7420  ist URL, artist 
-0000f160: 5552 4c2c 206f 7220 7365 6172 6368 2071  URL, or search q
-0000f170: 7565 7279 2069 6e73 7465 6164 206f 660a  uery instead of.
-0000f180: 2020 2020 6120 6669 6c65 2070 6174 682e      a file path.
-0000f190: 0a0a 2020 2020 5468 6520 272d 632f 2d2d  ..    The '-c/--
-0000f1a0: 636c 6970 2720 6f70 7469 6f6e 2063 616e  clip' option can
-0000f1b0: 2062 6520 7573 6564 2074 6f20 6164 6420   be used to add 
-0000f1c0: 6120 636c 6970 2066 6f72 2074 6865 2073  a clip for the s
-0000f1d0: 6f6e 672e 2049 7420 7461 6b65 7320 7477  ong. It takes tw
-0000f1e0: 6f0a 2020 2020 6172 6775 6d65 6e74 732c  o.    arguments,
-0000f1f0: 2062 7574 2075 6e6c 696b 6520 276d 6165   but unlike 'mae
-0000f200: 7374 726f 2063 6c69 7027 2c20 796f 7520  stro clip', you 
-0000f210: 6361 6e6e 6f74 2070 6173 7320 6f6e 6c79  cannot pass only
-0000f220: 2074 6865 2073 7461 7274 2074 696d 650a   the start time.
-0000f230: 2020 2020 616e 6420 6e6f 7420 7468 6520      and not the 
-0000f240: 656e 642e 2054 6f20 6765 7420 6172 6f75  end. To get arou
-0000f250: 6e64 2074 6869 732c 2079 6f75 2063 616e  nd this, you can
-0000f260: 2070 6173 7320 2d31 2061 7320 7468 6520   pass -1 as the 
-0000f270: 656e 6420 7469 6d65 2c20 652e 672e 0a20  end time, e.g.. 
-0000f280: 2020 2027 6d61 6573 7472 6f20 6164 6420     'maestro add 
-0000f290: 2d63 2033 3020 2d31 2068 7474 7073 3a2f  -c 30 -1 https:/
-0000f2a0: 2f77 7777 2e79 6f75 7475 6265 2e63 6f6d  /www.youtube.com
-0000f2b0: 2f77 6174 6368 3f76 3d33 5678 754d 4572  /watch?v=3VxuMEr
-0000f2c0: 4364 2d45 202d 7927 2e20 4966 0a20 2020  Cd-E -y'. If.   
-0000f2d0: 2061 6464 696e 6720 6d75 6c74 6970 6c65   adding multiple
-0000f2e0: 2073 6f6e 6773 2c20 7468 6973 206f 7074   songs, this opt
-0000f2f0: 696f 6e20 6361 6e6e 6f74 2062 6520 7573  ion cannot be us
-0000f300: 6564 2e0a 0a20 2020 2054 6865 2027 2d6d  ed...    The '-m
-0000f310: 2f2d 2d6d 6574 6164 6174 6127 206f 7074  /--metadata' opt
-0000f320: 696f 6e20 6361 6e20 6265 2075 7365 6420  ion can be used 
-0000f330: 746f 2061 6464 206d 6574 6164 6174 6120  to add metadata 
-0000f340: 746f 2074 6865 2073 6f6e 672e 2049 7420  to the song. It 
-0000f350: 7461 6b65 730a 2020 2020 6120 7374 7269  takes.    a stri
-0000f360: 6e67 206f 6620 7468 6520 666f 726d 6174  ng of the format
-0000f370: 2027 6b65 7931 3a76 616c 7565 317c 6b65   'key1:value1|ke
-0000f380: 7932 3a76 616c 7565 327c 2e2e 2e27 2e20  y2:value2|...'. 
-0000f390: 4966 2061 6464 696e 6720 6d75 6c74 6970  If adding multip
-0000f3a0: 6c65 0a20 2020 2073 6f6e 6773 2c20 7468  le.    songs, th
-0000f3b0: 6973 206f 7074 696f 6e20 6361 6e6e 6f74  is option cannot
-0000f3c0: 2062 6520 7573 6564 2e0a 0a20 2020 2050   be used...    P
-0000f3d0: 6f73 7369 626c 6520 6564 6974 6162 6c65  ossible editable
-0000f3e0: 206d 6574 6164 6174 6120 6b65 7973 2061   metadata keys a
-0000f3f0: 7265 3a20 616c 6275 6d2c 2061 6c62 756d  re: album, album
-0000f400: 6172 7469 7374 2c20 6172 7469 7374 2c20  artist, artist, 
-0000f410: 6172 7477 6f72 6b2c 0a20 2020 2063 6f6d  artwork,.    com
-0000f420: 6d65 6e74 2c20 636f 6d70 696c 6174 696f  ment, compilatio
-0000f430: 6e2c 2063 6f6d 706f 7365 722c 2064 6973  n, composer, dis
-0000f440: 636e 756d 6265 722c 2067 656e 7265 2c20  cnumber, genre, 
-0000f450: 6c79 7269 6373 2c20 746f 7461 6c64 6973  lyrics, totaldis
-0000f460: 6373 2c0a 2020 2020 746f 7461 6c74 7261  cs,.    totaltra
-0000f470: 636b 732c 2074 7261 636b 6e75 6d62 6572  cks, tracknumber
-0000f480: 2c20 7472 6163 6b74 6974 6c65 2c20 7965  , tracktitle, ye
-0000f490: 6172 2c20 6973 7263 0a0a 2020 2020 4b65  ar, isrc..    Ke
-0000f4a0: 7973 2061 7265 206e 6f74 2063 6173 6520  ys are not case 
-0000f4b0: 7365 6e73 6974 6976 6520 616e 6420 6361  sensitive and ca
-0000f4c0: 6e20 636f 6e74 6169 6e20 6172 6269 7472  n contain arbitr
-0000f4d0: 6172 7920 7768 6974 6573 7061 6365 2c20  ary whitespace, 
-0000f4e0: 272d 272c 2061 6e64 0a20 2020 2027 5f27  '-', and.    '_'
-0000f4f0: 2063 6861 7261 6374 6572 732e 2049 6e20   characters. In 
-0000f500: 6f74 6865 7220 776f 7264 732c 2027 416c  other words, 'Al
-0000f510: 6275 6d20 4172 7469 7374 272c 2027 616c  bum Artist', 'al
-0000f520: 6275 6d2d 6172 7469 7374 272c 2061 6e64  bum-artist', and
-0000f530: 0a20 2020 2027 616c 6275 6d5f 6172 7469  .    'album_arti
-0000f540: 7374 2720 6172 6520 616c 6c20 7379 6e6f  st' are all syno
-0000f550: 6e79 6d73 2066 6f72 2027 616c 6275 6d61  nyms for 'albuma
-0000f560: 7274 6973 7427 2e20 416c 736f 2c20 2764  rtist'. Also, 'd
-0000f570: 6973 6b27 2069 730a 2020 2020 7379 6e6f  isk' is.    syno
-0000f580: 6e79 6d6f 7573 2077 6974 6820 2764 6973  nymous with 'dis
-0000f590: 6327 2e0a 2020 2020 2222 220a 0a20 2020  c'..    """..   
-0000f5a0: 2070 6174 6873 203d 204e 6f6e 650a 2020   paths = None.  
-0000f5b0: 2020 6966 206e 6f74 2028 796f 7574 7562    if not (youtub
-0000f5c0: 6520 6f72 2073 706f 7469 6679 2920 616e  e or spotify) an
-0000f5d0: 6420 6e6f 7420 6f73 2e70 6174 682e 6578  d not os.path.ex
-0000f5e0: 6973 7473 2870 6174 685f 293a 0a20 2020  ists(path_):.   
-0000f5f0: 2020 2020 2063 6c69 636b 2e73 6563 686f       click.secho
-0000f600: 280a 2020 2020 2020 2020 2020 2020 6622  (.            f"
-0000f610: 5468 6520 7061 7468 2027 7b70 6174 685f  The path '{path_
-0000f620: 7d27 2064 6f65 7320 6e6f 7420 6578 6973  }' does not exis
-0000f630: 742e 2054 6f20 646f 776e 6c6f 6164 2066  t. To download f
-0000f640: 726f 6d20 6120 596f 7554 7562 6520 6f72  rom a YouTube or
-0000f650: 2059 6f75 5475 6265 204d 7573 6963 2055   YouTube Music U
-0000f660: 526c 2c20 7061 7373 2074 6865 2027 2d59  Rl, pass the '-Y
-0000f670: 2f2d 2d79 6f75 7475 6265 2720 666c 6167  /--youtube' flag
-0000f680: 2e20 546f 2064 6f77 6e6c 6f61 6420 6672  . To download fr
-0000f690: 6f6d 2061 2053 706f 7469 6679 2055 526c  om a Spotify URl
-0000f6a0: 2c20 7061 7373 2074 6865 2027 2d53 2f2d  , pass the '-S/-
-0000f6b0: 2d73 706f 7469 6679 2720 666c 6167 2e22  -spotify' flag."
-0000f6c0: 2c0a 2020 2020 2020 2020 2020 2020 6667  ,.            fg
-0000f6d0: 3d22 7265 6422 2c0a 2020 2020 2020 2020  ="red",.        
-0000f6e0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0000f6f0: 0a0a 2020 2020 6966 2079 6f75 7475 6265  ..    if youtube
-0000f700: 206f 7220 7370 6f74 6966 793a 0a20 2020   or spotify:.   
-0000f710: 2020 2020 2069 6620 796f 7574 7562 6520       if youtube 
-0000f720: 616e 6420 7370 6f74 6966 793a 0a20 2020  and spotify:.   
-0000f730: 2020 2020 2020 2020 2063 6c69 636b 2e73           click.s
-0000f740: 6563 686f 280a 2020 2020 2020 2020 2020  echo(.          
-0000f750: 2020 2020 2020 2243 616e 6e6f 7420 7061        "Cannot pa
-0000f760: 7373 2062 6f74 6820 272d 792f 2d2d 796f  ss both '-y/--yo
-0000f770: 7574 7562 6527 2061 6e64 2027 2d73 2f2d  utube' and '-s/-
-0000f780: 2d73 706f 7469 6679 2720 666c 6167 732e  -spotify' flags.
-0000f790: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-0000f7a0: 2020 2066 673d 2272 6564 222c 0a20 2020     fg="red",.   
-0000f7b0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0000f7c0: 2020 2020 2020 2072 6574 7572 6e0a 0a20         return.. 
-0000f7d0: 2020 2020 2020 2069 6620 796f 7574 7562         if youtub
-0000f7e0: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
-0000f7f0: 6620 666f 726d 6174 5f20 3d3d 2022 6f67  f format_ == "og
-0000f800: 6722 3a0a 2020 2020 2020 2020 2020 2020  g":.            
-0000f810: 2020 2020 636c 6963 6b2e 7365 6368 6f28      click.secho(
-0000f820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f830: 2020 2020 2022 4361 6e6e 6f74 2064 6f77       "Cannot dow
-0000f840: 6e6c 6f61 6420 736f 6e67 7320 6672 6f6d  nload songs from
-0000f850: 2059 6f75 5475 6265 2061 7320 272e 6f67   YouTube as '.og
-0000f860: 6727 2e20 506c 6561 7365 2063 686f 6f73  g'. Please choos
-0000f870: 6520 6120 6469 6666 6572 656e 7420 666f  e a different fo
-0000f880: 726d 6174 2e22 2c0a 2020 2020 2020 2020  rmat.",.        
-0000f890: 2020 2020 2020 2020 2020 2020 6667 3d22              fg="
-0000f8a0: 7265 6422 2c0a 2020 2020 2020 2020 2020  red",.          
-0000f8b0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0000f8c0: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
-0000f8d0: 2020 2020 2020 2020 2020 2073 7562 7072             subpr
-0000f8e0: 6f63 6573 732e 7275 6e28 0a20 2020 2020  ocess.run(.     
-0000f8f0: 2020 2020 2020 2020 2020 205b 0a20 2020             [.   
-0000f900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f910: 2022 7974 2d64 6c70 222c 0a20 2020 2020   "yt-dlp",.     
-0000f920: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0000f930: 6174 685f 2c0a 2020 2020 2020 2020 2020  ath_,.          
-0000f940: 2020 2020 2020 2020 2020 222d 7822 2c20            "-x", 
-0000f950: 2023 2065 7874 7261 6374 2061 7564 696f   # extract audio
-0000f960: 2028 6e65 6365 7373 6172 792c 206e 6565   (necessary, nee
-0000f970: 6473 2066 666d 7065 6729 0a20 2020 2020  ds ffmpeg).     
-0000f980: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000f990: 2d2d 6175 6469 6f2d 666f 726d 6174 222c  --audio-format",
-0000f9a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f9b0: 2020 2020 2066 6f72 6d61 745f 2c0a 2020       format_,.  
-0000f9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f9d0: 2020 222d 2d6e 6f2d 706c 6179 6c69 7374    "--no-playlist
-0000f9e0: 2220 6966 206e 6f74 2070 6c61 796c 6973  " if not playlis
-0000f9f0: 745f 2065 6c73 6520 2222 2c0a 2020 2020  t_ else "",.    
-0000fa00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fa10: 222d 2d65 6d62 6564 2d6d 6574 6164 6174  "--embed-metadat
-0000fa20: 6122 2c0a 2020 2020 2020 2020 2020 2020  a",.            
-0000fa30: 2020 2020 2020 2020 222d 6f22 2c0a 2020          "-o",.  
-0000fa40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fa50: 2020 6f73 2e70 6174 682e 6a6f 696e 284d    os.path.join(M
-0000fa60: 4145 5354 524f 5f44 4952 2c20 2225 2874  AESTRO_DIR, "%(t
-0000fa70: 6974 6c65 2973 2e25 2865 7874 2973 2229  itle)s.%(ext)s")
-0000fa80: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000fa90: 2020 5d2c 0a20 2020 2020 2020 2020 2020    ],.           
-0000faa0: 2020 2020 2063 6865 636b 3d54 7275 652c       check=True,
-0000fab0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-0000fac0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0000fad0: 2020 2020 2020 2020 2069 6620 666f 726d           if form
-0000fae0: 6174 5f20 3d3d 2022 7761 7622 3a0a 2020  at_ == "wav":.  
-0000faf0: 2020 2020 2020 2020 2020 2020 2020 636c                cl
-0000fb00: 6963 6b2e 7365 6368 6f28 0a20 2020 2020  ick.secho(.     
-0000fb10: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000fb20: 4361 6e6e 6f74 2064 6f77 6e6c 6f61 6420  Cannot download 
-0000fb30: 736f 6e67 7320 6672 6f6d 2053 706f 7469  songs from Spoti
-0000fb40: 6679 2061 7320 272e 7761 7627 2e20 506c  fy as '.wav'. Pl
-0000fb50: 6561 7365 2063 686f 6f73 6520 6120 6469  ease choose a di
-0000fb60: 6666 6572 656e 7420 666f 726d 6174 2e22  fferent format."
-0000fb70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000fb80: 2020 2020 2020 6667 3d22 7265 6422 2c0a        fg="red",.
-0000fb90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fba0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000fbb0: 2020 7265 7475 726e 0a0a 2020 2020 2020    return..      
-0000fbc0: 2020 2020 2020 6377 6420 3d20 6f73 2e67        cwd = os.g
-0000fbd0: 6574 6377 6428 290a 2020 2020 2020 2020  etcwd().        
-0000fbe0: 2020 2020 6f73 2e63 6864 6972 284d 4145      os.chdir(MAE
-0000fbf0: 5354 524f 5f44 4952 290a 2020 2020 2020  STRO_DIR).      
-0000fc00: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-0000fc10: 2020 2020 2020 2020 2020 2073 7562 7072             subpr
-0000fc20: 6f63 6573 732e 7275 6e28 0a20 2020 2020  ocess.run(.     
-0000fc30: 2020 2020 2020 2020 2020 2020 2020 205b                 [
-0000fc40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fc50: 2020 2020 2020 2020 2022 7370 6f74 646c           "spotdl
-0000fc60: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-0000fc70: 2020 2020 2020 2020 2020 2022 646f 776e             "down
-0000fc80: 6c6f 6164 222c 0a20 2020 2020 2020 2020  load",.         
-0000fc90: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0000fca0: 6174 685f 2c0a 2020 2020 2020 2020 2020  ath_,.          
-0000fcb0: 2020 2020 2020 2020 2020 2020 2020 222d                "-
-0000fcc0: 2d6f 7574 7075 7422 2c0a 2020 2020 2020  -output",.      
-0000fcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fce0: 2020 227b 7469 746c 657d 2e7b 6f75 7470    "{title}.{outp
-0000fcf0: 7574 2d65 7874 7d22 2c0a 2020 2020 2020  ut-ext}",.      
-0000fd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd10: 2020 222d 2d66 6f72 6d61 7422 2c0a 2020    "--format",.  
-0000fd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd30: 2020 2020 2020 666f 726d 6174 5f2c 0a20        format_,. 
-0000fd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd50: 2020 2020 2020 2022 2d2d 6865 6164 6c65         "--headle
-0000fd60: 7373 222c 0a20 2020 2020 2020 2020 2020  ss",.           
-0000fd70: 2020 2020 2020 2020 205d 2c0a 2020 2020           ],.    
-0000fd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd90: 6368 6563 6b3d 5472 7565 2c0a 2020 2020  check=True,.    
-0000fda0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0000fdb0: 2020 2020 2020 2020 2020 6578 6365 7074            except
-0000fdc0: 2045 7863 6570 7469 6f6e 2061 7320 6572   Exception as er
-0000fdd0: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
-0000fde0: 2020 206f 732e 6368 6469 7228 6377 6429     os.chdir(cwd)
-0000fdf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fe00: 2072 6169 7365 2065 7272 0a0a 2020 2020   raise err..    
-0000fe10: 2020 2020 7061 7468 7320 3d20 5b5d 0a20      paths = []. 
-0000fe20: 2020 2020 2020 2066 6f72 2066 6e61 6d65         for fname
-0000fe30: 2069 6e20 6f73 2e6c 6973 7464 6972 284d   in os.listdir(M
-0000fe40: 4145 5354 524f 5f44 4952 293a 0a20 2020  AESTRO_DIR):.   
-0000fe50: 2020 2020 2020 2020 2066 6f72 2066 2069           for f i
-0000fe60: 6e20 5b22 2e77 6176 222c 2022 2e6d 7033  n [".wav", ".mp3
-0000fe70: 222c 2022 2e66 6c61 6322 2c20 222e 6f67  ", ".flac", ".og
-0000fe80: 6722 5d3a 0a20 2020 2020 2020 2020 2020  g"]:.           
-0000fe90: 2020 2020 2069 6620 666e 616d 652e 656e       if fname.en
-0000fea0: 6473 7769 7468 2866 293a 0a20 2020 2020  dswith(f):.     
-0000feb0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000fec0: 6177 5f70 6174 6820 3d20 6f73 2e70 6174  aw_path = os.pat
-0000fed0: 682e 6a6f 696e 284d 4145 5354 524f 5f44  h.join(MAESTRO_D
-0000fee0: 4952 2c20 666e 616d 6529 0a20 2020 2020  IR, fname).     
+0000e470: 682e 6578 6973 7473 2853 4554 5449 4e47  h.exists(SETTING
+0000e480: 535f 4649 4c45 293a 0a20 2020 2020 2020  S_FILE):.       
+0000e490: 2077 6974 6820 6f70 656e 2853 4554 5449   with open(SETTI
+0000e4a0: 4e47 535f 4649 4c45 2c20 2278 222c 2065  NGS_FILE, "x", e
+0000e4b0: 6e63 6f64 696e 673d 2275 7466 2d38 2229  ncoding="utf-8")
+0000e4c0: 2061 7320 663a 0a20 2020 2020 2020 2020   as f:.         
+0000e4d0: 2020 206a 736f 6e2e 6475 6d70 287b 2273     json.dump({"s
+0000e4e0: 6f6e 675f 6469 7265 6374 6f72 7922 3a20  ong_directory": 
+0000e4f0: 4445 4641 554c 545f 534f 4e47 535f 4449  DEFAULT_SONGS_DI
+0000e500: 527d 2c20 6629 0a20 2020 2020 2020 2020  R}, f).         
+0000e510: 2020 2053 4f4e 4753 5f44 4952 203d 2044     SONGS_DIR = D
+0000e520: 4546 4155 4c54 5f53 4f4e 4753 5f44 4952  EFAULT_SONGS_DIR
+0000e530: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+0000e540: 2020 2077 6974 6820 6f70 656e 2853 4554     with open(SET
+0000e550: 5449 4e47 535f 4649 4c45 2c20 2272 222c  TINGS_FILE, "r",
+0000e560: 2065 6e63 6f64 696e 673d 2275 7466 2d38   encoding="utf-8
+0000e570: 2229 2061 7320 663a 0a20 2020 2020 2020  ") as f:.       
+0000e580: 2020 2020 2073 6574 7469 6e67 7320 3d20       settings = 
+0000e590: 6a73 6f6e 2e6c 6f61 6428 6629 0a20 2020  json.load(f).   
+0000e5a0: 2020 2020 2020 2020 2069 6620 2273 6f6e           if "son
+0000e5b0: 675f 6469 7265 6374 6f72 7922 206e 6f74  g_directory" not
+0000e5c0: 2069 6e20 7365 7474 696e 6773 3a0a 2020   in settings:.  
+0000e5d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000e5e0: 7474 696e 6773 5b22 736f 6e67 5f64 6972  ttings["song_dir
+0000e5f0: 6563 746f 7279 225d 203d 2044 4546 4155  ectory"] = DEFAU
+0000e600: 4c54 5f53 4f4e 4753 5f44 4952 0a20 2020  LT_SONGS_DIR.   
+0000e610: 2020 2020 2020 2020 2020 2020 2077 6974               wit
+0000e620: 6820 6f70 656e 2853 4554 5449 4e47 535f  h open(SETTINGS_
+0000e630: 4649 4c45 2c20 2277 222c 2065 6e63 6f64  FILE, "w", encod
+0000e640: 696e 673d 2275 7466 2d38 2229 2061 7320  ing="utf-8") as 
+0000e650: 673a 0a20 2020 2020 2020 2020 2020 2020  g:.             
+0000e660: 2020 2020 2020 206a 736f 6e2e 6475 6d70         json.dump
+0000e670: 2873 6574 7469 6e67 732c 2067 290a 2020  (settings, g).  
+0000e680: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+0000e690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e6a0: 6966 206e 6f74 206f 732e 7061 7468 2e65  if not os.path.e
+0000e6b0: 7869 7374 7328 7365 7474 696e 6773 5b22  xists(settings["
+0000e6c0: 736f 6e67 5f64 6972 6563 746f 7279 225d  song_directory"]
+0000e6d0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000e6e0: 2020 2020 2020 206f 732e 6d61 6b65 6469         os.makedi
+0000e6f0: 7273 2873 6574 7469 6e67 735b 2273 6f6e  rs(settings["son
+0000e700: 675f 6469 7265 6374 6f72 7922 5d29 0a20  g_directory"]). 
+0000e710: 2020 2020 2020 2020 2020 2053 4f4e 4753             SONGS
+0000e720: 5f44 4952 203d 2073 6574 7469 6e67 735b  _DIR = settings[
+0000e730: 2273 6f6e 675f 6469 7265 6374 6f72 7922  "song_directory"
+0000e740: 5d0a 0a20 2020 2069 6620 6e6f 7420 6f73  ]..    if not os
+0000e750: 2e70 6174 682e 6578 6973 7473 2853 4f4e  .path.exists(SON
+0000e760: 4753 5f49 4e46 4f5f 5041 5448 293a 0a20  GS_INFO_PATH):. 
+0000e770: 2020 2020 2020 2077 6974 6820 6f70 656e         with open
+0000e780: 2853 4f4e 4753 5f49 4e46 4f5f 5041 5448  (SONGS_INFO_PATH
+0000e790: 2c20 2278 222c 2065 6e63 6f64 696e 673d  , "x", encoding=
+0000e7a0: 2275 7466 2d38 2229 2061 7320 5f3a 0a20  "utf-8") as _:. 
+0000e7b0: 2020 2020 2020 2020 2020 2070 6173 730a             pass.
+0000e7c0: 0a20 2020 2069 6620 6e6f 7420 6f73 2e70  .    if not os.p
+0000e7d0: 6174 682e 6578 6973 7473 2853 5441 5453  ath.exists(STATS
+0000e7e0: 5f44 4952 293a 0a20 2020 2020 2020 206f  _DIR):.        o
+0000e7f0: 732e 6d61 6b65 6469 7273 2853 5441 5453  s.makedirs(STATS
+0000e800: 5f44 4952 290a 2020 2020 6966 206e 6f74  _DIR).    if not
+0000e810: 206f 732e 7061 7468 2e65 7869 7374 7328   os.path.exists(
+0000e820: 544f 5441 4c5f 5354 4154 535f 5041 5448  TOTAL_STATS_PATH
+0000e830: 293a 0a20 2020 2020 2020 2077 6974 6820  ):.        with 
+0000e840: 280a 2020 2020 2020 2020 2020 2020 6f70  (.            op
+0000e850: 656e 2854 4f54 414c 5f53 5441 5453 5f50  en(TOTAL_STATS_P
+0000e860: 4154 482c 2022 7722 2c20 656e 636f 6469  ATH, "w", encodi
+0000e870: 6e67 3d22 7574 662d 3822 2920 6173 2066  ng="utf-8") as f
+0000e880: 2c0a 2020 2020 2020 2020 2020 2020 6f70  ,.            op
+0000e890: 656e 2853 4f4e 4753 5f49 4e46 4f5f 5041  en(SONGS_INFO_PA
+0000e8a0: 5448 2c20 2272 222c 2065 6e63 6f64 696e  TH, "r", encodin
+0000e8b0: 673d 2275 7466 2d38 2229 2061 7320 672c  g="utf-8") as g,
+0000e8c0: 0a20 2020 2020 2020 2029 3a0a 2020 2020  .        ):.    
+0000e8d0: 2020 2020 2020 2020 666f 7220 6c69 6e65          for line
+0000e8e0: 2069 6e20 673a 0a20 2020 2020 2020 2020   in g:.         
+0000e8f0: 2020 2020 2020 2066 2e77 7269 7465 2866         f.write(f
+0000e900: 227b 6c69 6e65 2e73 7472 6970 2829 2e73  "{line.strip().s
+0000e910: 706c 6974 2827 7c27 295b 305d 7d7c 305c  plit('|')[0]}|0\
+0000e920: 6e22 290a 2020 2020 6966 206e 6f74 206f  n").    if not o
+0000e930: 732e 7061 7468 2e65 7869 7374 7328 4355  s.path.exists(CU
+0000e940: 525f 5945 4152 5f53 5441 5453 5f50 4154  R_YEAR_STATS_PAT
+0000e950: 4829 3a0a 2020 2020 2020 2020 7769 7468  H):.        with
+0000e960: 2028 0a20 2020 2020 2020 2020 2020 206f   (.            o
+0000e970: 7065 6e28 4355 525f 5945 4152 5f53 5441  pen(CUR_YEAR_STA
+0000e980: 5453 5f50 4154 482c 2022 7722 2c20 656e  TS_PATH, "w", en
+0000e990: 636f 6469 6e67 3d22 7574 662d 3822 2920  coding="utf-8") 
+0000e9a0: 6173 2066 2c0a 2020 2020 2020 2020 2020  as f,.          
+0000e9b0: 2020 6f70 656e 2853 4f4e 4753 5f49 4e46    open(SONGS_INF
+0000e9c0: 4f5f 5041 5448 2c20 2272 222c 2065 6e63  O_PATH, "r", enc
+0000e9d0: 6f64 696e 673d 2275 7466 2d38 2229 2061  oding="utf-8") a
+0000e9e0: 7320 672c 0a20 2020 2020 2020 2029 3a0a  s g,.        ):.
+0000e9f0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000ea00: 6c69 6e65 2069 6e20 673a 0a20 2020 2020  line in g:.     
+0000ea10: 2020 2020 2020 2020 2020 2066 2e77 7269             f.wri
+0000ea20: 7465 2866 227b 6c69 6e65 2e73 7472 6970  te(f"{line.strip
+0000ea30: 2829 2e73 706c 6974 2827 7c27 295b 305d  ().split('|')[0]
+0000ea40: 7d7c 305c 6e22 290a 0a0a 4063 6c69 2e63  }|0\n")...@cli.c
+0000ea50: 6f6d 6d61 6e64 2829 0a40 636c 6963 6b2e  ommand().@click.
+0000ea60: 6172 6775 6d65 6e74 2822 7061 7468 5f22  argument("path_"
+0000ea70: 2c20 6d65 7461 7661 723d 2250 4154 485f  , metavar="PATH_
+0000ea80: 4f52 5f55 524c 2229 0a40 636c 6963 6b2e  OR_URL").@click.
+0000ea90: 6172 6775 6d65 6e74 2822 7461 6773 222c  argument("tags",
+0000eaa0: 206e 6172 6773 3d2d 3129 0a40 636c 6963   nargs=-1).@clic
+0000eab0: 6b2e 6f70 7469 6f6e 280a 2020 2020 222d  k.option(.    "-
+0000eac0: 4d2f 2d6e 4d22 2c0a 2020 2020 222d 2d6d  M/-nM",.    "--m
+0000ead0: 6f76 652f 2d2d 6e6f 2d6d 6f76 6522 2c0a  ove/--no-move",.
+0000eae0: 2020 2020 226d 6f76 655f 222c 0a20 2020      "move_",.   
+0000eaf0: 2064 6566 6175 6c74 3d46 616c 7365 2c0a   default=False,.
+0000eb00: 2020 2020 6865 6c70 3d22 4d6f 7665 2066      help="Move f
+0000eb10: 696c 6520 6672 6f6d 2050 4154 4820 746f  ile from PATH to
+0000eb20: 206d 6165 7374 726f 2773 2069 6e74 6572   maestro's inter
+0000eb30: 6e61 6c20 736f 6e67 2064 6174 6162 6173  nal song databas
+0000eb40: 6520 696e 7374 6561 6420 6f66 2063 6f70  e instead of cop
+0000eb50: 7969 6e67 2e22 2c0a 290a 4063 6c69 636b  ying.",.).@click
+0000eb60: 2e6f 7074 696f 6e28 0a20 2020 2022 2d6e  .option(.    "-n
+0000eb70: 222c 0a20 2020 2022 2d2d 6e61 6d65 222c  ",.    "--name",
+0000eb80: 0a20 2020 2074 7970 653d 7374 722c 0a20  .    type=str,. 
+0000eb90: 2020 2068 656c 703d 2257 6861 7420 746f     help="What to
+0000eba0: 206e 616d 6520 7468 6520 736f 6e67 2c20   name the song, 
+0000ebb0: 6966 2079 6f75 2064 6f6e 2774 2077 616e  if you don't wan
+0000ebc0: 7420 746f 2075 7365 2074 6865 2074 6974  t to use the tit
+0000ebd0: 6c65 2066 726f 6d20 596f 7574 7562 652f  le from Youtube/
+0000ebe0: 5370 6f74 6966 7920 6f72 2066 696c 656e  Spotify or filen
+0000ebf0: 616d 652e 2044 6f20 6e6f 7420 696e 636c  ame. Do not incl
+0000ec00: 7564 6520 616e 2065 7874 656e 7369 6f6e  ude an extension
+0000ec10: 2028 652e 672e 2027 2e77 6176 2729 2e20   (e.g. '.wav'). 
+0000ec20: 4967 6e6f 7265 6420 6966 2061 6464 696e  Ignored if addin
+0000ec30: 6720 6d75 6c74 6970 6c65 2073 6f6e 6773  g multiple songs
+0000ec40: 2e22 2c0a 290a 4063 6c69 636b 2e6f 7074  .",.).@click.opt
+0000ec50: 696f 6e28 0a20 2020 2022 2d52 2c20 2d6e  ion(.    "-R, -n
+0000ec60: 5222 2c0a 2020 2020 222d 2d72 6563 7572  R",.    "--recur
+0000ec70: 7369 7665 2f2d 2d6e 6f2d 7265 6375 7273  sive/--no-recurs
+0000ec80: 6976 6522 2c0a 2020 2020 2272 6563 7572  ive",.    "recur
+0000ec90: 7365 222c 0a20 2020 2064 6566 6175 6c74  se",.    default
+0000eca0: 3d46 616c 7365 2c0a 2020 2020 6865 6c70  =False,.    help
+0000ecb0: 3d22 4966 2050 4154 4820 6973 2061 2066  ="If PATH is a f
+0000ecc0: 6f6c 6465 722c 2061 6464 2073 6f6e 6773  older, add songs
+0000ecd0: 2069 6e20 7375 6266 6f6c 6465 7273 2e22   in subfolders."
+0000ece0: 2c0a 290a 4063 6c69 636b 2e6f 7074 696f  ,.).@click.optio
+0000ecf0: 6e28 0a20 2020 2022 2d59 2f2d 6e59 222c  n(.    "-Y/-nY",
+0000ed00: 0a20 2020 2022 2d2d 796f 7574 7562 652f  .    "--youtube/
+0000ed10: 2d2d 6e6f 2d79 6f75 7475 6265 222c 0a20  --no-youtube",. 
+0000ed20: 2020 2064 6566 6175 6c74 3d46 616c 7365     default=False
+0000ed30: 2c0a 2020 2020 6865 6c70 3d22 4164 6420  ,.    help="Add 
+0000ed40: 6120 736f 6e67 2066 726f 6d20 6120 596f  a song from a Yo
+0000ed50: 7554 7562 6520 6f72 2059 6f75 5475 6265  uTube or YouTube
+0000ed60: 204d 7573 6963 2055 524c 2e22 2c0a 290a   Music URL.",.).
+0000ed70: 4063 6c69 636b 2e6f 7074 696f 6e28 0a20  @click.option(. 
+0000ed80: 2020 2022 2d53 2f2d 6e53 222c 0a20 2020     "-S/-nS",.   
+0000ed90: 2022 2d2d 7370 6f74 6966 792f 2d2d 6e6f   "--spotify/--no
+0000eda0: 2d73 706f 7469 6679 222c 0a20 2020 2064  -spotify",.    d
+0000edb0: 6566 6175 6c74 3d46 616c 7365 2c0a 2020  efault=False,.  
+0000edc0: 2020 6865 6c70 3d22 4164 6420 6120 736f    help="Add a so
+0000edd0: 6e67 2066 726f 6d20 5370 6f74 6966 7920  ng from Spotify 
+0000ede0: 2874 7261 636b 2055 524c 2c20 616c 6275  (track URL, albu
+0000edf0: 6d20 5552 4c2c 2070 6c61 796c 6973 7420  m URL, playlist 
+0000ee00: 5552 4c2c 2061 7274 6973 7420 5552 4c2c  URL, artist URL,
+0000ee10: 206f 7220 7365 6172 6368 2071 7565 7279   or search query
+0000ee20: 292e 222c 0a29 0a40 636c 6963 6b2e 6f70  ).",.).@click.op
+0000ee30: 7469 6f6e 280a 2020 2020 222d 6622 2c0a  tion(.    "-f",.
+0000ee40: 2020 2020 222d 2d66 6f72 6d61 7422 2c0a      "--format",.
+0000ee50: 2020 2020 2266 6f72 6d61 745f 222c 0a20      "format_",. 
+0000ee60: 2020 2074 7970 653d 636c 6963 6b2e 4368     type=click.Ch
+0000ee70: 6f69 6365 285b 2277 6176 222c 2022 6d70  oice(["wav", "mp
+0000ee80: 3322 2c20 2266 6c61 6322 2c20 226f 6767  3", "flac", "ogg
+0000ee90: 225d 292c 0a20 2020 2068 656c 703d 2253  "]),.    help="S
+0000eea0: 7065 6369 6679 2074 6865 2066 6f72 6d61  pecify the forma
+0000eeb0: 7420 6f66 2074 6865 2073 6f6e 6720 6966  t of the song if
+0000eec0: 2064 6f77 6e6c 6f61 6469 6e67 2066 726f   downloading fro
+0000eed0: 6d20 596f 7554 7562 652c 2059 6f75 5475  m YouTube, YouTu
+0000eee0: 6265 204d 7573 6963 2c20 6f72 2053 706f  be Music, or Spo
+0000eef0: 7469 6679 2055 524c 2e22 2c0a 2020 2020  tify URL.",.    
+0000ef00: 6465 6661 756c 743d 2266 6c61 6322 2c0a  default="flac",.
+0000ef10: 2020 2020 7368 6f77 5f64 6566 6175 6c74      show_default
+0000ef20: 3d54 7275 652c 0a29 0a40 636c 6963 6b2e  =True,.).@click.
+0000ef30: 6f70 7469 6f6e 280a 2020 2020 222d 6322  option(.    "-c"
+0000ef40: 2c0a 2020 2020 222d 2d63 6c69 7022 2c0a  ,.    "--clip",.
+0000ef50: 2020 2020 6e61 7267 733d 322c 0a20 2020      nargs=2,.   
+0000ef60: 2074 7970 653d 666c 6f61 742c 0a20 2020   type=float,.   
+0000ef70: 2068 656c 703d 2241 6464 2061 2063 6c69   help="Add a cli
+0000ef80: 702e 2049 676e 6f72 6564 2069 6620 6164  p. Ignored if ad
+0000ef90: 6469 6e67 206d 756c 7469 706c 6520 736f  ding multiple so
+0000efa0: 6e67 732e 222c 0a29 0a40 636c 6963 6b2e  ngs.",.).@click.
+0000efb0: 6f70 7469 6f6e 280a 2020 2020 222d 502f  option(.    "-P/
+0000efc0: 2d6e 5022 2c0a 2020 2020 222d 2d70 6c61  -nP",.    "--pla
+0000efd0: 796c 6973 742f 2d2d 6e6f 2d70 6c61 796c  ylist/--no-playl
+0000efe0: 6973 7422 2c0a 2020 2020 2270 6c61 796c  ist",.    "playl
+0000eff0: 6973 745f 222c 0a20 2020 2064 6566 6175  ist_",.    defau
+0000f000: 6c74 3d46 616c 7365 2c0a 2020 2020 6865  lt=False,.    he
+0000f010: 6c70 3d22 4966 2073 6f6e 6720 5552 4c20  lp="If song URL 
+0000f020: 7061 7373 6564 2069 7320 6672 6f6d 2061  passed is from a
+0000f030: 2059 6f75 5475 6265 2070 6c61 796c 6973   YouTube playlis
+0000f040: 742c 2064 6f77 6e6c 6f61 6420 616c 6c20  t, download all 
+0000f050: 7468 6520 736f 6e67 732e 2049 6620 7468  the songs. If th
+0000f060: 6520 5552 4c20 706f 696e 7473 2064 6972  e URL points dir
+0000f070: 6563 746c 7920 746f 2061 2070 6c61 796c  ectly to a playl
+0000f080: 6973 742c 2074 6869 7320 666c 6167 2069  ist, this flag i
+0000f090: 7320 756e 6e63 6573 7361 7279 2e22 2c0a  s unncessary.",.
+0000f0a0: 290a 4063 6c69 636b 2e6f 7074 696f 6e28  ).@click.option(
+0000f0b0: 0a20 2020 2022 2d6d 222c 0a20 2020 2022  .    "-m",.    "
+0000f0c0: 2d2d 6d65 7461 6461 7461 222c 0a20 2020  --metadata",.   
+0000f0d0: 2022 6d65 7461 6461 7461 5f70 6169 7273   "metadata_pairs
+0000f0e0: 222c 0a20 2020 2064 6566 6175 6c74 3d4e  ",.    default=N
+0000f0f0: 6f6e 652c 0a20 2020 2068 656c 703d 2241  one,.    help="A
+0000f100: 6464 206d 6574 6164 6174 6120 746f 2074  dd metadata to t
+0000f110: 6865 2073 6f6e 672e 2049 676e 6f72 6564  he song. Ignored
+0000f120: 2069 6620 6164 6469 6e67 206d 756c 7469   if adding multi
+0000f130: 706c 6520 736f 6e67 732e 2054 6865 2066  ple songs. The f
+0000f140: 6f72 6d61 7420 6973 2027 6b65 7931 3a76  ormat is 'key1:v
+0000f150: 616c 7565 317c 6b65 7932 3a76 616c 7565  alue1|key2:value
+0000f160: 327c 2e2e 2e27 2e22 2c0a 290a 6465 6620  2|...'.",.).def 
+0000f170: 6164 6428 0a20 2020 2070 6174 685f 2c0a  add(.    path_,.
+0000f180: 2020 2020 7461 6773 2c0a 2020 2020 6d6f      tags,.    mo
+0000f190: 7665 5f2c 0a20 2020 206e 616d 652c 0a20  ve_,.    name,. 
+0000f1a0: 2020 2072 6563 7572 7365 2c0a 2020 2020     recurse,.    
+0000f1b0: 796f 7574 7562 652c 0a20 2020 2073 706f  youtube,.    spo
+0000f1c0: 7469 6679 2c0a 2020 2020 666f 726d 6174  tify,.    format
+0000f1d0: 5f2c 0a20 2020 2063 6c69 702c 0a20 2020  _,.    clip,.   
+0000f1e0: 2070 6c61 796c 6973 745f 2c0a 2020 2020   playlist_,.    
+0000f1f0: 6d65 7461 6461 7461 5f70 6169 7273 2c0a  metadata_pairs,.
+0000f200: 293a 0a20 2020 2022 2222 0a20 2020 2041  ):.    """.    A
+0000f210: 6464 2061 206e 6577 2073 6f6e 672e 0a0a  dd a new song...
+0000f220: 2020 2020 4164 6473 2074 6865 2061 7564      Adds the aud
+0000f230: 696f 2066 696c 6520 6c6f 6361 7465 6420  io file located 
+0000f240: 6174 2050 4154 482e 2049 6620 5041 5448  at PATH. If PATH
+0000f250: 2069 7320 6120 666f 6c64 6572 2c20 6164   is a folder, ad
+0000f260: 6473 2061 6c6c 2066 696c 6573 0a20 2020  ds all files.   
+0000f270: 2069 6e20 5041 5448 2028 696e 636c 7564   in PATH (includ
+0000f280: 696e 6720 6669 6c65 7320 696e 2073 7562  ing files in sub
+0000f290: 666f 6c64 6572 7320 6966 2027 2d72 2720  folders if '-r' 
+0000f2a0: 6973 2070 6173 7365 6429 2e20 5468 6520  is passed). The 
+0000f2b0: 6e61 6d65 206f 6620 6561 6368 0a20 2020  name of each.   
+0000f2c0: 2073 6f6e 6720 7769 6c6c 2062 6520 7468   song will be th
+0000f2d0: 6520 6669 6c65 6e61 6d65 2028 756e 6c65  e filename (unle
+0000f2e0: 7373 2027 2d6e 2720 6973 2070 6173 7365  ss '-n' is passe
+0000f2f0: 6429 2e20 4669 6c65 6e61 6d65 7320 616e  d). Filenames an
+0000f300: 6420 7461 6773 2063 616e 6e6f 740a 2020  d tags cannot.  
+0000f310: 2020 636f 6e74 6169 6e20 7468 6520 6368    contain the ch
+0000f320: 6172 6163 7465 7220 277c 272c 2061 6e64  aracter '|', and
+0000f330: 2074 6167 7320 6361 6e6e 6f74 2063 6f6e   tags cannot con
+0000f340: 7461 696e 2027 2c27 2e0a 0a20 2020 2049  tain ','...    I
+0000f350: 6620 7468 6520 272d 5927 206f 7220 272d  f the '-Y' or '-
+0000f360: 2d79 6f75 7475 6265 2720 666c 6167 2069  -youtube' flag i
+0000f370: 7320 7061 7373 6564 2c20 5041 5448 2069  s passed, PATH i
+0000f380: 7320 7472 6561 7465 6420 6173 2061 2059  s treated as a Y
+0000f390: 6f75 5475 6265 206f 720a 2020 2020 596f  ouTube or.    Yo
+0000f3a0: 7554 7562 6520 4d75 7369 6320 5552 4c20  uTube Music URL 
+0000f3b0: 696e 7374 6561 6420 6f66 2061 2066 696c  instead of a fil
+0000f3c0: 6520 7061 7468 2e0a 0a20 2020 2049 6620  e path...    If 
+0000f3d0: 7468 6520 272d 5327 206f 7220 272d 2d73  the '-S' or '--s
+0000f3e0: 706f 7469 6679 2720 666c 6167 2069 7320  potify' flag is 
+0000f3f0: 7061 7373 6564 2c20 5041 5448 2069 7320  passed, PATH is 
+0000f400: 7472 6561 7465 6420 6173 2061 2053 706f  treated as a Spo
+0000f410: 7469 6679 0a20 2020 2074 7261 636b 2055  tify.    track U
+0000f420: 524c 2c20 616c 6275 6d20 5552 4c2c 2070  RL, album URL, p
+0000f430: 6c61 796c 6973 7420 5552 4c2c 2061 7274  laylist URL, art
+0000f440: 6973 7420 5552 4c2c 206f 7220 7365 6172  ist URL, or sear
+0000f450: 6368 2071 7565 7279 2069 6e73 7465 6164  ch query instead
+0000f460: 206f 660a 2020 2020 6120 6669 6c65 2070   of.    a file p
+0000f470: 6174 682e 0a0a 2020 2020 5468 6520 272d  ath...    The '-
+0000f480: 632f 2d2d 636c 6970 2720 6f70 7469 6f6e  c/--clip' option
+0000f490: 2063 616e 2062 6520 7573 6564 2074 6f20   can be used to 
+0000f4a0: 6164 6420 6120 636c 6970 2066 6f72 2074  add a clip for t
+0000f4b0: 6865 2073 6f6e 672e 2049 7420 7461 6b65  he song. It take
+0000f4c0: 7320 7477 6f0a 2020 2020 6172 6775 6d65  s two.    argume
+0000f4d0: 6e74 732c 2062 7574 2075 6e6c 696b 6520  nts, but unlike 
+0000f4e0: 276d 6165 7374 726f 2063 6c69 7027 2c20  'maestro clip', 
+0000f4f0: 796f 7520 6361 6e6e 6f74 2070 6173 7320  you cannot pass 
+0000f500: 6f6e 6c79 2074 6865 2073 7461 7274 2074  only the start t
+0000f510: 696d 650a 2020 2020 616e 6420 6e6f 7420  ime.    and not 
+0000f520: 7468 6520 656e 642e 2054 6f20 6765 7420  the end. To get 
+0000f530: 6172 6f75 6e64 2074 6869 732c 2079 6f75  around this, you
+0000f540: 2063 616e 2070 6173 7320 2d31 2061 7320   can pass -1 as 
+0000f550: 7468 6520 656e 6420 7469 6d65 2c20 652e  the end time, e.
+0000f560: 672e 0a20 2020 2027 6d61 6573 7472 6f20  g..    'maestro 
+0000f570: 6164 6420 2d63 2033 3020 2d31 2068 7474  add -c 30 -1 htt
+0000f580: 7073 3a2f 2f77 7777 2e79 6f75 7475 6265  ps://www.youtube
+0000f590: 2e63 6f6d 2f77 6174 6368 3f76 3d33 5678  .com/watch?v=3Vx
+0000f5a0: 754d 4572 4364 2d45 202d 7927 2e20 4966  uMErCd-E -y'. If
+0000f5b0: 0a20 2020 2061 6464 696e 6720 6d75 6c74  .    adding mult
+0000f5c0: 6970 6c65 2073 6f6e 6773 2c20 7468 6973  iple songs, this
+0000f5d0: 206f 7074 696f 6e20 6361 6e6e 6f74 2062   option cannot b
+0000f5e0: 6520 7573 6564 2e0a 0a20 2020 2054 6865  e used...    The
+0000f5f0: 2027 2d6d 2f2d 2d6d 6574 6164 6174 6127   '-m/--metadata'
+0000f600: 206f 7074 696f 6e20 6361 6e20 6265 2075   option can be u
+0000f610: 7365 6420 746f 2061 6464 206d 6574 6164  sed to add metad
+0000f620: 6174 6120 746f 2074 6865 2073 6f6e 672e  ata to the song.
+0000f630: 2049 7420 7461 6b65 730a 2020 2020 6120   It takes.    a 
+0000f640: 7374 7269 6e67 206f 6620 7468 6520 666f  string of the fo
+0000f650: 726d 6174 2027 6b65 7931 3a76 616c 7565  rmat 'key1:value
+0000f660: 317c 6b65 7932 3a76 616c 7565 327c 2e2e  1|key2:value2|..
+0000f670: 2e27 2e20 4966 2061 6464 696e 6720 6d75  .'. If adding mu
+0000f680: 6c74 6970 6c65 0a20 2020 2073 6f6e 6773  ltiple.    songs
+0000f690: 2c20 7468 6973 206f 7074 696f 6e20 6361  , this option ca
+0000f6a0: 6e6e 6f74 2062 6520 7573 6564 2e0a 0a20  nnot be used... 
+0000f6b0: 2020 2050 6f73 7369 626c 6520 6564 6974     Possible edit
+0000f6c0: 6162 6c65 206d 6574 6164 6174 6120 6b65  able metadata ke
+0000f6d0: 7973 2061 7265 3a20 616c 6275 6d2c 2061  ys are: album, a
+0000f6e0: 6c62 756d 6172 7469 7374 2c20 6172 7469  lbumartist, arti
+0000f6f0: 7374 2c20 6172 7477 6f72 6b2c 0a20 2020  st, artwork,.   
+0000f700: 2063 6f6d 6d65 6e74 2c20 636f 6d70 696c   comment, compil
+0000f710: 6174 696f 6e2c 2063 6f6d 706f 7365 722c  ation, composer,
+0000f720: 2064 6973 636e 756d 6265 722c 2067 656e   discnumber, gen
+0000f730: 7265 2c20 6c79 7269 6373 2c20 746f 7461  re, lyrics, tota
+0000f740: 6c64 6973 6373 2c0a 2020 2020 746f 7461  ldiscs,.    tota
+0000f750: 6c74 7261 636b 732c 2074 7261 636b 6e75  ltracks, tracknu
+0000f760: 6d62 6572 2c20 7472 6163 6b74 6974 6c65  mber, tracktitle
+0000f770: 2c20 7965 6172 2c20 6973 7263 0a0a 2020  , year, isrc..  
+0000f780: 2020 4b65 7973 2061 7265 206e 6f74 2063    Keys are not c
+0000f790: 6173 6520 7365 6e73 6974 6976 6520 616e  ase sensitive an
+0000f7a0: 6420 6361 6e20 636f 6e74 6169 6e20 6172  d can contain ar
+0000f7b0: 6269 7472 6172 7920 7768 6974 6573 7061  bitrary whitespa
+0000f7c0: 6365 2c20 272d 272c 2061 6e64 0a20 2020  ce, '-', and.   
+0000f7d0: 2027 5f27 2063 6861 7261 6374 6572 732e   '_' characters.
+0000f7e0: 2049 6e20 6f74 6865 7220 776f 7264 732c   In other words,
+0000f7f0: 2027 416c 6275 6d20 4172 7469 7374 272c   'Album Artist',
+0000f800: 2027 616c 6275 6d2d 6172 7469 7374 272c   'album-artist',
+0000f810: 2061 6e64 0a20 2020 2027 616c 6275 6d5f   and.    'album_
+0000f820: 6172 7469 7374 2720 6172 6520 616c 6c20  artist' are all 
+0000f830: 7379 6e6f 6e79 6d73 2066 6f72 2027 616c  synonyms for 'al
+0000f840: 6275 6d61 7274 6973 7427 2e20 416c 736f  bumartist'. Also
+0000f850: 2c20 2764 6973 6b27 2069 730a 2020 2020  , 'disk' is.    
+0000f860: 7379 6e6f 6e79 6d6f 7573 2077 6974 6820  synonymous with 
+0000f870: 2764 6973 6327 2e0a 2020 2020 2222 220a  'disc'..    """.
+0000f880: 0a20 2020 2070 6174 6873 203d 204e 6f6e  .    paths = Non
+0000f890: 650a 2020 2020 6966 206e 6f74 2028 796f  e.    if not (yo
+0000f8a0: 7574 7562 6520 6f72 2073 706f 7469 6679  utube or spotify
+0000f8b0: 2920 616e 6420 6e6f 7420 6f73 2e70 6174  ) and not os.pat
+0000f8c0: 682e 6578 6973 7473 2870 6174 685f 293a  h.exists(path_):
+0000f8d0: 0a20 2020 2020 2020 2063 6c69 636b 2e73  .        click.s
+0000f8e0: 6563 686f 280a 2020 2020 2020 2020 2020  echo(.          
+0000f8f0: 2020 6622 5468 6520 7061 7468 2027 7b70    f"The path '{p
+0000f900: 6174 685f 7d27 2064 6f65 7320 6e6f 7420  ath_}' does not 
+0000f910: 6578 6973 742e 2054 6f20 646f 776e 6c6f  exist. To downlo
+0000f920: 6164 2066 726f 6d20 6120 596f 7554 7562  ad from a YouTub
+0000f930: 6520 6f72 2059 6f75 5475 6265 204d 7573  e or YouTube Mus
+0000f940: 6963 2055 526c 2c20 7061 7373 2074 6865  ic URl, pass the
+0000f950: 2027 2d59 2f2d 2d79 6f75 7475 6265 2720   '-Y/--youtube' 
+0000f960: 666c 6167 2e20 546f 2064 6f77 6e6c 6f61  flag. To downloa
+0000f970: 6420 6672 6f6d 2061 2053 706f 7469 6679  d from a Spotify
+0000f980: 2055 526c 2c20 7061 7373 2074 6865 2027   URl, pass the '
+0000f990: 2d53 2f2d 2d73 706f 7469 6679 2720 666c  -S/--spotify' fl
+0000f9a0: 6167 2e22 2c0a 2020 2020 2020 2020 2020  ag.",.          
+0000f9b0: 2020 6667 3d22 7265 6422 2c0a 2020 2020    fg="red",.    
+0000f9c0: 2020 2020 290a 2020 2020 2020 2020 7265      ).        re
+0000f9d0: 7475 726e 0a0a 2020 2020 6966 2079 6f75  turn..    if you
+0000f9e0: 7475 6265 206f 7220 7370 6f74 6966 793a  tube or spotify:
+0000f9f0: 0a20 2020 2020 2020 2069 6620 796f 7574  .        if yout
+0000fa00: 7562 6520 616e 6420 7370 6f74 6966 793a  ube and spotify:
+0000fa10: 0a20 2020 2020 2020 2020 2020 2063 6c69  .            cli
+0000fa20: 636b 2e73 6563 686f 280a 2020 2020 2020  ck.secho(.      
+0000fa30: 2020 2020 2020 2020 2020 2243 616e 6e6f            "Canno
+0000fa40: 7420 7061 7373 2062 6f74 6820 272d 792f  t pass both '-y/
+0000fa50: 2d2d 796f 7574 7562 6527 2061 6e64 2027  --youtube' and '
+0000fa60: 2d73 2f2d 2d73 706f 7469 6679 2720 666c  -s/--spotify' fl
+0000fa70: 6167 732e 222c 0a20 2020 2020 2020 2020  ags.",.         
+0000fa80: 2020 2020 2020 2066 673d 2272 6564 222c         fg="red",
+0000fa90: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+0000faa0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000fab0: 6e0a 0a20 2020 2020 2020 2069 6620 796f  n..        if yo
+0000fac0: 7574 7562 653a 0a20 2020 2020 2020 2020  utube:.         
+0000fad0: 2020 2069 6620 666f 726d 6174 5f20 3d3d     if format_ ==
+0000fae0: 2022 6f67 6722 3a0a 2020 2020 2020 2020   "ogg":.        
+0000faf0: 2020 2020 2020 2020 636c 6963 6b2e 7365          click.se
+0000fb00: 6368 6f28 0a20 2020 2020 2020 2020 2020  cho(.           
+0000fb10: 2020 2020 2020 2020 2022 4361 6e6e 6f74           "Cannot
+0000fb20: 2064 6f77 6e6c 6f61 6420 736f 6e67 7320   download songs 
+0000fb30: 6672 6f6d 2059 6f75 5475 6265 2061 7320  from YouTube as 
+0000fb40: 272e 6f67 6727 2e20 506c 6561 7365 2063  '.ogg'. Please c
+0000fb50: 686f 6f73 6520 6120 6469 6666 6572 656e  hoose a differen
+0000fb60: 7420 666f 726d 6174 2e22 2c0a 2020 2020  t format.",.    
+0000fb70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fb80: 6667 3d22 7265 6422 2c0a 2020 2020 2020  fg="red",.      
+0000fb90: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0000fba0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000fbb0: 726e 0a20 2020 2020 2020 2020 2020 2073  rn.            s
+0000fbc0: 7562 7072 6f63 6573 732e 7275 6e28 0a20  ubprocess.run(. 
+0000fbd0: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+0000fbe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000fbf0: 2020 2020 2022 7974 2d64 6c70 222c 0a20       "yt-dlp",. 
+0000fc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fc10: 2020 2070 6174 685f 2c0a 2020 2020 2020     path_,.      
+0000fc20: 2020 2020 2020 2020 2020 2020 2020 222d                "-
+0000fc30: 7822 2c20 2023 2065 7874 7261 6374 2061  x",  # extract a
+0000fc40: 7564 696f 2028 6e65 6365 7373 6172 792c  udio (necessary,
+0000fc50: 206e 6565 6473 2066 666d 7065 6729 0a20   needs ffmpeg). 
+0000fc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fc70: 2020 2022 2d2d 6175 6469 6f2d 666f 726d     "--audio-form
+0000fc80: 6174 222c 0a20 2020 2020 2020 2020 2020  at",.           
+0000fc90: 2020 2020 2020 2020 2066 6f72 6d61 745f           format_
+0000fca0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000fcb0: 2020 2020 2020 222d 2d6e 6f2d 706c 6179        "--no-play
+0000fcc0: 6c69 7374 2220 6966 206e 6f74 2070 6c61  list" if not pla
+0000fcd0: 796c 6973 745f 2065 6c73 6520 2222 2c0a  ylist_ else "",.
+0000fce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fcf0: 2020 2020 222d 2d65 6d62 6564 2d6d 6574      "--embed-met
+0000fd00: 6164 6174 6122 2c0a 2020 2020 2020 2020  adata",.        
+0000fd10: 2020 2020 2020 2020 2020 2020 222d 6f22              "-o"
+0000fd20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000fd30: 2020 2020 2020 6f73 2e70 6174 682e 6a6f        os.path.jo
+0000fd40: 696e 284d 4145 5354 524f 5f44 4952 2c20  in(MAESTRO_DIR, 
+0000fd50: 2225 2874 6974 6c65 2973 2e25 2865 7874  "%(title)s.%(ext
+0000fd60: 2973 2229 2c0a 2020 2020 2020 2020 2020  )s"),.          
+0000fd70: 2020 2020 2020 5d2c 0a20 2020 2020 2020        ],.       
+0000fd80: 2020 2020 2020 2020 2063 6865 636b 3d54           check=T
+0000fd90: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
+0000fda0: 2029 0a20 2020 2020 2020 2065 6c73 653a   ).        else:
+0000fdb0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000fdc0: 666f 726d 6174 5f20 3d3d 2022 7761 7622  format_ == "wav"
+0000fdd0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000fde0: 2020 636c 6963 6b2e 7365 6368 6f28 0a20    click.secho(. 
+0000fdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fe00: 2020 2022 4361 6e6e 6f74 2064 6f77 6e6c     "Cannot downl
+0000fe10: 6f61 6420 736f 6e67 7320 6672 6f6d 2053  oad songs from S
+0000fe20: 706f 7469 6679 2061 7320 272e 7761 7627  potify as '.wav'
+0000fe30: 2e20 506c 6561 7365 2063 686f 6f73 6520  . Please choose 
+0000fe40: 6120 6469 6666 6572 656e 7420 666f 726d  a different form
+0000fe50: 6174 2e22 2c0a 2020 2020 2020 2020 2020  at.",.          
+0000fe60: 2020 2020 2020 2020 2020 6667 3d22 7265            fg="re
+0000fe70: 6422 2c0a 2020 2020 2020 2020 2020 2020  d",.            
+0000fe80: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0000fe90: 2020 2020 2020 7265 7475 726e 0a0a 2020        return..  
+0000fea0: 2020 2020 2020 2020 2020 6377 6420 3d20            cwd = 
+0000feb0: 6f73 2e67 6574 6377 6428 290a 2020 2020  os.getcwd().    
+0000fec0: 2020 2020 2020 2020 6f73 2e63 6864 6972          os.chdir
+0000fed0: 284d 4145 5354 524f 5f44 4952 290a 2020  (MAESTRO_DIR).  
+0000fee0: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
 0000fef0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000ff00: 616e 6974 697a 6564 5f70 6174 6820 3d20  anitized_path = 
-0000ff10: 7261 775f 7061 7468 2e72 6570 6c61 6365  raw_path.replace
-0000ff20: 2822 7c22 2c20 222d 2229 0a0a 2020 2020  ("|", "-")..    
-0000ff30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff40: 6f73 2e72 656e 616d 6528 7261 775f 7061  os.rename(raw_pa
-0000ff50: 7468 2c20 7361 6e69 7469 7a65 645f 7061  th, sanitized_pa
-0000ff60: 7468 290a 0a20 2020 2020 2020 2020 2020  th)..           
-0000ff70: 2020 2020 2020 2020 2070 6174 6873 2e61           paths.a
-0000ff80: 7070 656e 6428 7361 6e69 7469 7a65 645f  ppend(sanitized_
-0000ff90: 7061 7468 290a 2020 2020 2020 2020 2020  path).          
-0000ffa0: 2020 6966 2066 6e61 6d65 2e65 6e64 7377    if fname.endsw
-0000ffb0: 6974 6828 222e 7061 7274 2229 3a20 2023  ith(".part"):  #
-0000ffc0: 2064 656c 6574 6520 696e 636f 6d70 6c65   delete incomple
-0000ffd0: 7465 2064 6f77 6e6c 6f61 6473 0a20 2020  te downloads.   
-0000ffe0: 2020 2020 2020 2020 2020 2020 206f 732e               os.
-0000fff0: 7265 6d6f 7665 286f 732e 7061 7468 2e6a  remove(os.path.j
-00010000: 6f69 6e28 4d41 4553 5452 4f5f 4449 522c  oin(MAESTRO_DIR,
-00010010: 2066 6e61 6d65 2929 0a0a 2020 2020 2020   fname))..      
-00010020: 2020 6d6f 7665 5f20 3d20 5472 7565 0a0a    move_ = True..
-00010030: 2020 2020 6966 2070 6174 6873 2069 7320      if paths is 
-00010040: 4e6f 6e65 3a0a 2020 2020 2020 2020 6966  None:.        if
-00010050: 206f 732e 7061 7468 2e69 7364 6972 2870   os.path.isdir(p
-00010060: 6174 685f 293a 0a20 2020 2020 2020 2020  ath_):.         
-00010070: 2020 2070 6174 6873 203d 205b 5d0a 2020     paths = [].  
-00010080: 2020 2020 2020 2020 2020 6966 2072 6563            if rec
-00010090: 7572 7365 3a0a 2020 2020 2020 2020 2020  urse:.          
-000100a0: 2020 2020 2020 666f 7220 6469 7270 6174        for dirpat
-000100b0: 682c 205f 2c20 666e 616d 6573 2069 6e20  h, _, fnames in 
-000100c0: 6f73 2e77 616c 6b28 7061 7468 5f29 3a0a  os.walk(path_):.
-000100d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000100e0: 2020 2020 666f 7220 666e 616d 6520 696e      for fname in
-000100f0: 2066 6e61 6d65 733a 0a20 2020 2020 2020   fnames:.       
-00010100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010110: 2069 6620 6f73 2e70 6174 682e 7370 6c69   if os.path.spli
-00010120: 7465 7874 2866 6e61 6d65 295b 315d 2069  text(fname)[1] i
-00010130: 6e20 4558 5453 3a0a 2020 2020 2020 2020  n EXTS:.        
-00010140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010150: 2020 2020 7061 7468 732e 6170 7065 6e64      paths.append
-00010160: 286f 732e 7061 7468 2e6a 6f69 6e28 6469  (os.path.join(di
-00010170: 7270 6174 682c 2066 6e61 6d65 2929 0a20  rpath, fname)). 
-00010180: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00010190: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000101a0: 2066 6f72 2066 6e61 6d65 2069 6e20 6f73   for fname in os
-000101b0: 2e6c 6973 7464 6972 2870 6174 685f 293a  .listdir(path_):
-000101c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000101d0: 2020 2020 2069 6620 6f73 2e70 6174 682e       if os.path.
-000101e0: 7370 6c69 7465 7874 2866 6e61 6d65 295b  splitext(fname)[
-000101f0: 315d 2069 6e20 4558 5453 3a0a 2020 2020  1] in EXTS:.    
-00010200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010210: 2020 2020 6675 6c6c 5f70 6174 6820 3d20      full_path = 
-00010220: 6f73 2e70 6174 682e 6a6f 696e 2870 6174  os.path.join(pat
-00010230: 685f 2c20 666e 616d 6529 0a20 2020 2020  h_, fname).     
-00010240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010250: 2020 2069 6620 6f73 2e70 6174 682e 6973     if os.path.is
-00010260: 6669 6c65 2866 756c 6c5f 7061 7468 293a  file(full_path):
-00010270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010280: 2020 2020 2020 2020 2020 2020 2070 6174               pat
-00010290: 6873 2e61 7070 656e 6428 6675 6c6c 5f70  hs.append(full_p
-000102a0: 6174 6829 0a20 2020 2020 2020 2020 2020  ath).           
-000102b0: 2069 6620 6c65 6e28 7061 7468 7329 203d   if len(paths) =
-000102c0: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
-000102d0: 2020 2020 2063 6c69 636b 2e73 6563 686f       click.secho
-000102e0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000102f0: 2020 2020 2020 6622 4e6f 2073 6f6e 6773        f"No songs
-00010300: 2066 6f75 6e64 2069 6e20 277b 7061 7468   found in '{path
-00010310: 5f7d 272e 222c 0a20 2020 2020 2020 2020  _}'.",.         
-00010320: 2020 2020 2020 2020 2020 2066 673d 2272             fg="r
-00010330: 6564 222c 0a20 2020 2020 2020 2020 2020  ed",.           
-00010340: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00010350: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
-00010360: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00010370: 2020 2020 2020 2020 7061 7468 7320 3d20          paths = 
-00010380: 5b70 6174 685f 5d0a 0a20 2020 2069 6620  [path_]..    if 
-00010390: 6c65 6e28 7061 7468 7329 203e 2031 3a0a  len(paths) > 1:.
-000103a0: 2020 2020 2020 2020 6966 2063 6c69 7020          if clip 
-000103b0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000103c0: 2020 2020 2020 2020 2063 6c69 636b 2e73           click.s
-000103d0: 6563 686f 280a 2020 2020 2020 2020 2020  echo(.          
-000103e0: 2020 2020 2020 2243 616e 6e6f 7420 7061        "Cannot pa
-000103f0: 7373 2027 2d63 2f2d 2d63 6c69 7027 206f  ss '-c/--clip' o
-00010400: 7074 696f 6e20 7768 656e 2061 6464 696e  ption when addin
-00010410: 6720 6d75 6c74 6970 6c65 2073 6f6e 6773  g multiple songs
-00010420: 2e22 2c0a 2020 2020 2020 2020 2020 2020  .",.            
-00010430: 2020 2020 6667 3d22 7265 6422 2c0a 2020      fg="red",.  
-00010440: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00010450: 2020 2020 2020 2020 7265 7475 726e 0a0a          return..
-00010460: 2020 2020 2020 2020 6966 206e 616d 6520          if name 
-00010470: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00010480: 2020 2020 2020 2020 2063 6c69 636b 2e73           click.s
-00010490: 6563 686f 280a 2020 2020 2020 2020 2020  echo(.          
-000104a0: 2020 2020 2020 2243 616e 6e6f 7420 7061        "Cannot pa
-000104b0: 7373 2027 2d6e 2f2d 2d6e 616d 6527 206f  ss '-n/--name' o
-000104c0: 7074 696f 6e20 7768 656e 2061 6464 696e  ption when addin
-000104d0: 6720 6d75 6c74 6970 6c65 2073 6f6e 6773  g multiple songs
-000104e0: 2e22 2c0a 2020 2020 2020 2020 2020 2020  .",.            
-000104f0: 2020 2020 6667 3d22 7265 6422 2c0a 2020      fg="red",.  
-00010500: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00010510: 2020 2020 2020 2020 7265 7475 726e 0a0a          return..
-00010520: 2020 2020 6966 206c 656e 2870 6174 6873      if len(paths
-00010530: 2920 3d3d 2031 2061 6e64 206e 616d 6520  ) == 1 and name 
-00010540: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00010550: 2020 2020 206e 6577 5f70 6174 6820 3d20       new_path = 
-00010560: 6f73 2e70 6174 682e 6a6f 696e 280a 2020  os.path.join(.  
-00010570: 2020 2020 2020 2020 2020 4d41 4553 5452            MAESTR
-00010580: 4f5f 4449 522c 206e 616d 6520 2b20 6f73  O_DIR, name + os
-00010590: 2e70 6174 682e 7370 6c69 7465 7874 2870  .path.splitext(p
-000105a0: 6174 6873 5b30 5d29 5b31 5d0a 2020 2020  aths[0])[1].    
-000105b0: 2020 2020 290a 2020 2020 2020 2020 2320      ).        # 
-000105c0: 6d6f 7665 2f63 6f70 7920 746f 204d 4145  move/copy to MAE
-000105d0: 5354 524f 5f44 4952 2028 6176 6f69 6420  STRO_DIR (avoid 
-000105e0: 6e61 6d65 2063 6f6e 666c 6963 7473 290a  name conflicts).
-000105f0: 2020 2020 2020 2020 6966 206d 6f76 655f          if move_
-00010600: 3a0a 2020 2020 2020 2020 2020 2020 6d6f  :.            mo
-00010610: 7665 2870 6174 6873 5b30 5d2c 206e 6577  ve(paths[0], new
-00010620: 5f70 6174 6829 0a20 2020 2020 2020 2065  _path).        e
-00010630: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00010640: 2063 6f70 7928 7061 7468 735b 305d 2c20   copy(paths[0], 
-00010650: 6e65 775f 7061 7468 290a 2020 2020 2020  new_path).      
-00010660: 2020 7061 7468 7320 3d20 5b6e 6577 5f70    paths = [new_p
-00010670: 6174 685d 0a20 2020 2020 2020 206d 6f76  ath].        mov
-00010680: 655f 203d 2054 7275 6520 2023 2061 6c77  e_ = True  # alw
-00010690: 6179 7320 6d6f 7665 2028 6672 6f6d 2074  ays move (from t
-000106a0: 656d 7020 6c6f 6320 696e 204d 4145 5354  emp loc in MAEST
-000106b0: 524f 5f44 4952 2920 6966 2072 656e 616d  RO_DIR) if renam
-000106c0: 696e 670a 0a20 2020 2069 6620 636c 6970  ing..    if clip
-000106d0: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
-000106e0: 206c 656e 2870 6174 6873 2920 3d3d 2031   len(paths) == 1
-000106f0: 3a0a 2020 2020 2020 2020 736f 6e67 5f64  :.        song_d
-00010700: 7572 6174 696f 6e20 3d20 6d75 7369 635f  uration = music_
-00010710: 7461 672e 6c6f 6164 5f66 696c 6528 7061  tag.load_file(pa
-00010720: 7468 735b 305d 295b 2223 6c65 6e67 7468  ths[0])["#length
-00010730: 225d 2e76 616c 7565 0a0a 2020 2020 2020  "].value..      
-00010740: 2020 7374 6172 742c 2065 6e64 203d 2063    start, end = c
-00010750: 6c69 700a 2020 2020 2020 2020 6966 2073  lip.        if s
-00010760: 7461 7274 203c 2030 3a0a 2020 2020 2020  tart < 0:.      
-00010770: 2020 2020 2020 636c 6963 6b2e 7365 6368        click.sech
-00010780: 6f28 2243 6c69 7020 7374 6172 7420 7469  o("Clip start ti
-00010790: 6d65 2063 616e 6e6f 7420 6265 206e 6567  me cannot be neg
-000107a0: 6174 6976 652e 222c 2066 673d 2272 6564  ative.", fg="red
-000107b0: 2229 0a20 2020 2020 2020 2020 2020 2072  ").            r
-000107c0: 6574 7572 6e0a 2020 2020 2020 2020 6966  eturn.        if
-000107d0: 2073 7461 7274 203e 2073 6f6e 675f 6475   start > song_du
-000107e0: 7261 7469 6f6e 3a0a 2020 2020 2020 2020  ration:.        
-000107f0: 2020 2020 636c 6963 6b2e 7365 6368 6f28      click.secho(
-00010800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010810: 2022 436c 6970 2073 7461 7274 2074 696d   "Clip start tim
-00010820: 6520 6361 6e6e 6f74 2062 6520 6772 6561  e cannot be grea
-00010830: 7465 7220 7468 616e 2074 6865 2073 6f6e  ter than the son
-00010840: 6720 6475 7261 7469 6f6e 2e22 2c0a 2020  g duration.",.  
-00010850: 2020 2020 2020 2020 2020 2020 2020 6667                fg
-00010860: 3d22 7265 6422 2c0a 2020 2020 2020 2020  ="red",.        
-00010870: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00010880: 2020 7265 7475 726e 0a0a 2020 2020 2020    return..      
-00010890: 2020 6966 2065 6e64 203d 3d20 2d31 3a0a    if end == -1:.
-000108a0: 2020 2020 2020 2020 2020 2020 656e 6420              end 
-000108b0: 3d20 736f 6e67 5f64 7572 6174 696f 6e0a  = song_duration.
-000108c0: 2020 2020 2020 2020 656c 6966 2065 6e64          elif end
-000108d0: 203c 2073 7461 7274 3a0a 2020 2020 2020   < start:.      
-000108e0: 2020 2020 2020 636c 6963 6b2e 7365 6368        click.sech
-000108f0: 6f28 0a20 2020 2020 2020 2020 2020 2020  o(.             
-00010900: 2020 2022 436c 6970 2065 6e64 2074 696d     "Clip end tim
-00010910: 6520 6361 6e6e 6f74 2062 6520 6c65 7373  e cannot be less
-00010920: 2074 6861 6e20 7468 6520 636c 6970 2073   than the clip s
-00010930: 7461 7274 2074 696d 652e 222c 0a20 2020  tart time.",.   
-00010940: 2020 2020 2020 2020 2020 2020 2066 673d               fg=
-00010950: 2272 6564 222c 0a20 2020 2020 2020 2020  "red",.         
-00010960: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00010970: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
-00010980: 656c 6966 2065 6e64 203e 2073 6f6e 675f  elif end > song_
-00010990: 6475 7261 7469 6f6e 3a0a 2020 2020 2020  duration:.      
-000109a0: 2020 2020 2020 636c 6963 6b2e 7365 6368        click.sech
-000109b0: 6f28 0a20 2020 2020 2020 2020 2020 2020  o(.             
-000109c0: 2020 2022 436c 6970 2065 6e64 2074 696d     "Clip end tim
-000109d0: 6520 6361 6e6e 6f74 2062 6520 6772 6561  e cannot be grea
-000109e0: 7465 7220 7468 616e 2074 6865 2073 6f6e  ter than the son
-000109f0: 6720 6475 7261 7469 6f6e 2e22 2c0a 2020  g duration.",.  
-00010a00: 2020 2020 2020 2020 2020 2020 2020 6667                fg
-00010a10: 3d22 7265 6422 2c0a 2020 2020 2020 2020  ="red",.        
-00010a20: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00010a30: 2020 7265 7475 726e 0a20 2020 2065 6c73    return.    els
-00010a40: 653a 0a20 2020 2020 2020 2073 7461 7274  e:.        start
-00010a50: 203d 2065 6e64 203d 204e 6f6e 650a 0a20   = end = None.. 
-00010a60: 2020 2069 6620 6d65 7461 6461 7461 5f70     if metadata_p
-00010a70: 6169 7273 2069 7320 6e6f 7420 4e6f 6e65  airs is not None
-00010a80: 2061 6e64 206c 656e 2870 6174 6873 2920   and len(paths) 
-00010a90: 3d3d 2031 3a0a 2020 2020 2020 2020 2320  == 1:.        # 
-00010aa0: 636f 6e76 6572 7420 6672 6f6d 2022 6b65  convert from "ke
-00010ab0: 793a 7661 6c75 652c 6b65 793a 7661 6c75  y:value,key:valu
-00010ac0: 6522 2074 6f20 5b28 226b 6579 222c 2022  e" to [("key", "
-00010ad0: 7661 6c75 6522 295d 0a20 2020 2020 2020  value")].       
-00010ae0: 206d 6574 6164 6174 615f 7061 6972 7320   metadata_pairs 
-00010af0: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
-00010b00: 7475 706c 6528 7061 6972 2e73 7472 6970  tuple(pair.strip
-00010b10: 2829 2e73 706c 6974 2822 3a22 2929 2066  ().split(":")) f
-00010b20: 6f72 2070 6169 7220 696e 206d 6574 6164  or pair in metad
-00010b30: 6174 615f 7061 6972 732e 7370 6c69 7428  ata_pairs.split(
-00010b40: 227c 2229 0a20 2020 2020 2020 205d 0a20  "|").        ]. 
-00010b50: 2020 2020 2020 2073 6f6e 675f 6461 7461         song_data
-00010b60: 203d 206d 7573 6963 5f74 6167 2e6c 6f61   = music_tag.loa
-00010b70: 645f 6669 6c65 2870 6174 6873 5b30 5d29  d_file(paths[0])
-00010b80: 0a20 2020 2020 2020 2066 6f72 206b 6579  .        for key
-00010b90: 2c20 7661 6c75 6520 696e 206d 6574 6164  , value in metad
-00010ba0: 6174 615f 7061 6972 733a 0a20 2020 2020  ata_pairs:.     
-00010bb0: 2020 2020 2020 2069 6620 6b65 7920 6e6f         if key no
-00010bc0: 7420 696e 204d 4554 4144 4154 415f 4b45  t in METADATA_KE
-00010bd0: 5953 206f 7220 6b65 792e 7374 6172 7473  YS or key.starts
-00010be0: 7769 7468 2822 2322 293a 0a20 2020 2020  with("#"):.     
-00010bf0: 2020 2020 2020 2020 2020 2063 6c69 636b             click
-00010c00: 2e73 6563 686f 280a 2020 2020 2020 2020  .secho(.        
-00010c10: 2020 2020 2020 2020 2020 2020 6622 277b              f"'{
-00010c20: 6b65 797d 2720 6973 206e 6f74 2061 2076  key}' is not a v
-00010c30: 616c 6964 2065 6469 7461 626c 6520 6d65  alid editable me
-00010c40: 7461 6461 7461 206b 6579 2e22 2c20 6667  tadata key.", fg
-00010c50: 3d22 7265 6422 0a20 2020 2020 2020 2020  ="red".         
-00010c60: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00010c70: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-00010c80: 650a 2020 2020 2020 2020 2020 2020 736f  e.            so
-00010c90: 6e67 5f64 6174 615b 6b65 795d 203d 2076  ng_data[key] = v
-00010ca0: 616c 7565 0a20 2020 2020 2020 2073 6f6e  alue.        son
-00010cb0: 675f 6461 7461 2e73 6176 6528 290a 0a20  g_data.save().. 
-00010cc0: 2020 2066 6f72 2070 6174 6820 696e 2070     for path in p
-00010cd0: 6174 6873 3a0a 2020 2020 2020 2020 6578  aths:.        ex
-00010ce0: 7420 3d20 6f73 2e70 6174 682e 7370 6c69  t = os.path.spli
-00010cf0: 7465 7874 2870 6174 6829 5b31 5d0a 2020  text(path)[1].  
-00010d00: 2020 2020 2020 6966 206e 6f74 206f 732e        if not os.
-00010d10: 7061 7468 2e69 7364 6972 2870 6174 6829  path.isdir(path)
-00010d20: 2061 6e64 2065 7874 206e 6f74 2069 6e20   and ext not in 
-00010d30: 4558 5453 3a0a 2020 2020 2020 2020 2020  EXTS:.          
-00010d40: 2020 636c 6963 6b2e 7365 6368 6f28 6622    click.secho(f"
-00010d50: 277b 6578 747d 2720 6973 206e 6f74 2073  '{ext}' is not s
-00010d60: 7570 706f 7274 6564 2e22 2c20 6667 3d22  upported.", fg="
-00010d70: 7265 6422 290a 2020 2020 2020 2020 2020  red").          
-00010d80: 2020 7265 7475 726e 0a0a 2020 2020 2020    return..      
-00010d90: 2020 666f 7220 7461 6720 696e 2074 6167    for tag in tag
-00010da0: 733a 0a20 2020 2020 2020 2020 2020 2069  s:.            i
-00010db0: 6620 222c 2220 696e 2074 6167 206f 7220  f "," in tag or 
-00010dc0: 227c 2220 696e 2074 6167 3a0a 2020 2020  "|" in tag:.    
-00010dd0: 2020 2020 2020 2020 2020 2020 636c 6963              clic
-00010de0: 6b2e 7365 6368 6f28 2254 6167 7320 6361  k.secho("Tags ca
-00010df0: 6e6e 6f74 2063 6f6e 7461 696e 2027 2c27  nnot contain ','
-00010e00: 206f 7220 277c 272e 222c 2066 673d 2272   or '|'.", fg="r
-00010e10: 6564 2229 0a20 2020 2020 2020 2020 2020  ed").           
-00010e20: 2020 2020 2072 6574 7572 6e0a 0a20 2020       return..   
-00010e30: 2020 2020 2077 6974 6820 6f70 656e 2853       with open(S
-00010e40: 4f4e 4753 5f49 4e46 4f5f 5041 5448 2c20  ONGS_INFO_PATH, 
-00010e50: 2261 2b22 2c20 656e 636f 6469 6e67 3d22  "a+", encoding="
-00010e60: 7574 662d 3822 2920 6173 2073 6f6e 6773  utf-8") as songs
-00010e70: 5f66 696c 653a 0a20 2020 2020 2020 2020  _file:.         
-00010e80: 2020 2073 6f6e 6773 5f66 696c 652e 7365     songs_file.se
-00010e90: 656b 2830 2920 2023 2073 7461 7274 2072  ek(0)  # start r
-00010ea0: 6561 6469 6e67 2066 726f 6d20 6265 6769  eading from begi
-00010eb0: 6e6e 696e 670a 0a20 2020 2020 2020 2020  nning..         
-00010ec0: 2020 206c 696e 6573 203d 2073 6f6e 6773     lines = songs
-00010ed0: 5f66 696c 652e 7265 6164 6c69 6e65 7328  _file.readlines(
-00010ee0: 290a 0a20 2020 2020 2020 2020 2020 2073  )..            s
-00010ef0: 6f6e 675f 6964 203d 2031 0a20 2020 2020  ong_id = 1.     
-00010f00: 2020 2020 2020 2066 6f72 206c 696e 6520         for line 
-00010f10: 696e 206c 696e 6573 3a0a 2020 2020 2020  in lines:.      
-00010f20: 2020 2020 2020 2020 2020 736f 6e67 5f69            song_i
-00010f30: 6420 3d20 6d61 7828 736f 6e67 5f69 642c  d = max(song_id,
-00010f40: 2069 6e74 286c 696e 652e 7370 6c69 7428   int(line.split(
-00010f50: 227c 2229 5b30 5d29 202b 2031 290a 0a20  "|")[0]) + 1).. 
-00010f60: 2020 2020 2020 2020 2020 2070 7265 7065             prepe
-00010f70: 6e64 5f6e 6577 6c69 6e65 203d 206c 696e  nd_newline = lin
-00010f80: 6573 2061 6e64 206c 696e 6573 5b2d 315d  es and lines[-1]
-00010f90: 5b2d 315d 2021 3d20 225c 6e22 0a0a 2020  [-1] != "\n"..  
-00010fa0: 2020 2020 2020 2020 2020 6164 645f 736f            add_so
-00010fb0: 6e67 280a 2020 2020 2020 2020 2020 2020  ng(.            
-00010fc0: 2020 2020 7061 7468 2c0a 2020 2020 2020      path,.      
-00010fd0: 2020 2020 2020 2020 2020 7461 6773 2c0a            tags,.
-00010fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ff0: 6d6f 7665 5f2c 0a20 2020 2020 2020 2020  move_,.         
-00011000: 2020 2020 2020 2073 6f6e 6773 5f66 696c         songs_fil
-00011010: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00011020: 2020 206c 696e 6573 2c0a 2020 2020 2020     lines,.      
-00011030: 2020 2020 2020 2020 2020 736f 6e67 5f69            song_i
-00011040: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
-00011050: 2020 2070 7265 7065 6e64 5f6e 6577 6c69     prepend_newli
-00011060: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-00011070: 2020 2020 7374 6172 742c 0a20 2020 2020      start,.     
-00011080: 2020 2020 2020 2020 2020 2065 6e64 2c0a             end,.
-00011090: 2020 2020 2020 2020 2020 2020 290a 0a0a              )...
-000110a0: 4063 6c69 2e63 6f6d 6d61 6e64 2829 0a40  @cli.command().@
-000110b0: 636c 6963 6b2e 6172 6775 6d65 6e74 2822  click.argument("
-000110c0: 4152 4753 222c 2072 6571 7569 7265 643d  ARGS", required=
-000110d0: 5472 7565 2c20 6e61 7267 733d 2d31 290a  True, nargs=-1).
-000110e0: 4063 6c69 636b 2e6f 7074 696f 6e28 0a20  @click.option(. 
-000110f0: 2020 2022 2d46 2f2d 6e46 222c 2022 2d2d     "-F/-nF", "--
-00011100: 666f 7263 652f 2d2d 6e6f 2d66 6f72 6365  force/--no-force
-00011110: 222c 2064 6566 6175 6c74 3d46 616c 7365  ", default=False
-00011120: 2c20 6865 6c70 3d22 466f 7263 6520 6465  , help="Force de
-00011130: 6c65 7469 6f6e 2e22 0a29 0a40 636c 6963  letion.".).@clic
-00011140: 6b2e 6f70 7469 6f6e 280a 2020 2020 222d  k.option(.    "-
-00011150: 542f 2d6e 5422 2c0a 2020 2020 222d 2d74  T/-nT",.    "--t
-00011160: 6167 2f2d 2d6e 6f2d 7461 6722 2c0a 2020  ag/--no-tag",.  
-00011170: 2020 6465 6661 756c 743d 4661 6c73 652c    default=False,
-00011180: 0a20 2020 2068 656c 703d 2249 6620 7061  .    help="If pa
-00011190: 7373 6564 2c20 7472 6561 7420 616c 6c20  ssed, treat all 
-000111a0: 6172 6775 6d65 6e74 7320 6173 2074 6167  arguments as tag
-000111b0: 732c 2064 656c 6574 696e 6720 6576 6572  s, deleting ever
-000111c0: 7920 6f63 7572 7265 6e63 6520 6f66 2065  y ocurrence of e
-000111d0: 6163 6820 7461 672e 222c 0a29 0a64 6566  ach tag.",.).def
-000111e0: 2072 656d 6f76 6528 6172 6773 2c20 666f   remove(args, fo
-000111f0: 7263 652c 2074 6167 293a 0a20 2020 2022  rce, tag):.    "
-00011200: 2222 5265 6d6f 7665 2065 6974 6865 7220  ""Remove either 
-00011210: 7461 6728 7329 206f 7220 736f 6e67 2873  tag(s) or song(s
-00011220: 2920 7061 7373 6564 2061 7320 4944 2873  ) passed as ID(s
-00011230: 292e 2222 220a 2020 2020 6966 206e 6f74  ).""".    if not
-00011240: 2074 6167 3a0a 2020 2020 2020 2020 7472   tag:.        tr
-00011250: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
-00011260: 6f6e 675f 6964 7320 3d20 7b69 6e74 2873  ong_ids = {int(s
-00011270: 6f6e 675f 6964 2920 666f 7220 736f 6e67  ong_id) for song
-00011280: 5f69 6420 696e 2061 7267 737d 0a20 2020  _id in args}.   
-00011290: 2020 2020 2020 2020 2072 656d 6169 6e69           remaini
-000112a0: 6e67 5f73 6f6e 675f 6964 7320 3d20 7b6e  ng_song_ids = {n
-000112b0: 2066 6f72 206e 2069 6e20 736f 6e67 5f69   for n in song_i
-000112c0: 6473 7d0a 2020 2020 2020 2020 6578 6365  ds}.        exce
-000112d0: 7074 2056 616c 7565 4572 726f 723a 0a20  pt ValueError:. 
-000112e0: 2020 2020 2020 2020 2020 2063 6c69 636b             click
-000112f0: 2e73 6563 686f 280a 2020 2020 2020 2020  .secho(.        
-00011300: 2020 2020 2020 2020 2253 6f6e 6720 4944          "Song ID
-00011310: 7320 6d75 7374 2062 6520 696e 7465 6765  s must be intege
-00011320: 7273 2e20 546f 2064 656c 6574 6520 7461  rs. To delete ta
-00011330: 6773 2c20 7061 7373 2074 6865 2027 2d54  gs, pass the '-T
-00011340: 2f2d 2d74 6167 2720 666c 6167 2e22 2c0a  /--tag' flag.",.
-00011350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011360: 6667 3d22 7265 6422 2c0a 2020 2020 2020  fg="red",.      
-00011370: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00011380: 2020 2020 7265 7475 726e 0a0a 2020 2020      return..    
-00011390: 2020 2020 6966 206e 6f74 2066 6f72 6365      if not force
-000113a0: 3a0a 2020 2020 2020 2020 2020 2020 6368  :.            ch
-000113b0: 6172 203d 2069 6e70 7574 280a 2020 2020  ar = input(.    
-000113c0: 2020 2020 2020 2020 2020 2020 6622 4172              f"Ar
-000113d0: 6520 796f 7520 7375 7265 2079 6f75 2077  e you sure you w
-000113e0: 616e 7420 746f 2064 656c 6574 6520 7b6c  ant to delete {l
-000113f0: 656e 2873 6f6e 675f 6964 7329 7d20 736f  en(song_ids)} so
-00011400: 6e67 2873 293f 205b 792f 6e5d 2022 0a20  ng(s)? [y/n] ". 
-00011410: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-00011420: 2020 2020 2020 2020 2020 6966 2063 6861            if cha
-00011430: 722e 6c6f 7765 7228 2920 213d 2022 7922  r.lower() != "y"
-00011440: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00011450: 2020 7072 696e 7428 2244 6964 206e 6f74    print("Did not
-00011460: 2064 656c 6574 652e 2229 0a20 2020 2020   delete.").     
-00011470: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00011480: 6e0a 0a20 2020 2020 2020 2077 6974 6820  n..        with 
-00011490: 6f70 656e 2853 4f4e 4753 5f49 4e46 4f5f  open(SONGS_INFO_
-000114a0: 5041 5448 2c20 2272 222c 2065 6e63 6f64  PATH, "r", encod
-000114b0: 696e 673d 2275 7466 2d38 2229 2061 7320  ing="utf-8") as 
-000114c0: 736f 6e67 735f 6669 6c65 3a0a 2020 2020  songs_file:.    
-000114d0: 2020 2020 2020 2020 6c69 6e65 7320 3d20          lines = 
-000114e0: 736f 6e67 735f 6669 6c65 2e72 6561 6428  songs_file.read(
-000114f0: 292e 7370 6c69 746c 696e 6573 2829 0a0a  ).splitlines()..
-00011500: 2020 2020 2020 2020 2020 2020 746f 5f62              to_b
-00011510: 655f 6465 6c65 7465 6420 3d20 5b5d 0a20  e_deleted = []. 
-00011520: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-00011530: 2069 6e20 7261 6e67 6528 6c65 6e28 6c69   in range(len(li
-00011540: 6e65 7329 293a 0a20 2020 2020 2020 2020  nes)):.         
-00011550: 2020 2020 2020 2064 6574 6169 6c73 203d         details =
-00011560: 206c 696e 6573 5b69 5d2e 7374 7269 7028   lines[i].strip(
-00011570: 292e 7370 6c69 7428 227c 2229 0a20 2020  ).split("|").   
-00011580: 2020 2020 2020 2020 2020 2020 2073 6f6e               son
-00011590: 675f 6964 203d 2069 6e74 2864 6574 6169  g_id = int(detai
-000115a0: 6c73 5b30 5d29 0a20 2020 2020 2020 2020  ls[0]).         
-000115b0: 2020 2020 2020 2069 6620 736f 6e67 5f69         if song_i
-000115c0: 6420 696e 2072 656d 6169 6e69 6e67 5f73  d in remaining_s
-000115d0: 6f6e 675f 6964 733a 0a20 2020 2020 2020  ong_ids:.       
-000115e0: 2020 2020 2020 2020 2020 2020 2072 656d               rem
-000115f0: 6169 6e69 6e67 5f73 6f6e 675f 6964 732e  aining_song_ids.
-00011600: 7265 6d6f 7665 2873 6f6e 675f 6964 290a  remove(song_id).
-00011610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011620: 2020 2020 746f 5f62 655f 6465 6c65 7465      to_be_delete
-00011630: 642e 6170 7065 6e64 2869 290a 0a20 2020  d.append(i)..   
-00011640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011650: 2073 6f6e 675f 6e61 6d65 203d 2064 6574   song_name = det
-00011660: 6169 6c73 5b31 5d0a 2020 2020 2020 2020  ails[1].        
-00011670: 2020 2020 2020 2020 2020 2020 6f73 2e72              os.r
-00011680: 656d 6f76 6528 2020 2320 7265 6d6f 7665  emove(  # remove
-00011690: 2061 6374 7561 6c20 736f 6e67 0a20 2020   actual song.   
+0000ff00: 7562 7072 6f63 6573 732e 7275 6e28 0a20  ubprocess.run(. 
+0000ff10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff20: 2020 205b 0a20 2020 2020 2020 2020 2020     [.           
+0000ff30: 2020 2020 2020 2020 2020 2020 2022 7370               "sp
+0000ff40: 6f74 646c 222c 0a20 2020 2020 2020 2020  otdl",.         
+0000ff50: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0000ff60: 646f 776e 6c6f 6164 222c 0a20 2020 2020  download",.     
+0000ff70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff80: 2020 2070 6174 685f 2c0a 2020 2020 2020     path_,.      
+0000ff90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ffa0: 2020 222d 2d6f 7574 7075 7422 2c0a 2020    "--output",.  
+0000ffb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ffc0: 2020 2020 2020 227b 7469 746c 657d 2e7b        "{title}.{
+0000ffd0: 6f75 7470 7574 2d65 7874 7d22 2c0a 2020  output-ext}",.  
+0000ffe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fff0: 2020 2020 2020 222d 2d66 6f72 6d61 7422        "--format"
+00010000: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00010010: 2020 2020 2020 2020 2020 666f 726d 6174            format
+00010020: 5f2c 0a20 2020 2020 2020 2020 2020 2020  _,.             
+00010030: 2020 2020 2020 2020 2020 2022 2d2d 6865             "--he
+00010040: 6164 6c65 7373 222c 0a20 2020 2020 2020  adless",.       
+00010050: 2020 2020 2020 2020 2020 2020 205d 2c0a               ],.
+00010060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010070: 2020 2020 6368 6563 6b3d 5472 7565 2c0a      check=True,.
+00010080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010090: 290a 2020 2020 2020 2020 2020 2020 6578  ).            ex
+000100a0: 6365 7074 2045 7863 6570 7469 6f6e 2061  cept Exception a
+000100b0: 7320 6572 723a 0a20 2020 2020 2020 2020  s err:.         
+000100c0: 2020 2020 2020 206f 732e 6368 6469 7228         os.chdir(
+000100d0: 6377 6429 0a20 2020 2020 2020 2020 2020  cwd).           
+000100e0: 2020 2020 2072 6169 7365 2065 7272 0a0a       raise err..
+000100f0: 2020 2020 2020 2020 7061 7468 7320 3d20          paths = 
+00010100: 5b5d 0a20 2020 2020 2020 2066 6f72 2066  [].        for f
+00010110: 6e61 6d65 2069 6e20 6f73 2e6c 6973 7464  name in os.listd
+00010120: 6972 284d 4145 5354 524f 5f44 4952 293a  ir(MAESTRO_DIR):
+00010130: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00010140: 2066 2069 6e20 5b22 2e77 6176 222c 2022   f in [".wav", "
+00010150: 2e6d 7033 222c 2022 2e66 6c61 6322 2c20  .mp3", ".flac", 
+00010160: 222e 6f67 6722 5d3a 0a20 2020 2020 2020  ".ogg"]:.       
+00010170: 2020 2020 2020 2020 2069 6620 666e 616d           if fnam
+00010180: 652e 656e 6473 7769 7468 2866 293a 0a20  e.endswith(f):. 
+00010190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000101a0: 2020 2072 6177 5f70 6174 6820 3d20 6f73     raw_path = os
+000101b0: 2e70 6174 682e 6a6f 696e 284d 4145 5354  .path.join(MAEST
+000101c0: 524f 5f44 4952 2c20 666e 616d 6529 0a20  RO_DIR, fname). 
+000101d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000101e0: 2020 2073 616e 6974 697a 6564 5f70 6174     sanitized_pat
+000101f0: 6820 3d20 7261 775f 7061 7468 2e72 6570  h = raw_path.rep
+00010200: 6c61 6365 2822 7c22 2c20 222d 2229 0a0a  lace("|", "-")..
+00010210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010220: 2020 2020 6f73 2e72 656e 616d 6528 7261      os.rename(ra
+00010230: 775f 7061 7468 2c20 7361 6e69 7469 7a65  w_path, sanitize
+00010240: 645f 7061 7468 290a 0a20 2020 2020 2020  d_path)..       
+00010250: 2020 2020 2020 2020 2020 2020 2070 6174               pat
+00010260: 6873 2e61 7070 656e 6428 7361 6e69 7469  hs.append(saniti
+00010270: 7a65 645f 7061 7468 290a 2020 2020 2020  zed_path).      
+00010280: 2020 2020 2020 6966 2066 6e61 6d65 2e65        if fname.e
+00010290: 6e64 7377 6974 6828 222e 7061 7274 2229  ndswith(".part")
+000102a0: 3a20 2023 2064 656c 6574 6520 696e 636f  :  # delete inco
+000102b0: 6d70 6c65 7465 2064 6f77 6e6c 6f61 6473  mplete downloads
+000102c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000102d0: 206f 732e 7265 6d6f 7665 286f 732e 7061   os.remove(os.pa
+000102e0: 7468 2e6a 6f69 6e28 4d41 4553 5452 4f5f  th.join(MAESTRO_
+000102f0: 4449 522c 2066 6e61 6d65 2929 0a0a 2020  DIR, fname))..  
+00010300: 2020 2020 2020 6d6f 7665 5f20 3d20 5472        move_ = Tr
+00010310: 7565 0a0a 2020 2020 6966 2070 6174 6873  ue..    if paths
+00010320: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+00010330: 2020 6966 206f 732e 7061 7468 2e69 7364    if os.path.isd
+00010340: 6972 2870 6174 685f 293a 0a20 2020 2020  ir(path_):.     
+00010350: 2020 2020 2020 2070 6174 6873 203d 205b         paths = [
+00010360: 5d0a 2020 2020 2020 2020 2020 2020 6966  ].            if
+00010370: 2072 6563 7572 7365 3a0a 2020 2020 2020   recurse:.      
+00010380: 2020 2020 2020 2020 2020 666f 7220 6469            for di
+00010390: 7270 6174 682c 205f 2c20 666e 616d 6573  rpath, _, fnames
+000103a0: 2069 6e20 6f73 2e77 616c 6b28 7061 7468   in os.walk(path
+000103b0: 5f29 3a0a 2020 2020 2020 2020 2020 2020  _):.            
+000103c0: 2020 2020 2020 2020 666f 7220 666e 616d          for fnam
+000103d0: 6520 696e 2066 6e61 6d65 733a 0a20 2020  e in fnames:.   
+000103e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000103f0: 2020 2020 2069 6620 6f73 2e70 6174 682e       if os.path.
+00010400: 7370 6c69 7465 7874 2866 6e61 6d65 295b  splitext(fname)[
+00010410: 315d 2069 6e20 4558 5453 3a0a 2020 2020  1] in EXTS:.    
+00010420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010430: 2020 2020 2020 2020 7061 7468 732e 6170          paths.ap
+00010440: 7065 6e64 286f 732e 7061 7468 2e6a 6f69  pend(os.path.joi
+00010450: 6e28 6469 7270 6174 682c 2066 6e61 6d65  n(dirpath, fname
+00010460: 2929 0a20 2020 2020 2020 2020 2020 2065  )).            e
+00010470: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00010480: 2020 2020 2066 6f72 2066 6e61 6d65 2069       for fname i
+00010490: 6e20 6f73 2e6c 6973 7464 6972 2870 6174  n os.listdir(pat
+000104a0: 685f 293a 0a20 2020 2020 2020 2020 2020  h_):.           
+000104b0: 2020 2020 2020 2020 2069 6620 6f73 2e70           if os.p
+000104c0: 6174 682e 7370 6c69 7465 7874 2866 6e61  ath.splitext(fna
+000104d0: 6d65 295b 315d 2069 6e20 4558 5453 3a0a  me)[1] in EXTS:.
+000104e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000104f0: 2020 2020 2020 2020 6675 6c6c 5f70 6174          full_pat
+00010500: 6820 3d20 6f73 2e70 6174 682e 6a6f 696e  h = os.path.join
+00010510: 2870 6174 685f 2c20 666e 616d 6529 0a20  (path_, fname). 
+00010520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010530: 2020 2020 2020 2069 6620 6f73 2e70 6174         if os.pat
+00010540: 682e 6973 6669 6c65 2866 756c 6c5f 7061  h.isfile(full_pa
+00010550: 7468 293a 0a20 2020 2020 2020 2020 2020  th):.           
+00010560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010570: 2070 6174 6873 2e61 7070 656e 6428 6675   paths.append(fu
+00010580: 6c6c 5f70 6174 6829 0a20 2020 2020 2020  ll_path).       
+00010590: 2020 2020 2069 6620 6c65 6e28 7061 7468       if len(path
+000105a0: 7329 203d 3d20 303a 0a20 2020 2020 2020  s) == 0:.       
+000105b0: 2020 2020 2020 2020 2063 6c69 636b 2e73           click.s
+000105c0: 6563 686f 280a 2020 2020 2020 2020 2020  echo(.          
+000105d0: 2020 2020 2020 2020 2020 6622 4e6f 2073            f"No s
+000105e0: 6f6e 6773 2066 6f75 6e64 2069 6e20 277b  ongs found in '{
+000105f0: 7061 7468 5f7d 272e 222c 0a20 2020 2020  path_}'.",.     
+00010600: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00010610: 673d 2272 6564 222c 0a20 2020 2020 2020  g="red",.       
+00010620: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00010630: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00010640: 6e0a 2020 2020 2020 2020 656c 7365 3a0a  n.        else:.
+00010650: 2020 2020 2020 2020 2020 2020 7061 7468              path
+00010660: 7320 3d20 5b70 6174 685f 5d0a 0a20 2020  s = [path_]..   
+00010670: 2069 6620 6c65 6e28 7061 7468 7329 203e   if len(paths) >
+00010680: 2031 3a0a 2020 2020 2020 2020 6966 2063   1:.        if c
+00010690: 6c69 7020 6973 206e 6f74 204e 6f6e 653a  lip is not None:
+000106a0: 0a20 2020 2020 2020 2020 2020 2063 6c69  .            cli
+000106b0: 636b 2e73 6563 686f 280a 2020 2020 2020  ck.secho(.      
+000106c0: 2020 2020 2020 2020 2020 2243 616e 6e6f            "Canno
+000106d0: 7420 7061 7373 2027 2d63 2f2d 2d63 6c69  t pass '-c/--cli
+000106e0: 7027 206f 7074 696f 6e20 7768 656e 2061  p' option when a
+000106f0: 6464 696e 6720 6d75 6c74 6970 6c65 2073  dding multiple s
+00010700: 6f6e 6773 2e22 2c0a 2020 2020 2020 2020  ongs.",.        
+00010710: 2020 2020 2020 2020 6667 3d22 7265 6422          fg="red"
+00010720: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
+00010730: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00010740: 726e 0a0a 2020 2020 2020 2020 6966 206e  rn..        if n
+00010750: 616d 6520 6973 206e 6f74 204e 6f6e 653a  ame is not None:
+00010760: 0a20 2020 2020 2020 2020 2020 2063 6c69  .            cli
+00010770: 636b 2e73 6563 686f 280a 2020 2020 2020  ck.secho(.      
+00010780: 2020 2020 2020 2020 2020 2243 616e 6e6f            "Canno
+00010790: 7420 7061 7373 2027 2d6e 2f2d 2d6e 616d  t pass '-n/--nam
+000107a0: 6527 206f 7074 696f 6e20 7768 656e 2061  e' option when a
+000107b0: 6464 696e 6720 6d75 6c74 6970 6c65 2073  dding multiple s
+000107c0: 6f6e 6773 2e22 2c0a 2020 2020 2020 2020  ongs.",.        
+000107d0: 2020 2020 2020 2020 6667 3d22 7265 6422          fg="red"
+000107e0: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
+000107f0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00010800: 726e 0a0a 2020 2020 6966 206c 656e 2870  rn..    if len(p
+00010810: 6174 6873 2920 3d3d 2031 2061 6e64 206e  aths) == 1 and n
+00010820: 616d 6520 6973 206e 6f74 204e 6f6e 653a  ame is not None:
+00010830: 0a20 2020 2020 2020 206e 6577 5f70 6174  .        new_pat
+00010840: 6820 3d20 6f73 2e70 6174 682e 6a6f 696e  h = os.path.join
+00010850: 280a 2020 2020 2020 2020 2020 2020 4d41  (.            MA
+00010860: 4553 5452 4f5f 4449 522c 206e 616d 6520  ESTRO_DIR, name 
+00010870: 2b20 6f73 2e70 6174 682e 7370 6c69 7465  + os.path.splite
+00010880: 7874 2870 6174 6873 5b30 5d29 5b31 5d0a  xt(paths[0])[1].
+00010890: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+000108a0: 2020 2320 6d6f 7665 2f63 6f70 7920 746f    # move/copy to
+000108b0: 204d 4145 5354 524f 5f44 4952 2028 6176   MAESTRO_DIR (av
+000108c0: 6f69 6420 6e61 6d65 2063 6f6e 666c 6963  oid name conflic
+000108d0: 7473 290a 2020 2020 2020 2020 6966 206d  ts).        if m
+000108e0: 6f76 655f 3a0a 2020 2020 2020 2020 2020  ove_:.          
+000108f0: 2020 6d6f 7665 2870 6174 6873 5b30 5d2c    move(paths[0],
+00010900: 206e 6577 5f70 6174 6829 0a20 2020 2020   new_path).     
+00010910: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00010920: 2020 2020 2063 6f70 7928 7061 7468 735b       copy(paths[
+00010930: 305d 2c20 6e65 775f 7061 7468 290a 2020  0], new_path).  
+00010940: 2020 2020 2020 7061 7468 7320 3d20 5b6e        paths = [n
+00010950: 6577 5f70 6174 685d 0a20 2020 2020 2020  ew_path].       
+00010960: 206d 6f76 655f 203d 2054 7275 6520 2023   move_ = True  #
+00010970: 2061 6c77 6179 7320 6d6f 7665 2028 6672   always move (fr
+00010980: 6f6d 2074 656d 7020 6c6f 6320 696e 204d  om temp loc in M
+00010990: 4145 5354 524f 5f44 4952 2920 6966 2072  AESTRO_DIR) if r
+000109a0: 656e 616d 696e 670a 0a20 2020 2069 6620  enaming..    if 
+000109b0: 636c 6970 2069 7320 6e6f 7420 4e6f 6e65  clip is not None
+000109c0: 2061 6e64 206c 656e 2870 6174 6873 2920   and len(paths) 
+000109d0: 3d3d 2031 3a0a 2020 2020 2020 2020 736f  == 1:.        so
+000109e0: 6e67 5f64 7572 6174 696f 6e20 3d20 6d75  ng_duration = mu
+000109f0: 7369 635f 7461 672e 6c6f 6164 5f66 696c  sic_tag.load_fil
+00010a00: 6528 7061 7468 735b 305d 295b 2223 6c65  e(paths[0])["#le
+00010a10: 6e67 7468 225d 2e76 616c 7565 0a0a 2020  ngth"].value..  
+00010a20: 2020 2020 2020 7374 6172 742c 2065 6e64        start, end
+00010a30: 203d 2063 6c69 700a 2020 2020 2020 2020   = clip.        
+00010a40: 6966 2073 7461 7274 203c 2030 3a0a 2020  if start < 0:.  
+00010a50: 2020 2020 2020 2020 2020 636c 6963 6b2e            click.
+00010a60: 7365 6368 6f28 2243 6c69 7020 7374 6172  secho("Clip star
+00010a70: 7420 7469 6d65 2063 616e 6e6f 7420 6265  t time cannot be
+00010a80: 206e 6567 6174 6976 652e 222c 2066 673d   negative.", fg=
+00010a90: 2272 6564 2229 0a20 2020 2020 2020 2020  "red").         
+00010aa0: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
+00010ab0: 2020 6966 2073 7461 7274 203e 2073 6f6e    if start > son
+00010ac0: 675f 6475 7261 7469 6f6e 3a0a 2020 2020  g_duration:.    
+00010ad0: 2020 2020 2020 2020 636c 6963 6b2e 7365          click.se
+00010ae0: 6368 6f28 0a20 2020 2020 2020 2020 2020  cho(.           
+00010af0: 2020 2020 2022 436c 6970 2073 7461 7274       "Clip start
+00010b00: 2074 696d 6520 6361 6e6e 6f74 2062 6520   time cannot be 
+00010b10: 6772 6561 7465 7220 7468 616e 2074 6865  greater than the
+00010b20: 2073 6f6e 6720 6475 7261 7469 6f6e 2e22   song duration."
+00010b30: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00010b40: 2020 6667 3d22 7265 6422 2c0a 2020 2020    fg="red",.    
+00010b50: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00010b60: 2020 2020 2020 7265 7475 726e 0a0a 2020        return..  
+00010b70: 2020 2020 2020 6966 2065 6e64 203d 3d20        if end == 
+00010b80: 2d31 3a0a 2020 2020 2020 2020 2020 2020  -1:.            
+00010b90: 656e 6420 3d20 736f 6e67 5f64 7572 6174  end = song_durat
+00010ba0: 696f 6e0a 2020 2020 2020 2020 656c 6966  ion.        elif
+00010bb0: 2065 6e64 203c 2073 7461 7274 3a0a 2020   end < start:.  
+00010bc0: 2020 2020 2020 2020 2020 636c 6963 6b2e            click.
+00010bd0: 7365 6368 6f28 0a20 2020 2020 2020 2020  secho(.         
+00010be0: 2020 2020 2020 2022 436c 6970 2065 6e64         "Clip end
+00010bf0: 2074 696d 6520 6361 6e6e 6f74 2062 6520   time cannot be 
+00010c00: 6c65 7373 2074 6861 6e20 7468 6520 636c  less than the cl
+00010c10: 6970 2073 7461 7274 2074 696d 652e 222c  ip start time.",
+00010c20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010c30: 2066 673d 2272 6564 222c 0a20 2020 2020   fg="red",.     
+00010c40: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00010c50: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+00010c60: 2020 2020 656c 6966 2065 6e64 203e 2073      elif end > s
+00010c70: 6f6e 675f 6475 7261 7469 6f6e 3a0a 2020  ong_duration:.  
+00010c80: 2020 2020 2020 2020 2020 636c 6963 6b2e            click.
+00010c90: 7365 6368 6f28 0a20 2020 2020 2020 2020  secho(.         
+00010ca0: 2020 2020 2020 2022 436c 6970 2065 6e64         "Clip end
+00010cb0: 2074 696d 6520 6361 6e6e 6f74 2062 6520   time cannot be 
+00010cc0: 6772 6561 7465 7220 7468 616e 2074 6865  greater than the
+00010cd0: 2073 6f6e 6720 6475 7261 7469 6f6e 2e22   song duration."
+00010ce0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00010cf0: 2020 6667 3d22 7265 6422 2c0a 2020 2020    fg="red",.    
+00010d00: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00010d10: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
+00010d20: 2065 6c73 653a 0a20 2020 2020 2020 2073   else:.        s
+00010d30: 7461 7274 203d 2065 6e64 203d 204e 6f6e  tart = end = Non
+00010d40: 650a 0a20 2020 2069 6620 6d65 7461 6461  e..    if metada
+00010d50: 7461 5f70 6169 7273 2069 7320 6e6f 7420  ta_pairs is not 
+00010d60: 4e6f 6e65 2061 6e64 206c 656e 2870 6174  None and len(pat
+00010d70: 6873 2920 3d3d 2031 3a0a 2020 2020 2020  hs) == 1:.      
+00010d80: 2020 2320 636f 6e76 6572 7420 6672 6f6d    # convert from
+00010d90: 2022 6b65 793a 7661 6c75 652c 6b65 793a   "key:value,key:
+00010da0: 7661 6c75 6522 2074 6f20 5b28 226b 6579  value" to [("key
+00010db0: 222c 2022 7661 6c75 6522 295d 0a20 2020  ", "value")].   
+00010dc0: 2020 2020 206d 6574 6164 6174 615f 7061       metadata_pa
+00010dd0: 6972 7320 3d20 5b0a 2020 2020 2020 2020  irs = [.        
+00010de0: 2020 2020 7475 706c 6528 7061 6972 2e73      tuple(pair.s
+00010df0: 7472 6970 2829 2e73 706c 6974 2822 3a22  trip().split(":"
+00010e00: 2929 2066 6f72 2070 6169 7220 696e 206d  )) for pair in m
+00010e10: 6574 6164 6174 615f 7061 6972 732e 7370  etadata_pairs.sp
+00010e20: 6c69 7428 227c 2229 0a20 2020 2020 2020  lit("|").       
+00010e30: 205d 0a20 2020 2020 2020 2073 6f6e 675f   ].        song_
+00010e40: 6461 7461 203d 206d 7573 6963 5f74 6167  data = music_tag
+00010e50: 2e6c 6f61 645f 6669 6c65 2870 6174 6873  .load_file(paths
+00010e60: 5b30 5d29 0a20 2020 2020 2020 2066 6f72  [0]).        for
+00010e70: 206b 6579 2c20 7661 6c75 6520 696e 206d   key, value in m
+00010e80: 6574 6164 6174 615f 7061 6972 733a 0a20  etadata_pairs:. 
+00010e90: 2020 2020 2020 2020 2020 2069 6620 6b65             if ke
+00010ea0: 7920 6e6f 7420 696e 204d 4554 4144 4154  y not in METADAT
+00010eb0: 415f 4b45 5953 206f 7220 6b65 792e 7374  A_KEYS or key.st
+00010ec0: 6172 7473 7769 7468 2822 2322 293a 0a20  artswith("#"):. 
+00010ed0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00010ee0: 6c69 636b 2e73 6563 686f 280a 2020 2020  lick.secho(.    
+00010ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f00: 6622 277b 6b65 797d 2720 6973 206e 6f74  f"'{key}' is not
+00010f10: 2061 2076 616c 6964 2065 6469 7461 626c   a valid editabl
+00010f20: 6520 6d65 7461 6461 7461 206b 6579 2e22  e metadata key."
+00010f30: 2c20 6667 3d22 7265 6422 0a20 2020 2020  , fg="red".     
+00010f40: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00010f50: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+00010f60: 7469 6e75 650a 2020 2020 2020 2020 2020  tinue.          
+00010f70: 2020 736f 6e67 5f64 6174 615b 6b65 795d    song_data[key]
+00010f80: 203d 2076 616c 7565 0a20 2020 2020 2020   = value.       
+00010f90: 2073 6f6e 675f 6461 7461 2e73 6176 6528   song_data.save(
+00010fa0: 290a 0a20 2020 2066 6f72 2070 6174 6820  )..    for path 
+00010fb0: 696e 2070 6174 6873 3a0a 2020 2020 2020  in paths:.      
+00010fc0: 2020 6578 7420 3d20 6f73 2e70 6174 682e    ext = os.path.
+00010fd0: 7370 6c69 7465 7874 2870 6174 6829 5b31  splitext(path)[1
+00010fe0: 5d0a 2020 2020 2020 2020 6966 206e 6f74  ].        if not
+00010ff0: 206f 732e 7061 7468 2e69 7364 6972 2870   os.path.isdir(p
+00011000: 6174 6829 2061 6e64 2065 7874 206e 6f74  ath) and ext not
+00011010: 2069 6e20 4558 5453 3a0a 2020 2020 2020   in EXTS:.      
+00011020: 2020 2020 2020 636c 6963 6b2e 7365 6368        click.sech
+00011030: 6f28 6622 277b 6578 747d 2720 6973 206e  o(f"'{ext}' is n
+00011040: 6f74 2073 7570 706f 7274 6564 2e22 2c20  ot supported.", 
+00011050: 6667 3d22 7265 6422 290a 2020 2020 2020  fg="red").      
+00011060: 2020 2020 2020 7265 7475 726e 0a0a 2020        return..  
+00011070: 2020 2020 2020 666f 7220 7461 6720 696e        for tag in
+00011080: 2074 6167 733a 0a20 2020 2020 2020 2020   tags:.         
+00011090: 2020 2069 6620 222c 2220 696e 2074 6167     if "," in tag
+000110a0: 206f 7220 227c 2220 696e 2074 6167 3a0a   or "|" in tag:.
+000110b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000110c0: 636c 6963 6b2e 7365 6368 6f28 2254 6167  click.secho("Tag
+000110d0: 7320 6361 6e6e 6f74 2063 6f6e 7461 696e  s cannot contain
+000110e0: 2027 2c27 206f 7220 277c 272e 222c 2066   ',' or '|'.", f
+000110f0: 673d 2272 6564 2229 0a20 2020 2020 2020  g="red").       
+00011100: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+00011110: 0a20 2020 2020 2020 2077 6974 6820 6f70  .        with op
+00011120: 656e 2853 4f4e 4753 5f49 4e46 4f5f 5041  en(SONGS_INFO_PA
+00011130: 5448 2c20 2261 2b22 2c20 656e 636f 6469  TH, "a+", encodi
+00011140: 6e67 3d22 7574 662d 3822 2920 6173 2073  ng="utf-8") as s
+00011150: 6f6e 6773 5f66 696c 653a 0a20 2020 2020  ongs_file:.     
+00011160: 2020 2020 2020 2073 6f6e 6773 5f66 696c         songs_fil
+00011170: 652e 7365 656b 2830 2920 2023 2073 7461  e.seek(0)  # sta
+00011180: 7274 2072 6561 6469 6e67 2066 726f 6d20  rt reading from 
+00011190: 6265 6769 6e6e 696e 670a 0a20 2020 2020  beginning..     
+000111a0: 2020 2020 2020 206c 696e 6573 203d 2073         lines = s
+000111b0: 6f6e 6773 5f66 696c 652e 7265 6164 6c69  ongs_file.readli
+000111c0: 6e65 7328 290a 0a20 2020 2020 2020 2020  nes()..         
+000111d0: 2020 2073 6f6e 675f 6964 203d 2031 0a20     song_id = 1. 
+000111e0: 2020 2020 2020 2020 2020 2066 6f72 206c             for l
+000111f0: 696e 6520 696e 206c 696e 6573 3a0a 2020  ine in lines:.  
+00011200: 2020 2020 2020 2020 2020 2020 2020 736f                so
+00011210: 6e67 5f69 6420 3d20 6d61 7828 736f 6e67  ng_id = max(song
+00011220: 5f69 642c 2069 6e74 286c 696e 652e 7370  _id, int(line.sp
+00011230: 6c69 7428 227c 2229 5b30 5d29 202b 2031  lit("|")[0]) + 1
+00011240: 290a 0a20 2020 2020 2020 2020 2020 2070  )..            p
+00011250: 7265 7065 6e64 5f6e 6577 6c69 6e65 203d  repend_newline =
+00011260: 206c 696e 6573 2061 6e64 206c 696e 6573   lines and lines
+00011270: 5b2d 315d 5b2d 315d 2021 3d20 225c 6e22  [-1][-1] != "\n"
+00011280: 0a0a 2020 2020 2020 2020 2020 2020 6164  ..            ad
+00011290: 645f 736f 6e67 280a 2020 2020 2020 2020  d_song(.        
+000112a0: 2020 2020 2020 2020 7061 7468 2c0a 2020          path,.  
+000112b0: 2020 2020 2020 2020 2020 2020 2020 7461                ta
+000112c0: 6773 2c0a 2020 2020 2020 2020 2020 2020  gs,.            
+000112d0: 2020 2020 6d6f 7665 5f2c 0a20 2020 2020      move_,.     
+000112e0: 2020 2020 2020 2020 2020 2073 6f6e 6773             songs
+000112f0: 5f66 696c 652c 0a20 2020 2020 2020 2020  _file,.         
+00011300: 2020 2020 2020 206c 696e 6573 2c0a 2020         lines,.  
+00011310: 2020 2020 2020 2020 2020 2020 2020 736f                so
+00011320: 6e67 5f69 642c 0a20 2020 2020 2020 2020  ng_id,.         
+00011330: 2020 2020 2020 2070 7265 7065 6e64 5f6e         prepend_n
+00011340: 6577 6c69 6e65 2c0a 2020 2020 2020 2020  ewline,.        
+00011350: 2020 2020 2020 2020 7374 6172 742c 0a20          start,. 
+00011360: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00011370: 6e64 2c0a 2020 2020 2020 2020 2020 2020  nd,.            
+00011380: 290a 0a0a 4063 6c69 2e63 6f6d 6d61 6e64  )...@cli.command
+00011390: 2829 0a40 636c 6963 6b2e 6172 6775 6d65  ().@click.argume
+000113a0: 6e74 2822 4152 4753 222c 2072 6571 7569  nt("ARGS", requi
+000113b0: 7265 643d 5472 7565 2c20 6e61 7267 733d  red=True, nargs=
+000113c0: 2d31 290a 4063 6c69 636b 2e6f 7074 696f  -1).@click.optio
+000113d0: 6e28 0a20 2020 2022 2d46 2f2d 6e46 222c  n(.    "-F/-nF",
+000113e0: 2022 2d2d 666f 7263 652f 2d2d 6e6f 2d66   "--force/--no-f
+000113f0: 6f72 6365 222c 2064 6566 6175 6c74 3d46  orce", default=F
+00011400: 616c 7365 2c20 6865 6c70 3d22 466f 7263  alse, help="Forc
+00011410: 6520 6465 6c65 7469 6f6e 2e22 0a29 0a40  e deletion.".).@
+00011420: 636c 6963 6b2e 6f70 7469 6f6e 280a 2020  click.option(.  
+00011430: 2020 222d 542f 2d6e 5422 2c0a 2020 2020    "-T/-nT",.    
+00011440: 222d 2d74 6167 2f2d 2d6e 6f2d 7461 6722  "--tag/--no-tag"
+00011450: 2c0a 2020 2020 6465 6661 756c 743d 4661  ,.    default=Fa
+00011460: 6c73 652c 0a20 2020 2068 656c 703d 2249  lse,.    help="I
+00011470: 6620 7061 7373 6564 2c20 7472 6561 7420  f passed, treat 
+00011480: 616c 6c20 6172 6775 6d65 6e74 7320 6173  all arguments as
+00011490: 2074 6167 732c 2064 656c 6574 696e 6720   tags, deleting 
+000114a0: 6576 6572 7920 6f63 7572 7265 6e63 6520  every ocurrence 
+000114b0: 6f66 2065 6163 6820 7461 672e 222c 0a29  of each tag.",.)
+000114c0: 0a64 6566 2072 656d 6f76 6528 6172 6773  .def remove(args
+000114d0: 2c20 666f 7263 652c 2074 6167 293a 0a20  , force, tag):. 
+000114e0: 2020 2022 2222 5265 6d6f 7665 2065 6974     """Remove eit
+000114f0: 6865 7220 7461 6728 7329 206f 7220 736f  her tag(s) or so
+00011500: 6e67 2873 2920 7061 7373 6564 2061 7320  ng(s) passed as 
+00011510: 4944 2873 292e 2222 220a 2020 2020 6966  ID(s).""".    if
+00011520: 206e 6f74 2074 6167 3a0a 2020 2020 2020   not tag:.      
+00011530: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+00011540: 2020 2073 6f6e 675f 6964 7320 3d20 7b69     song_ids = {i
+00011550: 6e74 2873 6f6e 675f 6964 2920 666f 7220  nt(song_id) for 
+00011560: 736f 6e67 5f69 6420 696e 2061 7267 737d  song_id in args}
+00011570: 0a20 2020 2020 2020 2020 2020 2072 656d  .            rem
+00011580: 6169 6e69 6e67 5f73 6f6e 675f 6964 7320  aining_song_ids 
+00011590: 3d20 7b6e 2066 6f72 206e 2069 6e20 736f  = {n for n in so
+000115a0: 6e67 5f69 6473 7d0a 2020 2020 2020 2020  ng_ids}.        
+000115b0: 6578 6365 7074 2056 616c 7565 4572 726f  except ValueErro
+000115c0: 723a 0a20 2020 2020 2020 2020 2020 2063  r:.            c
+000115d0: 6c69 636b 2e73 6563 686f 280a 2020 2020  lick.secho(.    
+000115e0: 2020 2020 2020 2020 2020 2020 2253 6f6e              "Son
+000115f0: 6720 4944 7320 6d75 7374 2062 6520 696e  g IDs must be in
+00011600: 7465 6765 7273 2e20 546f 2064 656c 6574  tegers. To delet
+00011610: 6520 7461 6773 2c20 7061 7373 2074 6865  e tags, pass the
+00011620: 2027 2d54 2f2d 2d74 6167 2720 666c 6167   '-T/--tag' flag
+00011630: 2e22 2c0a 2020 2020 2020 2020 2020 2020  .",.            
+00011640: 2020 2020 6667 3d22 7265 6422 2c0a 2020      fg="red",.  
+00011650: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00011660: 2020 2020 2020 2020 7265 7475 726e 0a0a          return..
+00011670: 2020 2020 2020 2020 6966 206e 6f74 2066          if not f
+00011680: 6f72 6365 3a0a 2020 2020 2020 2020 2020  orce:.          
+00011690: 2020 6368 6172 203d 2069 6e70 7574 280a    char = input(.
 000116a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000116b0: 2020 2020 206f 732e 7061 7468 2e6a 6f69       os.path.joi
-000116c0: 6e28 534f 4e47 535f 4449 522c 2073 6f6e  n(SONGS_DIR, son
-000116d0: 675f 6e61 6d65 290a 2020 2020 2020 2020  g_name).        
-000116e0: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-000116f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011700: 2020 2063 6c69 636b 2e73 6563 686f 280a     click.secho(.
-00011710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011720: 2020 2020 2020 2020 6622 5265 6d6f 7665          f"Remove
-00011730: 6420 736f 6e67 2027 7b73 6f6e 675f 6e61  d song '{song_na
-00011740: 6d65 7d27 2077 6974 6820 4944 207b 736f  me}' with ID {so
-00011750: 6e67 5f69 647d 2e22 2c0a 2020 2020 2020  ng_id}.",.      
-00011760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011770: 2020 6667 3d22 6772 6565 6e22 2c0a 2020    fg="green",.  
-00011780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011790: 2020 290a 0a20 2020 2020 2020 2066 6f72    )..        for
-000117a0: 2069 2069 6e20 7265 7665 7273 6564 2874   i in reversed(t
-000117b0: 6f5f 6265 5f64 656c 6574 6564 293a 0a20  o_be_deleted):. 
-000117c0: 2020 2020 2020 2020 2020 2064 656c 206c             del l
-000117d0: 696e 6573 5b69 5d0a 0a20 2020 2020 2020  ines[i]..       
-000117e0: 2077 6974 6820 6f70 656e 2853 4f4e 4753   with open(SONGS
-000117f0: 5f49 4e46 4f5f 5041 5448 2c20 2277 222c  _INFO_PATH, "w",
-00011800: 2065 6e63 6f64 696e 673d 2275 7466 2d38   encoding="utf-8
-00011810: 2229 2061 7320 736f 6e67 735f 6669 6c65  ") as songs_file
-00011820: 3a0a 2020 2020 2020 2020 2020 2020 736f  :.            so
-00011830: 6e67 735f 6669 6c65 2e77 7269 7465 2822  ngs_file.write("
-00011840: 5c6e 222e 6a6f 696e 286c 696e 6573 2929  \n".join(lines))
-00011850: 0a0a 2020 2020 2020 2020 666f 7220 7374  ..        for st
-00011860: 6174 735f 6669 6c65 2069 6e20 6f73 2e6c  ats_file in os.l
-00011870: 6973 7464 6972 2853 5441 5453 5f44 4952  istdir(STATS_DIR
-00011880: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
-00011890: 6620 6e6f 7420 7374 6174 735f 6669 6c65  f not stats_file
-000118a0: 2e65 6e64 7377 6974 6828 222e 7478 7422  .endswith(".txt"
-000118b0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000118c0: 2020 2063 6f6e 7469 6e75 650a 0a20 2020     continue..   
-000118d0: 2020 2020 2020 2020 2073 7461 7473 5f70           stats_p
-000118e0: 6174 6820 3d20 6f73 2e70 6174 682e 6a6f  ath = os.path.jo
-000118f0: 696e 2853 5441 5453 5f44 4952 2c20 7374  in(STATS_DIR, st
-00011900: 6174 735f 6669 6c65 290a 2020 2020 2020  ats_file).      
-00011910: 2020 2020 2020 7769 7468 206f 7065 6e28        with open(
-00011920: 7374 6174 735f 7061 7468 2c20 2272 222c  stats_path, "r",
-00011930: 2065 6e63 6f64 696e 673d 2275 7466 2d38   encoding="utf-8
-00011940: 2229 2061 7320 7374 6174 735f 6669 6c65  ") as stats_file
-00011950: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00011960: 2020 7374 6174 735f 6c69 6e65 7320 3d20    stats_lines = 
-00011970: 7374 6174 735f 6669 6c65 2e72 6561 6428  stats_file.read(
-00011980: 292e 7370 6c69 746c 696e 6573 2829 0a0a  ).splitlines()..
-00011990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000119a0: 746f 5f62 655f 6465 6c65 7465 6420 3d20  to_be_deleted = 
-000119b0: 5b5d 0a20 2020 2020 2020 2020 2020 2020  [].             
-000119c0: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-000119d0: 6528 6c65 6e28 7374 6174 735f 6c69 6e65  e(len(stats_line
-000119e0: 7329 293a 0a20 2020 2020 2020 2020 2020  s)):.           
-000119f0: 2020 2020 2020 2020 2064 6574 6169 6c73           details
-00011a00: 203d 2073 7461 7473 5f6c 696e 6573 5b69   = stats_lines[i
-00011a10: 5d2e 7374 7269 7028 292e 7370 6c69 7428  ].strip().split(
-00011a20: 227c 2229 0a20 2020 2020 2020 2020 2020  "|").           
-00011a30: 2020 2020 2020 2020 2073 6f6e 675f 6964           song_id
-00011a40: 203d 2069 6e74 2864 6574 6169 6c73 5b30   = int(details[0
-00011a50: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
-00011a60: 2020 2020 2020 2069 6620 736f 6e67 5f69         if song_i
-00011a70: 6420 696e 2073 6f6e 675f 6964 733a 0a20  d in song_ids:. 
-00011a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a90: 2020 2020 2020 2074 6f5f 6265 5f64 656c         to_be_del
-00011aa0: 6574 6564 2e61 7070 656e 6428 6929 0a0a  eted.append(i)..
-00011ab0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00011ac0: 6920 696e 2072 6576 6572 7365 6428 746f  i in reversed(to
-00011ad0: 5f62 655f 6465 6c65 7465 6429 3a0a 2020  _be_deleted):.  
-00011ae0: 2020 2020 2020 2020 2020 2020 2020 6465                de
-00011af0: 6c20 7374 6174 735f 6c69 6e65 735b 695d  l stats_lines[i]
-00011b00: 0a0a 2020 2020 2020 2020 2020 2020 7769  ..            wi
-00011b10: 7468 206f 7065 6e28 7374 6174 735f 7061  th open(stats_pa
-00011b20: 7468 2c20 2277 222c 2065 6e63 6f64 696e  th, "w", encodin
-00011b30: 673d 2275 7466 2d38 2229 2061 7320 7374  g="utf-8") as st
-00011b40: 6174 735f 6669 6c65 3a0a 2020 2020 2020  ats_file:.      
-00011b50: 2020 2020 2020 2020 2020 7374 6174 735f            stats_
-00011b60: 6669 6c65 2e77 7269 7465 2822 5c6e 222e  file.write("\n".
-00011b70: 6a6f 696e 2873 7461 7473 5f6c 696e 6573  join(stats_lines
-00011b80: 2929 0a0a 2020 2020 2020 2020 6966 2072  ))..        if r
-00011b90: 656d 6169 6e69 6e67 5f73 6f6e 675f 6964  emaining_song_id
-00011ba0: 733a 0a20 2020 2020 2020 2020 2020 2063  s:.            c
-00011bb0: 6c69 636b 2e73 6563 686f 280a 2020 2020  lick.secho(.    
-00011bc0: 2020 2020 2020 2020 2020 2020 6622 436f              f"Co
-00011bd0: 756c 6420 6e6f 7420 6669 6e64 2074 6865  uld not find the
-00011be0: 2066 6f6c 6c6f 7769 6e67 2073 6f6e 6720   following song 
-00011bf0: 4944 733a 207b 272c 2027 2e6a 6f69 6e28  IDs: {', '.join(
-00011c00: 6d61 7028 7374 722c 2072 656d 6169 6e69  map(str, remaini
-00011c10: 6e67 5f73 6f6e 675f 6964 7329 297d 2e22  ng_song_ids))}."
-00011c20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00011c30: 2020 6667 3d22 7265 6422 2c0a 2020 2020    fg="red",.    
-00011c40: 2020 2020 2020 2020 290a 2020 2020 656c          ).    el
-00011c50: 7365 3a0a 2020 2020 2020 2020 7461 6773  se:.        tags
-00011c60: 5f74 6f5f 7265 6d6f 7665 203d 2073 6574  _to_remove = set
-00011c70: 2861 7267 7329 0a20 2020 2020 2020 2069  (args).        i
-00011c80: 6620 6e6f 7420 666f 7263 653a 0a20 2020  f not force:.   
-00011c90: 2020 2020 2020 2020 2063 6861 7220 3d20           char = 
-00011ca0: 696e 7075 7428 0a20 2020 2020 2020 2020  input(.         
-00011cb0: 2020 2020 2020 2066 2241 7265 2079 6f75         f"Are you
-00011cc0: 2073 7572 6520 796f 7520 7761 6e74 2074   sure you want t
-00011cd0: 6f20 6465 6c65 7465 207b 6c65 6e28 7461  o delete {len(ta
-00011ce0: 6773 5f74 6f5f 7265 6d6f 7665 297d 2074  gs_to_remove)} t
-00011cf0: 6167 2873 293f 205b 792f 6e5d 2022 0a20  ag(s)? [y/n] ". 
-00011d00: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-00011d10: 2020 2020 2020 2020 2020 6966 2063 6861            if cha
-00011d20: 722e 6c6f 7765 7228 2920 213d 2022 7922  r.lower() != "y"
-00011d30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00011d40: 2020 7072 696e 7428 2244 6964 206e 6f74    print("Did not
-00011d50: 2064 656c 6574 652e 2229 0a20 2020 2020   delete.").     
-00011d60: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00011d70: 6e0a 0a20 2020 2020 2020 2077 6974 6820  n..        with 
-00011d80: 6f70 656e 2853 4f4e 4753 5f49 4e46 4f5f  open(SONGS_INFO_
-00011d90: 5041 5448 2c20 2272 222c 2065 6e63 6f64  PATH, "r", encod
-00011da0: 696e 673d 2275 7466 2d38 2229 2061 7320  ing="utf-8") as 
-00011db0: 736f 6e67 735f 6669 6c65 3a0a 2020 2020  songs_file:.    
-00011dc0: 2020 2020 2020 2020 6c69 6e65 7320 3d20          lines = 
-00011dd0: 736f 6e67 735f 6669 6c65 2e72 6561 6428  songs_file.read(
-00011de0: 292e 7370 6c69 746c 696e 6573 2829 0a20  ).splitlines(). 
-00011df0: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-00011e00: 2069 6e20 7261 6e67 6528 6c65 6e28 6c69   in range(len(li
-00011e10: 6e65 7329 293a 0a20 2020 2020 2020 2020  nes)):.         
-00011e20: 2020 2020 2020 2064 6574 6169 6c73 203d         details =
-00011e30: 206c 696e 6573 5b69 5d2e 7374 7269 7028   lines[i].strip(
-00011e40: 292e 7370 6c69 7428 227c 2229 0a20 2020  ).split("|").   
-00011e50: 2020 2020 2020 2020 2020 2020 2074 6167               tag
-00011e60: 7320 3d20 6465 7461 696c 735b 325d 2e73  s = details[2].s
-00011e70: 706c 6974 2822 2c22 290a 2020 2020 2020  plit(",").      
-00011e80: 2020 2020 2020 2020 2020 666f 7220 6a20            for j 
-00011e90: 696e 2072 616e 6765 286c 656e 2874 6167  in range(len(tag
-00011ea0: 7329 293a 0a20 2020 2020 2020 2020 2020  s)):.           
-00011eb0: 2020 2020 2020 2020 2069 6620 7461 6773           if tags
-00011ec0: 5b6a 5d20 696e 2074 6167 735f 746f 5f72  [j] in tags_to_r
-00011ed0: 656d 6f76 653a 0a20 2020 2020 2020 2020  emove:.         
-00011ee0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00011ef0: 656c 2074 6167 735b 6a5d 0a20 2020 2020  el tags[j].     
-00011f00: 2020 2020 2020 2020 2020 2064 6574 6169             detai
-00011f10: 6c73 5b32 5d20 3d20 222c 222e 6a6f 696e  ls[2] = ",".join
-00011f20: 2874 6167 7329 0a20 2020 2020 2020 2020  (tags).         
-00011f30: 2020 2020 2020 206c 696e 6573 5b69 5d20         lines[i] 
-00011f40: 3d20 227c 222e 6a6f 696e 2864 6574 6169  = "|".join(detai
-00011f50: 6c73 290a 0a20 2020 2020 2020 2077 6974  ls)..        wit
-00011f60: 6820 6f70 656e 2853 4f4e 4753 5f49 4e46  h open(SONGS_INF
-00011f70: 4f5f 5041 5448 2c20 2277 222c 2065 6e63  O_PATH, "w", enc
-00011f80: 6f64 696e 673d 2275 7466 2d38 2229 2061  oding="utf-8") a
-00011f90: 7320 736f 6e67 735f 6669 6c65 3a0a 2020  s songs_file:.  
-00011fa0: 2020 2020 2020 2020 2020 736f 6e67 735f            songs_
-00011fb0: 6669 6c65 2e77 7269 7465 2822 5c6e 222e  file.write("\n".
-00011fc0: 6a6f 696e 286c 696e 6573 2929 0a0a 2020  join(lines))..  
-00011fd0: 2020 2020 2020 636c 6963 6b2e 7365 6368        click.sech
-00011fe0: 6f28 0a20 2020 2020 2020 2020 2020 2066  o(.            f
-00011ff0: 2244 656c 6574 6564 2061 6c6c 206f 6363  "Deleted all occ
-00012000: 7572 7265 6e63 6573 206f 6620 7b6c 656e  urrences of {len
-00012010: 2874 6167 735f 746f 5f72 656d 6f76 6529  (tags_to_remove)
-00012020: 7d20 7461 6728 7329 2e22 2c0a 2020 2020  } tag(s).",.    
-00012030: 2020 2020 2020 2020 6667 3d22 6772 6565          fg="gree
-00012040: 6e22 2c0a 2020 2020 2020 2020 290a 0a0a  n",.        )...
-00012050: 4063 6c69 2e63 6f6d 6d61 6e64 286e 616d  @cli.command(nam
-00012060: 653d 2274 6167 2229 0a40 636c 6963 6b2e  e="tag").@click.
-00012070: 6172 6775 6d65 6e74 2822 736f 6e67 5f69  argument("song_i
-00012080: 6473 222c 2074 7970 653d 636c 6963 6b2e  ds", type=click.
-00012090: 494e 542c 2072 6571 7569 7265 643d 5472  INT, required=Tr
-000120a0: 7565 2c20 6e61 7267 733d 2d31 290a 4063  ue, nargs=-1).@c
-000120b0: 6c69 636b 2e6f 7074 696f 6e28 0a20 2020  lick.option(.   
-000120c0: 2022 2d74 222c 0a20 2020 2022 2d2d 7461   "-t",.    "--ta
-000120d0: 6722 2c0a 2020 2020 2274 6167 7322 2c0a  g",.    "tags",.
-000120e0: 2020 2020 6865 6c70 3d22 5461 6773 2074      help="Tags t
-000120f0: 6f20 6164 642e 222c 0a20 2020 206d 756c  o add.",.    mul
-00012100: 7469 706c 653d 5472 7565 2c0a 290a 6465  tiple=True,.).de
-00012110: 6620 7461 675f 2873 6f6e 675f 6964 732c  f tag_(song_ids,
-00012120: 2074 6167 7329 3a0a 2020 2020 2222 2241   tags):.    """A
-00012130: 6464 2074 6167 7320 746f 2061 2073 6f6e  dd tags to a son
-00012140: 6720 2870 6173 7365 6420 6173 2049 4429  g (passed as ID)
-00012150: 2e20 5461 6773 2063 616e 6e6f 7420 636f  . Tags cannot co
-00012160: 6e74 6169 6e20 7468 6520 6368 6172 6163  ntain the charac
-00012170: 7465 7273 0a20 2020 2027 2c27 206f 7220  ters.    ',' or 
-00012180: 277c 272e 2222 220a 2020 2020 736f 6e67  '|'.""".    song
-00012190: 5f69 6473 203d 2073 6574 2873 6f6e 675f  _ids = set(song_
-000121a0: 6964 7329 0a20 2020 206e 756d 5f73 6f6e  ids).    num_son
-000121b0: 6773 203d 206c 656e 2873 6f6e 675f 6964  gs = len(song_id
-000121c0: 7329 0a20 2020 2074 6167 7320 3d20 7365  s).    tags = se
-000121d0: 7428 7461 6773 290a 2020 2020 666f 7220  t(tags).    for 
-000121e0: 7461 6720 696e 2074 6167 733a 0a20 2020  tag in tags:.   
-000121f0: 2020 2020 2069 6620 222c 2220 696e 2074       if "," in t
-00012200: 6167 206f 7220 227c 2220 696e 2074 6167  ag or "|" in tag
-00012210: 3a0a 2020 2020 2020 2020 2020 2020 636c  :.            cl
-00012220: 6963 6b2e 7365 6368 6f28 2254 6167 7320  ick.secho("Tags 
-00012230: 6361 6e6e 6f74 2063 6f6e 7461 696e 2027  cannot contain '
-00012240: 2c27 206f 7220 277c 272e 222c 2066 673d  ,' or '|'.", fg=
-00012250: 2272 6564 2229 0a20 2020 2020 2020 2020  "red").         
-00012260: 2020 2072 6574 7572 6e0a 2020 2020 6966     return.    if
-00012270: 2074 6167 733a 0a20 2020 2020 2020 2073   tags:.        s
-00012280: 6f6e 6773 5f66 696c 6520 3d20 6f70 656e  ongs_file = open
-00012290: 2853 4f4e 4753 5f49 4e46 4f5f 5041 5448  (SONGS_INFO_PATH
-000122a0: 2c20 2272 222c 2065 6e63 6f64 696e 673d  , "r", encoding=
-000122b0: 2275 7466 2d38 2229 0a20 2020 2020 2020  "utf-8").       
-000122c0: 206c 696e 6573 203d 2073 6f6e 6773 5f66   lines = songs_f
-000122d0: 696c 652e 7265 6164 2829 2e73 706c 6974  ile.read().split
-000122e0: 6c69 6e65 7328 290a 2020 2020 2020 2020  lines().        
-000122f0: 666f 7220 6920 696e 2072 616e 6765 286c  for i in range(l
-00012300: 656e 286c 696e 6573 2929 3a0a 2020 2020  en(lines)):.    
-00012310: 2020 2020 2020 2020 6465 7461 696c 7320          details 
-00012320: 3d20 6c69 6e65 735b 695d 2e73 7472 6970  = lines[i].strip
-00012330: 2829 2e73 706c 6974 2822 7c22 290a 2020  ().split("|").  
-00012340: 2020 2020 2020 2020 2020 736f 6e67 5f69            song_i
-00012350: 6420 3d20 696e 7428 6465 7461 696c 735b  d = int(details[
-00012360: 305d 290a 2020 2020 2020 2020 2020 2020  0]).            
-00012370: 6966 2073 6f6e 675f 6964 2069 6e20 736f  if song_id in so
-00012380: 6e67 5f69 6473 3a0a 2020 2020 2020 2020  ng_ids:.        
-00012390: 2020 2020 2020 2020 736f 6e67 5f69 6473          song_ids
-000123a0: 2e72 656d 6f76 6528 736f 6e67 5f69 6429  .remove(song_id)
-000123b0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000123c0: 2020 6966 2064 6574 6169 6c73 5b32 5d3a    if details[2]:
-000123d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000123e0: 2020 2020 206e 6577 5f74 6167 7320 3d20       new_tags = 
-000123f0: 6465 7461 696c 735b 325d 2e73 706c 6974  details[2].split
-00012400: 2822 2c22 290a 2020 2020 2020 2020 2020  (",").          
-00012410: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00012420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012430: 6e65 775f 7461 6773 203d 205b 5d0a 2020  new_tags = [].  
-00012440: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
-00012450: 775f 7461 6773 202b 3d20 5b74 6167 2066  w_tags += [tag f
-00012460: 6f72 2074 6167 2069 6e20 7461 6773 2069  or tag in tags i
-00012470: 6620 7461 6720 6e6f 7420 696e 206e 6577  f tag not in new
-00012480: 5f74 6167 735d 0a20 2020 2020 2020 2020  _tags].         
-00012490: 2020 2020 2020 2064 6574 6169 6c73 5b32         details[2
-000124a0: 5d20 3d20 222c 222e 6a6f 696e 286e 6577  ] = ",".join(new
-000124b0: 5f74 6167 7329 0a20 2020 2020 2020 2020  _tags).         
-000124c0: 2020 2020 2020 206c 696e 6573 5b69 5d20         lines[i] 
-000124d0: 3d20 227c 222e 6a6f 696e 2864 6574 6169  = "|".join(detai
-000124e0: 6c73 290a 2020 2020 2020 2020 736f 6e67  ls).        song
-000124f0: 735f 6669 6c65 2e63 6c6f 7365 2829 0a0a  s_file.close()..
-00012500: 2020 2020 2020 2020 736f 6e67 735f 6669          songs_fi
-00012510: 6c65 203d 206f 7065 6e28 534f 4e47 535f  le = open(SONGS_
-00012520: 494e 464f 5f50 4154 482c 2022 7722 2c20  INFO_PATH, "w", 
-00012530: 656e 636f 6469 6e67 3d22 7574 662d 3822  encoding="utf-8"
-00012540: 290a 2020 2020 2020 2020 736f 6e67 735f  ).        songs_
-00012550: 6669 6c65 2e77 7269 7465 2822 5c6e 222e  file.write("\n".
-00012560: 6a6f 696e 286c 696e 6573 2929 0a20 2020  join(lines)).   
-00012570: 2020 2020 2073 6f6e 6773 5f66 696c 652e       songs_file.
-00012580: 636c 6f73 6528 290a 0a20 2020 2020 2020  close()..       
-00012590: 2069 6620 736f 6e67 5f69 6473 3a0a 2020   if song_ids:.  
-000125a0: 2020 2020 2020 2020 2020 636c 6963 6b2e            click.
-000125b0: 7365 6368 6f28 0a20 2020 2020 2020 2020  secho(.         
-000125c0: 2020 2020 2020 2066 2243 6f75 6c64 206e         f"Could n
-000125d0: 6f74 2066 696e 6420 736f 6e67 2873 2920  ot find song(s) 
-000125e0: 7769 7468 2049 4428 7329 207b 272c 2027  with ID(s) {', '
-000125f0: 2e6a 6f69 6e28 6d61 7028 7374 722c 2073  .join(map(str, s
-00012600: 6f6e 675f 6964 7329 297d 2e22 2c0a 2020  ong_ids))}.",.  
-00012610: 2020 2020 2020 2020 2020 2020 2020 6667                fg
-00012620: 3d22 7265 6422 2c0a 2020 2020 2020 2020  ="red",.        
-00012630: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00012640: 2020 6966 206c 656e 2873 6f6e 675f 6964    if len(song_id
-00012650: 7329 203d 3d20 6e75 6d5f 736f 6e67 733a  s) == num_songs:
-00012660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012670: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
-00012680: 636c 6963 6b2e 7365 6368 6f28 0a20 2020  click.secho(.   
-00012690: 2020 2020 2020 2020 2066 2241 6464 6564           f"Added
-000126a0: 207b 6c65 6e28 7461 6773 297d 2074 6167   {len(tags)} tag
-000126b0: 2873 2920 746f 207b 6e75 6d5f 736f 6e67  (s) to {num_song
-000126c0: 7320 2d20 6c65 6e28 736f 6e67 5f69 6473  s - len(song_ids
-000126d0: 297d 2073 6f6e 6728 7329 2e22 2c0a 2020  )} song(s).",.  
-000126e0: 2020 2020 2020 2020 2020 6667 3d22 6772            fg="gr
-000126f0: 6565 6e22 2c0a 2020 2020 2020 2020 290a  een",.        ).
-00012700: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00012710: 2020 636c 6963 6b2e 7365 6368 6f28 224e    click.secho("N
-00012720: 6f20 7461 6773 2070 6173 7365 642e 222c  o tags passed.",
-00012730: 2066 673d 2272 6564 2229 0a0a 0a40 636c   fg="red")...@cl
-00012740: 692e 636f 6d6d 616e 6428 290a 4063 6c69  i.command().@cli
-00012750: 636b 2e61 7267 756d 656e 7428 2273 6f6e  ck.argument("son
-00012760: 675f 6964 7322 2c20 7479 7065 3d63 6c69  g_ids", type=cli
-00012770: 636b 2e49 4e54 2c20 7265 7175 6972 6564  ck.INT, required
-00012780: 3d54 7275 652c 206e 6172 6773 3d2d 3129  =True, nargs=-1)
-00012790: 0a40 636c 6963 6b2e 6f70 7469 6f6e 280a  .@click.option(.
-000127a0: 2020 2020 222d 7422 2c0a 2020 2020 222d      "-t",.    "-
-000127b0: 2d74 6167 222c 0a20 2020 2022 7461 6773  -tag",.    "tags
-000127c0: 222c 0a20 2020 2068 656c 703d 2254 6167  ",.    help="Tag
-000127d0: 7320 746f 2072 656d 6f76 652e 222c 0a20  s to remove.",. 
-000127e0: 2020 206d 756c 7469 706c 653d 5472 7565     multiple=True
-000127f0: 2c0a 290a 4063 6c69 636b 2e6f 7074 696f  ,.).@click.optio
-00012800: 6e28 222d 412f 2d6e 4122 2c20 222d 2d61  n("-A/-nA", "--a
-00012810: 6c6c 2f2d 2d6e 6f2d 616c 6c22 2c20 2261  ll/--no-all", "a
-00012820: 6c6c 5f22 2c20 6465 6661 756c 743d 4661  ll_", default=Fa
-00012830: 6c73 6529 0a64 6566 2075 6e74 6167 2873  lse).def untag(s
-00012840: 6f6e 675f 6964 732c 2074 6167 732c 2061  ong_ids, tags, a
-00012850: 6c6c 5f29 3a0a 2020 2020 2222 2252 656d  ll_):.    """Rem
-00012860: 6f76 6520 7461 6773 2066 726f 6d20 6120  ove tags from a 
-00012870: 7370 6563 6966 6963 2073 6f6e 6720 2870  specific song (p
-00012880: 6173 7365 6420 6173 2049 4429 2e20 5461  assed as ID). Ta
-00012890: 6773 2074 6861 7420 7468 6520 736f 6e67  gs that the song
-000128a0: 0a20 2020 2064 6f65 736e 2774 2068 6176  .    doesn't hav
-000128b0: 6520 7769 6c6c 2062 6520 6967 6e6f 7265  e will be ignore
-000128c0: 642e 0a0a 2020 2020 5061 7373 696e 6720  d...    Passing 
-000128d0: 7468 6520 272d 412f 2d2d 616c 6c27 2066  the '-A/--all' f
-000128e0: 6c61 6720 7769 6c6c 2072 656d 6f76 6520  lag will remove 
-000128f0: 616c 6c20 7461 6773 2066 726f 6d20 7468  all tags from th
-00012900: 6520 736f 6e67 2c20 756e 6c65 7373 2054  e song, unless T
-00012910: 4147 530a 2020 2020 6973 2070 6173 7365  AGS.    is passe
-00012920: 6420 2869 6e20 7768 6963 6820 6361 7365  d (in which case
-00012930: 2074 6865 2066 6c61 6720 6973 2069 676e   the flag is ign
-00012940: 6f72 6564 292e 2222 220a 2020 2020 736f  ored).""".    so
-00012950: 6e67 5f69 6473 203d 2073 6574 2873 6f6e  ng_ids = set(son
-00012960: 675f 6964 7329 0a20 2020 206e 756d 5f73  g_ids).    num_s
-00012970: 6f6e 6773 203d 206c 656e 2873 6f6e 675f  ongs = len(song_
-00012980: 6964 7329 0a20 2020 2074 6167 7320 3d20  ids).    tags = 
-00012990: 7365 7428 7461 6773 290a 2020 2020 6966  set(tags).    if
-000129a0: 2074 6167 733a 0a20 2020 2020 2020 2073   tags:.        s
-000129b0: 6f6e 6773 5f66 696c 6520 3d20 6f70 656e  ongs_file = open
-000129c0: 2853 4f4e 4753 5f49 4e46 4f5f 5041 5448  (SONGS_INFO_PATH
-000129d0: 2c20 2272 222c 2065 6e63 6f64 696e 673d  , "r", encoding=
-000129e0: 2275 7466 2d38 2229 0a20 2020 2020 2020  "utf-8").       
-000129f0: 206c 696e 6573 203d 2073 6f6e 6773 5f66   lines = songs_f
-00012a00: 696c 652e 7265 6164 2829 2e73 706c 6974  ile.read().split
-00012a10: 6c69 6e65 7328 290a 2020 2020 2020 2020  lines().        
-00012a20: 666f 7220 6920 696e 2072 616e 6765 286c  for i in range(l
-00012a30: 656e 286c 696e 6573 2929 3a0a 2020 2020  en(lines)):.    
-00012a40: 2020 2020 2020 2020 6465 7461 696c 7320          details 
-00012a50: 3d20 6c69 6e65 735b 695d 2e73 7472 6970  = lines[i].strip
-00012a60: 2829 2e73 706c 6974 2822 7c22 290a 2020  ().split("|").  
-00012a70: 2020 2020 2020 2020 2020 736f 6e67 5f69            song_i
-00012a80: 6420 3d20 696e 7428 6465 7461 696c 735b  d = int(details[
-00012a90: 305d 290a 2020 2020 2020 2020 2020 2020  0]).            
-00012aa0: 6966 2073 6f6e 675f 6964 2069 6e20 736f  if song_id in so
-00012ab0: 6e67 5f69 6473 3a0a 2020 2020 2020 2020  ng_ids:.        
-00012ac0: 2020 2020 2020 2020 736f 6e67 5f69 6473          song_ids
-00012ad0: 2e72 656d 6f76 6528 736f 6e67 5f69 6429  .remove(song_id)
-00012ae0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012af0: 2020 7461 6773 5f74 6f5f 6b65 6570 203d    tags_to_keep =
-00012b00: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
-00012b10: 2020 2020 2020 2074 6167 2066 6f72 2074         tag for t
-00012b20: 6167 2069 6e20 6465 7461 696c 735b 325d  ag in details[2]
-00012b30: 2e73 706c 6974 2822 2c22 2920 6966 2074  .split(",") if t
-00012b40: 6167 206e 6f74 2069 6e20 7461 6773 0a20  ag not in tags. 
-00012b50: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
-00012b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012b70: 206c 696e 6573 5b69 5d20 3d20 227c 222e   lines[i] = "|".
-00012b80: 6a6f 696e 280a 2020 2020 2020 2020 2020  join(.          
-00012b90: 2020 2020 2020 2020 2020 6465 7461 696c            detail
-00012ba0: 735b 3a32 5d20 2b20 5b22 2c22 2e6a 6f69  s[:2] + [",".joi
-00012bb0: 6e28 7461 6773 5f74 6f5f 6b65 6570 295d  n(tags_to_keep)]
-00012bc0: 202b 2064 6574 6169 6c73 5b33 3a5d 0a20   + details[3:]. 
-00012bd0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00012be0: 0a20 2020 2020 2020 2073 6f6e 6773 5f66  .        songs_f
-00012bf0: 696c 652e 636c 6f73 6528 290a 0a20 2020  ile.close()..   
-00012c00: 2020 2020 2073 6f6e 6773 5f66 696c 6520       songs_file 
-00012c10: 3d20 6f70 656e 2853 4f4e 4753 5f49 4e46  = open(SONGS_INF
-00012c20: 4f5f 5041 5448 2c20 2277 222c 2065 6e63  O_PATH, "w", enc
-00012c30: 6f64 696e 673d 2275 7466 2d38 2229 0a20  oding="utf-8"). 
-00012c40: 2020 2020 2020 2073 6f6e 6773 5f66 696c         songs_fil
-00012c50: 652e 7772 6974 6528 225c 6e22 2e6a 6f69  e.write("\n".joi
-00012c60: 6e28 6c69 6e65 7329 290a 2020 2020 2020  n(lines)).      
-00012c70: 2020 736f 6e67 735f 6669 6c65 2e63 6c6f    songs_file.clo
-00012c80: 7365 2829 0a0a 2020 2020 2020 2020 6966  se()..        if
-00012c90: 2073 6f6e 675f 6964 733a 0a20 2020 2020   song_ids:.     
-00012ca0: 2020 2020 2020 2063 6c69 636b 2e73 6563         click.sec
-00012cb0: 686f 280a 2020 2020 2020 2020 2020 2020  ho(.            
-00012cc0: 2020 2020 6622 436f 756c 6420 6e6f 7420      f"Could not 
-00012cd0: 6669 6e64 2073 6f6e 6728 7329 2077 6974  find song(s) wit
-00012ce0: 6820 4944 2873 2920 7b27 2c20 272e 6a6f  h ID(s) {', '.jo
-00012cf0: 696e 286d 6170 2873 7472 2c20 736f 6e67  in(map(str, song
-00012d00: 5f69 6473 2929 7d2e 222c 0a20 2020 2020  _ids))}.",.     
-00012d10: 2020 2020 2020 2020 2020 2066 673d 2272             fg="r
-00012d20: 6564 222c 0a20 2020 2020 2020 2020 2020  ed",.           
-00012d30: 2029 0a20 2020 2020 2020 2020 2020 2069   ).            i
-00012d40: 6620 6c65 6e28 736f 6e67 5f69 6473 2920  f len(song_ids) 
-00012d50: 3d3d 206e 756d 5f73 6f6e 6773 3a0a 2020  == num_songs:.  
-00012d60: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00012d70: 7475 726e 0a20 2020 2020 2020 2063 6c69  turn.        cli
-00012d80: 636b 2e73 6563 686f 280a 2020 2020 2020  ck.secho(.      
-00012d90: 2020 2020 2020 6622 5265 6d6f 7665 6420        f"Removed 
-00012da0: 616e 7920 6f63 6375 7272 656e 6365 7320  any occurrences 
-00012db0: 6f66 207b 6c65 6e28 7461 6773 297d 2074  of {len(tags)} t
-00012dc0: 6167 2873 2920 6672 6f6d 207b 6e75 6d5f  ag(s) from {num_
-00012dd0: 736f 6e67 7320 2d20 6c65 6e28 736f 6e67  songs - len(song
-00012de0: 5f69 6473 297d 2073 6f6e 6728 7329 2e22  _ids)} song(s)."
-00012df0: 2c0a 2020 2020 2020 2020 2020 2020 6667  ,.            fg
-00012e00: 3d22 6772 6565 6e22 2c0a 2020 2020 2020  ="green",.      
-00012e10: 2020 290a 2020 2020 656c 7365 3a0a 2020    ).    else:.  
-00012e20: 2020 2020 2020 6966 206e 6f74 2061 6c6c        if not all
-00012e30: 5f3a 0a20 2020 2020 2020 2020 2020 2063  _:.            c
-00012e40: 6c69 636b 2e73 6563 686f 280a 2020 2020  lick.secho(.    
-00012e50: 2020 2020 2020 2020 2020 2020 224e 6f20              "No 
-00012e60: 7461 6773 2070 6173 7365 64e2 8094 746f  tags passed...to
-00012e70: 2072 656d 6f76 6520 616c 6c20 7461 6773   remove all tags
-00012e80: 2c20 7061 7373 2074 6865 2027 2d41 2f2d  , pass the '-A/-
-00012e90: 2d61 6c6c 2720 666c 6167 2e22 2c0a 2020  -all' flag.",.  
-00012ea0: 2020 2020 2020 2020 2020 2020 2020 6667                fg
-00012eb0: 3d22 7265 6422 2c0a 2020 2020 2020 2020  ="red",.        
-00012ec0: 2020 2020 290a 2020 2020 2020 2020 656c      ).        el
-00012ed0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00012ee0: 736f 6e67 735f 6669 6c65 203d 206f 7065  songs_file = ope
-00012ef0: 6e28 534f 4e47 535f 494e 464f 5f50 4154  n(SONGS_INFO_PAT
-00012f00: 482c 2022 7222 2c20 656e 636f 6469 6e67  H, "r", encoding
-00012f10: 3d22 7574 662d 3822 290a 2020 2020 2020  ="utf-8").      
-00012f20: 2020 2020 2020 6c69 6e65 7320 3d20 736f        lines = so
-00012f30: 6e67 735f 6669 6c65 2e72 6561 6428 292e  ngs_file.read().
-00012f40: 7370 6c69 746c 696e 6573 2829 0a20 2020  splitlines().   
-00012f50: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
-00012f60: 6e20 7261 6e67 6528 6c65 6e28 6c69 6e65  n range(len(line
-00012f70: 7329 293a 0a20 2020 2020 2020 2020 2020  s)):.           
-00012f80: 2020 2020 206c 696e 6520 3d20 6c69 6e65       line = line
-00012f90: 735b 695d 0a20 2020 2020 2020 2020 2020  s[i].           
-00012fa0: 2020 2020 2064 6574 6169 6c73 203d 206c       details = l
-00012fb0: 696e 652e 7374 7269 7028 292e 7370 6c69  ine.strip().spli
-00012fc0: 7428 227c 2229 0a20 2020 2020 2020 2020  t("|").         
-00012fd0: 2020 2020 2020 2069 6620 696e 7428 6465         if int(de
-00012fe0: 7461 696c 735b 305d 2920 696e 2073 6f6e  tails[0]) in son
-00012ff0: 675f 6964 733a 0a20 2020 2020 2020 2020  g_ids:.         
-00013000: 2020 2020 2020 2020 2020 206c 696e 6573             lines
-00013010: 5b69 5d20 3d20 227c 222e 6a6f 696e 2864  [i] = "|".join(d
-00013020: 6574 6169 6c73 5b3a 325d 202b 205b 2222  etails[:2] + [""
-00013030: 5d20 2b20 6465 7461 696c 735b 333a 5d29  ] + details[3:])
-00013040: 0a20 2020 2020 2020 2020 2020 2073 6f6e  .            son
-00013050: 6773 5f66 696c 652e 636c 6f73 6528 290a  gs_file.close().
-00013060: 0a20 2020 2020 2020 2020 2020 2073 6f6e  .            son
-00013070: 6773 5f66 696c 6520 3d20 6f70 656e 2853  gs_file = open(S
-00013080: 4f4e 4753 5f49 4e46 4f5f 5041 5448 2c20  ONGS_INFO_PATH, 
-00013090: 2277 222c 2065 6e63 6f64 696e 673d 2275  "w", encoding="u
-000130a0: 7466 2d38 2229 0a20 2020 2020 2020 2020  tf-8").         
-000130b0: 2020 2073 6f6e 6773 5f66 696c 652e 7772     songs_file.wr
-000130c0: 6974 6528 225c 6e22 2e6a 6f69 6e28 6c69  ite("\n".join(li
-000130d0: 6e65 7329 290a 2020 2020 2020 2020 2020  nes)).          
-000130e0: 2020 736f 6e67 735f 6669 6c65 2e63 6c6f    songs_file.clo
-000130f0: 7365 2829 0a0a 2020 2020 2020 2020 2020  se()..          
-00013100: 2020 636c 6963 6b2e 7365 6368 6f28 0a20    click.secho(. 
-00013110: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00013120: 2252 656d 6f76 6564 207b 6c65 6e28 7461  "Removed {len(ta
-00013130: 6773 297d 2074 6167 2873 2920 6672 6f6d  gs)} tag(s) from
-00013140: 207b 6c65 6e28 736f 6e67 5f69 6473 297d   {len(song_ids)}
-00013150: 2073 6f6e 6728 7329 2e22 2c0a 2020 2020   song(s).",.    
-00013160: 2020 2020 2020 2020 2020 2020 6667 3d22              fg="
-00013170: 6772 6565 6e22 2c0a 2020 2020 2020 2020  green",.        
-00013180: 2020 2020 290a 0a0a 4063 6c69 2e63 6f6d      )...@cli.com
-00013190: 6d61 6e64 2829 0a40 636c 6963 6b2e 6172  mand().@click.ar
-000131a0: 6775 6d65 6e74 2822 7461 6773 222c 206e  gument("tags", n
-000131b0: 6172 6773 3d2d 3129 0a40 636c 6963 6b2e  args=-1).@click.
-000131c0: 6f70 7469 6f6e 280a 2020 2020 222d 7322  option(.    "-s"
-000131d0: 2c0a 2020 2020 222d 2d73 6875 6666 6c65  ,.    "--shuffle
-000131e0: 222c 0a20 2020 2022 7368 7566 666c 655f  ",.    "shuffle_
-000131f0: 222c 0a20 2020 2074 7970 653d 636c 6963  ",.    type=clic
-00013200: 6b2e 496e 7452 616e 6765 2830 2c20 3229  k.IntRange(0, 2)
-00013210: 2c0a 2020 2020 6865 6c70 3d22 303a 2073  ,.    help="0: s
-00013220: 6875 6666 6c65 206f 6e63 652c 2031 3a20  huffle once, 1: 
-00013230: 7368 7566 666c 6520 6576 6572 7920 6c6f  shuffle every lo
-00013240: 6f70 2c20 323a 2073 6875 6666 6c65 2065  op, 2: shuffle e
-00013250: 7665 7279 206c 6f6f 7020 6578 6365 7074  very loop except
-00013260: 2066 6f72 2074 6865 2066 6972 7374 206f   for the first o
-00013270: 6e65 2e22 2c0a 290a 4063 6c69 636b 2e6f  ne.",.).@click.o
-00013280: 7074 696f 6e28 0a20 2020 2022 2d52 2f2d  ption(.    "-R/-
-00013290: 6e52 222c 0a20 2020 2022 2d2d 7265 7665  nR",.    "--reve
-000132a0: 7273 652f 2d2d 6e6f 2d72 6576 6572 7365  rse/--no-reverse
-000132b0: 222c 0a20 2020 2022 7265 7665 7273 6522  ",.    "reverse"
-000132c0: 2c0a 2020 2020 6465 6661 756c 743d 4661  ,.    default=Fa
-000132d0: 6c73 652c 0a20 2020 2068 656c 703d 2250  lse,.    help="P
-000132e0: 6c61 7920 736f 6e67 7320 696e 2072 6576  lay songs in rev
-000132f0: 6572 7365 2028 6d6f 7374 2072 6563 656e  erse (most recen
-00013300: 746c 7920 6164 6465 6420 6669 7273 7429  tly added first)
-00013310: 2e22 2c0a 290a 4063 6c69 636b 2e6f 7074  .",.).@click.opt
-00013320: 696f 6e28 0a20 2020 2022 2d6f 222c 0a20  ion(.    "-o",. 
-00013330: 2020 2022 2d2d 6f6e 6c79 222c 0a20 2020     "--only",.   
-00013340: 2022 6f6e 6c79 222c 0a20 2020 2074 7970   "only",.    typ
-00013350: 653d 636c 6963 6b2e 494e 542c 0a20 2020  e=click.INT,.   
-00013360: 206d 756c 7469 706c 653d 5472 7565 2c0a   multiple=True,.
-00013370: 2020 2020 6865 6c70 3d22 506c 6179 206f      help="Play o
-00013380: 6e6c 7920 7468 6973 2f74 6865 7365 2073  nly this/these s
-00013390: 6f6e 6728 7329 2028 6361 6e20 6265 2070  ong(s) (can be p
-000133a0: 6173 7365 6420 6d75 6c74 6970 6c65 2074  assed multiple t
-000133b0: 696d 6573 2c20 652e 672e 2027 6d61 6573  imes, e.g. 'maes
-000133c0: 7472 6f20 706c 6179 202d 6f20 3120 2d6f  tro play -o 1 -o
-000133d0: 2031 3727 292e 222c 0a29 0a40 636c 6963   17').",.).@clic
-000133e0: 6b2e 6f70 7469 6f6e 280a 2020 2020 222d  k.option(.    "-
-000133f0: 7622 2c0a 2020 2020 222d 2d76 6f6c 756d  v",.    "--volum
-00013400: 6522 2c0a 2020 2020 2276 6f6c 756d 6522  e",.    "volume"
-00013410: 2c0a 2020 2020 7479 7065 3d63 6c69 636b  ,.    type=click
-00013420: 2e49 6e74 5261 6e67 6528 302c 2031 3030  .IntRange(0, 100
-00013430: 292c 0a20 2020 2064 6566 6175 6c74 3d31  ),.    default=1
-00013440: 3030 2c0a 2020 2020 7368 6f77 5f64 6566  00,.    show_def
-00013450: 6175 6c74 3d54 7275 652c 0a29 0a40 636c  ault=True,.).@cl
-00013460: 6963 6b2e 6f70 7469 6f6e 280a 2020 2020  ick.option(.    
-00013470: 222d 4c2f 2d6e 4c22 2c0a 2020 2020 222d  "-L/-nL",.    "-
-00013480: 2d6c 6f6f 702f 2d2d 6e6f 2d6c 6f6f 7022  -loop/--no-loop"
-00013490: 2c0a 2020 2020 226c 6f6f 7022 2c0a 2020  ,.    "loop",.  
-000134a0: 2020 6465 6661 756c 743d 4661 6c73 652c    default=False,
-000134b0: 0a20 2020 2068 656c 703d 224c 6f6f 7020  .    help="Loop 
-000134c0: 7468 6520 706c 6179 6c69 7374 2e20 4361  the playlist. Ca
-000134d0: 6e20 6265 2074 6f67 676c 6564 2077 6974  n be toggled wit
-000134e0: 6820 276c 272e 222c 0a29 0a40 636c 6963  h 'l'.",.).@clic
-000134f0: 6b2e 6f70 7469 6f6e 280a 2020 2020 222d  k.option(.    "-
-00013500: 432f 2d6e 4322 2c0a 2020 2020 222d 2d63  C/-nC",.    "--c
-00013510: 6c69 7073 2f2d 2d6e 6f2d 636c 6970 7322  lips/--no-clips"
-00013520: 2c0a 2020 2020 2263 6c69 7073 222c 0a20  ,.    "clips",. 
-00013530: 2020 2064 6566 6175 6c74 3d46 616c 7365     default=False
-00013540: 2c0a 2020 2020 6865 6c70 3d22 5374 6172  ,.    help="Star
-00013550: 7420 696e 2063 6c69 7020 6d6f 6465 2e20  t in clip mode. 
-00013560: 4361 6e20 6265 2074 6f67 676c 6564 2077  Can be toggled w
-00013570: 6974 6820 2763 272e 222c 0a29 0a40 636c  ith 'c'.",.).@cl
-00013580: 6963 6b2e 6f70 7469 6f6e 280a 2020 2020  ick.option(.    
-00013590: 222d 442f 2d6e 4422 2c0a 2020 2020 222d  "-D/-nD",.    "-
-000135a0: 2d64 6973 636f 7264 2f2d 2d6e 6f2d 6469  -discord/--no-di
-000135b0: 7363 6f72 6422 2c0a 2020 2020 2264 6973  scord",.    "dis
-000135c0: 636f 7264 222c 0a20 2020 2064 6566 6175  cord",.    defau
-000135d0: 6c74 3d46 616c 7365 2c0a 2020 2020 6865  lt=False,.    he
-000135e0: 6c70 3d22 4469 7363 6f72 6420 7269 6368  lp="Discord rich
-000135f0: 2070 7265 7365 6e63 652e 2049 676e 6f72   presence. Ignor
-00013600: 6564 2069 6620 7265 7175 6972 6564 2064  ed if required d
-00013610: 6570 656e 6465 6e63 6965 7320 6172 6520  ependencies are 
-00013620: 6e6f 7420 696e 7374 616c 6c65 642e 2057  not installed. W
-00013630: 696c 6c20 6661 696c 2073 696c 656e 746c  ill fail silentl
-00013640: 7920 616e 6420 7265 7472 7920 6576 6572  y and retry ever
-00013650: 7920 7469 6d65 2074 6865 2073 6f6e 6720  y time the song 
-00013660: 6368 616e 6765 7320 6966 2044 6973 636f  changes if Disco
-00013670: 7264 2063 6f6e 6e65 6374 696f 6e20 6661  rd connection fa
-00013680: 696c 7320 2865 2e67 2e20 4469 7363 6f72  ils (e.g. Discor
-00013690: 6420 6e6f 7420 6f70 656e 292e 222c 0a29  d not open).",.)
-000136a0: 0a40 636c 6963 6b2e 6f70 7469 6f6e 280a  .@click.option(.
-000136b0: 2020 2020 222d 4d2f 2d6e 4d22 2c0a 2020      "-M/-nM",.  
-000136c0: 2020 222d 2d6d 6174 6368 2d61 6c6c 2f2d    "--match-all/-
-000136d0: 2d6e 6f2d 6d61 7463 682d 616c 6c22 2c0a  -no-match-all",.
-000136e0: 2020 2020 226d 6174 6368 5f61 6c6c 222c      "match_all",
-000136f0: 0a20 2020 2064 6566 6175 6c74 3d46 616c  .    default=Fal
-00013700: 7365 2c0a 2020 2020 6865 6c70 3d22 506c  se,.    help="Pl
-00013710: 6179 2073 6f6e 6773 2074 6861 7420 6d61  ay songs that ma
-00013720: 7463 6820 616c 6c20 7461 6773 2c20 6e6f  tch all tags, no
-00013730: 7420 616e 792e 222c 0a29 0a40 636c 6963  t any.",.).@clic
-00013740: 6b2e 6f70 7469 6f6e 280a 2020 2020 222d  k.option(.    "-
-00013750: 562f 2d6e 5622 2c0a 2020 2020 222d 2d76  V/-nV",.    "--v
-00013760: 6973 7561 6c69 7a65 2f2d 2d6e 6f2d 7669  isualize/--no-vi
-00013770: 7375 616c 697a 6522 2c0a 2020 2020 2276  sualize",.    "v
-00013780: 6973 7561 6c69 7a65 222c 0a20 2020 2064  isualize",.    d
-00013790: 6566 6175 6c74 3d46 616c 7365 2c0a 2020  efault=False,.  
-000137a0: 2020 6865 6c70 3d22 5669 7375 616c 697a    help="Visualiz
-000137b0: 6520 7468 6520 736f 6e67 2062 6569 6e67  e the song being
-000137c0: 2070 6c61 7965 642e 2049 676e 6f72 6564   played. Ignored
-000137d0: 2069 6620 7265 7175 6972 6564 2064 6570   if required dep
-000137e0: 656e 6465 6e63 6965 7320 6172 6520 6e6f  endencies are no
-000137f0: 7420 696e 7374 616c 6c65 642e 222c 0a29  t installed.",.)
-00013800: 0a64 6566 2070 6c61 7928 0a20 2020 2074  .def play(.    t
-00013810: 6167 732c 0a20 2020 2073 6875 6666 6c65  ags,.    shuffle
-00013820: 5f2c 0a20 2020 2072 6576 6572 7365 2c0a  _,.    reverse,.
-00013830: 2020 2020 6f6e 6c79 2c0a 2020 2020 766f      only,.    vo
-00013840: 6c75 6d65 2c0a 2020 2020 6c6f 6f70 2c0a  lume,.    loop,.
-00013850: 2020 2020 636c 6970 732c 0a20 2020 2064      clips,.    d
-00013860: 6973 636f 7264 2c0a 2020 2020 6d61 7463  iscord,.    matc
-00013870: 685f 616c 6c2c 0a20 2020 2076 6973 7561  h_all,.    visua
-00013880: 6c69 7a65 2c0a 293a 0a20 2020 2022 2222  lize,.):.    """
-00013890: 506c 6179 2079 6f75 7220 736f 6e67 732e  Play your songs.
-000138a0: 2049 6620 7461 6773 2061 7265 2070 6173   If tags are pas
-000138b0: 7365 642c 2061 6e79 2073 6f6e 6720 6d61  sed, any song ma
-000138c0: 7463 6869 6e67 2061 6e79 2074 6167 2077  tching any tag w
-000138d0: 696c 6c20 6265 2069 6e0a 2020 2020 796f  ill be in.    yo
-000138e0: 7572 2070 6c61 796c 6973 742c 2075 6e6c  ur playlist, unl
-000138f0: 6573 7320 7468 6520 272d 4d2f 2d2d 6d61  ess the '-M/--ma
-00013900: 7463 682d 616c 6c27 2066 6c61 6720 6973  tch-all' flag is
-00013910: 2070 6173 7365 642c 2069 6e20 7768 6963   passed, in whic
-00013920: 6820 6361 7365 0a20 2020 2065 7665 7279  h case.    every
-00013930: 2074 6167 206d 7573 7420 6265 206d 6174   tag must be mat
-00013940: 6368 6564 2e0a 0a20 2020 205c 620a 2020  ched...    \b.  
-00013950: 2020 5c78 3162 5b31 6d53 5041 4345 5c78    \x1b[1mSPACE\x
-00013960: 3162 5b30 6d20 2074 6f20 7061 7573 652f  1b[0m  to pause/
-00013970: 706c 6179 0a20 2020 205c 7831 625b 316d  play.    \x1b[1m
-00013980: 625c 7831 625b 306d 2020 746f 2067 6f20  b\x1b[0m  to go 
-00013990: 5b62 5d61 636b 2074 6f20 7072 6576 696f  [b]ack to previo
-000139a0: 7573 2073 6f6e 670a 2020 2020 5c78 3162  us song.    \x1b
-000139b0: 5b31 6d72 5c78 3162 5b30 6d20 2074 6f20  [1mr\x1b[0m  to 
-000139c0: 5b72 5d65 706c 6179 2073 6f6e 670a 2020  [r]eplay song.  
-000139d0: 2020 5c78 3162 5b31 6d6e 5c78 3162 5b30    \x1b[1mn\x1b[0
-000139e0: 6d20 2074 6f20 736b 6970 2074 6f20 5b6e  m  to skip to [n
-000139f0: 5d65 7874 2073 6f6e 670a 2020 2020 5c78  ]ext song.    \x
-00013a00: 3162 5b31 6d6c 5c78 3162 5b30 6d20 2074  1b[1ml\x1b[0m  t
-00013a10: 6f20 5b6c 5d6f 6f70 2074 6865 2063 7572  o [l]oop the cur
-00013a20: 7265 6e74 2073 6f6e 6720 6f6e 6365 2028  rent song once (
-00013a30: 276c 2720 696e 2073 7461 7475 7320 6261  'l' in status ba
-00013a40: 7229 2e20 7072 6573 7320 6167 6169 6e20  r). press again 
-00013a50: 746f 206c 6f6f 7020 696e 6669 6e69 7465  to loop infinite
-00013a60: 6c79 2028 274c 2720 696e 2073 7461 7475  ly ('L' in statu
-00013a70: 7320 6261 7229 2e20 7072 6573 7320 6f6e  s bar). press on
-00013a80: 6365 2061 6761 696e 2074 6f20 7475 726e  ce again to turn
-00013a90: 206f 6666 206c 6f6f 7069 6e67 0a20 2020   off looping.   
-00013aa0: 205c 7831 625b 316d 635c 7831 625b 306d   \x1b[1mc\x1b[0m
-00013ab0: 2020 746f 2074 6f67 676c 6520 5b63 5d6c    to toggle [c]l
-00013ac0: 6970 206d 6f64 650a 2020 2020 5c78 3162  ip mode.    \x1b
-00013ad0: 5b31 6d76 5c78 3162 5b30 6d20 2074 6f20  [1mv\x1b[0m  to 
-00013ae0: 746f 6767 6c65 205b 765d 6973 7561 6c69  toggle [v]isuali
-00013af0: 7a61 7469 6f6e 0a20 2020 205c 7831 625b  zation.    \x1b[
-00013b00: 316d 4c45 4654 5c78 3162 5b30 6d20 2074  1mLEFT\x1b[0m  t
-00013b10: 6f20 7265 7769 6e64 2035 730a 2020 2020  o rewind 5s.    
-00013b20: 5c78 3162 5b31 6d52 4947 4854 5c78 3162  \x1b[1mRIGHT\x1b
-00013b30: 5b30 6d20 2074 6f20 6661 7374 2066 6f72  [0m  to fast for
-00013b40: 7761 7264 2035 730a 2020 2020 5c78 3162  ward 5s.    \x1b
-00013b50: 5b31 6d5b 5c78 3162 5b30 6d20 2074 6f20  [1m[\x1b[0m  to 
-00013b60: 6465 6372 6561 7365 2076 6f6c 756d 650a  decrease volume.
-00013b70: 2020 2020 5c78 3162 5b31 6d5d 5c78 3162      \x1b[1m]\x1b
-00013b80: 5b30 6d20 2074 6f20 696e 6372 6561 7365  [0m  to increase
-00013b90: 2076 6f6c 756d 650a 2020 2020 5c78 3162   volume.    \x1b
-00013ba0: 5b31 6d6d 5c78 3162 5b30 6d20 2074 6f20  [1mm\x1b[0m  to 
-00013bb0: 5b6d 5d75 7465 2f75 6e6d 7574 650a 2020  [m]ute/unmute.  
-00013bc0: 2020 5c78 3162 5b31 6d65 5c78 3162 5b30    \x1b[1me\x1b[0
-00013bd0: 6d20 2074 6f20 5b65 5d6e 6420 7468 6520  m  to [e]nd the 
-00013be0: 736f 6e67 2070 6c61 7965 7220 6166 7465  song player afte
-00013bf0: 7220 7468 6520 6375 7272 656e 7420 736f  r the current so
-00013c00: 6e67 2066 696e 6973 6865 7320 2869 6e64  ng finishes (ind
-00013c10: 6963 6174 6f72 2069 6e20 7374 6174 7573  icator in status
-00013c20: 2062 6172 2c20 2765 2720 746f 2063 616e   bar, 'e' to can
-00013c30: 6365 6c29 0a20 2020 205c 7831 625b 316d  cel).    \x1b[1m
-00013c40: 715c 7831 625b 306d 2020 746f 205b 715d  q\x1b[0m  to [q]
-00013c50: 7569 7420 7468 6520 736f 6e67 2070 6c61  uit the song pla
-00013c60: 7965 7220 696d 6d65 6469 6174 656c 790a  yer immediately.
-00013c70: 2020 2020 5c78 3162 5b31 6d55 502f 444f      \x1b[1mUP/DO
-00013c80: 574e 5c78 3162 5b30 6d20 2074 6f20 7363  WN\x1b[0m  to sc
-00013c90: 726f 6c6c 2074 6872 6f75 6768 2074 6865  roll through the
-00013ca0: 2070 6c61 796c 6973 7420 286d 6f75 7365   playlist (mouse
-00013cb0: 2073 6372 6f6c 6c69 6e67 2073 686f 756c   scrolling shoul
-00013cc0: 6420 616c 736f 2077 6f72 6b29 0a20 2020  d also work).   
-00013cd0: 205c 7831 625b 316d 705c 7831 625b 306d   \x1b[1mp\x1b[0m
-00013ce0: 2020 746f 2073 6e61 5b70 5d20 6261 636b    to sna[p] back
-00013cf0: 2074 6f20 7468 6520 6375 7272 656e 746c   to the currentl
-00013d00: 7920 706c 6179 696e 6720 736f 6e67 0a20  y playing song. 
-00013d10: 2020 205c 7831 625b 316d 675c 7831 625b     \x1b[1mg\x1b[
-00013d20: 306d 2020 746f 2067 6f20 746f 2074 6865  0m  to go to the
-00013d30: 206e 6578 7420 7061 5b67 5d65 2f6c 6f6f   next pa[g]e/loo
-00013d40: 7020 6f66 2074 6865 2070 6c61 796c 6973  p of the playlis
-00013d50: 7420 2869 676e 6f72 6564 2069 6620 6e6f  t (ignored if no
-00013d60: 7420 7265 7065 6174 696e 6720 706c 6179  t repeating play
-00013d70: 6c69 7374 290a 2020 2020 5c78 3162 5b31  list).    \x1b[1
-00013d80: 6d42 4143 4b53 5041 4345 2f44 454c 4554  mBACKSPACE/DELET
-00013d90: 455c 7831 625b 306d 2020 6465 6c65 7465  E\x1b[0m  delete
-00013da0: 2074 6865 2073 656c 6563 7465 6420 286e   the selected (n
-00013db0: 6f74 206e 6563 6573 7361 7269 6c79 2063  ot necessarily c
-00013dc0: 7572 7265 6e74 6c79 2070 6c61 7969 6e67  urrently playing
-00013dd0: 2129 2073 6f6e 6720 6672 6f6d 2074 6865  !) song from the
-00013de0: 2071 7565 7565 0a20 2020 205c 7831 625b   queue.    \x1b[
-00013df0: 316d 645c 7831 625b 306d 2020 746f 2074  1md\x1b[0m  to t
-00013e00: 6f67 676c 6520 5b44 5d69 7363 6f72 6420  oggle [D]iscord 
-00013e10: 7269 6368 2070 7265 7365 6e63 650a 2020  rich presence.  
-00013e20: 2020 5c78 3162 5b31 6d61 5c78 3162 5b30    \x1b[1ma\x1b[0
-00013e30: 6d20 2074 6f20 6164 6420 6120 736f 6e67  m  to add a song
-00013e40: 2028 6279 2049 4429 2074 6f20 7468 6520   (by ID) to the 
-00013e50: 656e 6420 6f66 2074 6865 2070 6c61 796c  end of the playl
-00013e60: 6973 742e 204f 7065 6e73 2061 2070 726f  ist. Opens a pro
-00013e70: 6d70 7420 746f 2065 6e74 6572 2074 6865  mpt to enter the
-00013e80: 2049 443a 2045 4e54 4552 2074 6f20 636f   ID: ENTER to co
-00013e90: 6e66 6972 6d2c 2045 5343 2074 6f20 6361  nfirm, ESC to ca
-00013ea0: 6e63 656c 2e0a 2020 2020 5c78 3162 5b31  ncel..    \x1b[1
-00013eb0: 6d69 5c78 3162 5b30 6d20 2074 6f20 696e  mi\x1b[0m  to in
-00013ec0: 7365 7274 2061 2073 6f6e 6720 2862 7920  sert a song (by 
-00013ed0: 4944 2920 696e 2074 6865 2070 6c61 796c  ID) in the playl
-00013ee0: 6973 7420 6166 7465 7220 7468 6520 7365  ist after the se
-00013ef0: 6c65 6374 6564 2073 6f6e 672e 204f 7065  lected song. Ope
-00013f00: 6e73 2061 2070 726f 6d70 7420 6c69 6b65  ns a prompt like
-00013f10: 2027 6127 2e0a 2020 2020 5c78 3162 5b31   'a'..    \x1b[1
-00013f20: 6d74 5c78 3162 5b30 6d20 2074 6f20 6164  mt\x1b[0m  to ad
-00013f30: 6420 6120 7461 6720 746f 2061 6c6c 2073  d a tag to all s
-00013f40: 6f6e 6773 2069 6e20 7468 6520 706c 6179  ongs in the play
-00013f50: 6c69 7374 2e20 4f70 656e 7320 6120 7072  list. Opens a pr
-00013f60: 6f6d 7074 2074 6f20 656e 7465 7220 7468  ompt to enter th
-00013f70: 6520 7461 673a 2045 4e54 4552 2074 6f20  e tag: ENTER to 
-00013f80: 636f 6e66 6972 6d2c 2045 5343 2074 6f20  confirm, ESC to 
-00013f90: 6361 6e63 656c 2e0a 0a20 2020 205c 620a  cancel...    \b.
-00013fa0: 2020 2020 736f 6e67 2063 6f6c 6f72 2069      song color i
-00013fb0: 6e64 6963 6174 6573 206d 6f64 653a 0a20  ndicates mode:. 
-00013fc0: 2020 2020 2020 205c 7831 625b 313b 3334         \x1b[1;34
-00013fd0: 6d62 6c75 655c 7831 625b 306d 2020 2020  mblue\x1b[0m    
-00013fe0: 206e 6f72 6d61 6c0a 2020 2020 2020 2020   normal.        
-00013ff0: 5c78 3162 5b31 3b33 336d 7965 6c6c 6f77  \x1b[1;33myellow
-00014000: 5c78 3162 5b30 6d20 2020 6c6f 6f70 696e  \x1b[0m   loopin
-00014010: 6720 6375 7272 656e 7420 736f 6e67 2028  g current song (
-00014020: 6f6e 6365 206f 7220 7265 7065 6174 6564  once or repeated
-00014030: 6c79 290a 0a20 2020 205c 620a 2020 2020  ly)..    \b.    
-00014040: 7072 6f67 7265 7373 2062 6172 2063 6f6c  progress bar col
-00014050: 6f72 2069 6e64 6963 6174 6573 2073 7461  or indicates sta
-00014060: 7475 733a 0a20 2020 2020 2020 205c 7831  tus:.        \x1
-00014070: 625b 313b 3333 6d79 656c 6c6f 775c 7831  b[1;33myellow\x1
-00014080: 625b 306d 2020 206e 6f72 6d61 6c20 286f  b[0m   normal (o
-00014090: 7220 6375 7272 656e 7420 736f 6e67 2064  r current song d
-000140a0: 6f65 736e 2774 2068 6176 6520 6120 636c  oesn't have a cl
-000140b0: 6970 290a 2020 2020 2020 2020 5c78 3162  ip).        \x1b
-000140c0: 5b31 3b33 356d 6d61 6765 6e74 615c 7831  [1;35mmagenta\x1
-000140d0: 625b 306d 2020 706c 6179 696e 6720 636c  b[0m  playing cl
-000140e0: 6970 0a0a 2020 2020 466f 7220 7468 6520  ip..    For the 
-000140f0: 636f 6c6f 7220 7669 7369 6f6e 2064 6566  color vision def
-00014100: 6963 6965 6e74 2c20 626f 7468 206d 6f64  icient, both mod
-00014110: 6573 2061 6c73 6f20 6861 7665 2069 6e64  es also have ind
-00014120: 6963 6174 6f72 7320 696e 2074 6865 2073  icators in the s
-00014130: 7461 7475 7320 6261 722e 0a20 2020 2022  tatus bar..    "
-00014140: 2222 0a20 2020 2070 6c61 796c 6973 7420  "".    playlist 
-00014150: 3d20 5b5d 0a0a 2020 2020 6966 206f 6e6c  = []..    if onl
-00014160: 793a 0a20 2020 2020 2020 206f 6e6c 7920  y:.        only 
-00014170: 3d20 7365 7428 6f6e 6c79 290a 2020 2020  = set(only).    
-00014180: 2020 2020 7769 7468 206f 7065 6e28 534f      with open(SO
-00014190: 4e47 535f 494e 464f 5f50 4154 482c 2022  NGS_INFO_PATH, "
-000141a0: 7222 2c20 656e 636f 6469 6e67 3d22 7574  r", encoding="ut
-000141b0: 662d 3822 2920 6173 2073 6f6e 6773 5f66  f-8") as songs_f
-000141c0: 696c 653a 0a20 2020 2020 2020 2020 2020  ile:.           
-000141d0: 2066 6f72 206c 696e 6520 696e 2073 6f6e   for line in son
-000141e0: 6773 5f66 696c 653a 0a20 2020 2020 2020  gs_file:.       
-000141f0: 2020 2020 2020 2020 2064 6574 6169 6c73           details
-00014200: 203d 206c 696e 652e 7374 7269 7028 292e   = line.strip().
-00014210: 7370 6c69 7428 227c 2229 0a20 2020 2020  split("|").     
-00014220: 2020 2020 2020 2020 2020 2073 6f6e 675f             song_
-00014230: 6964 203d 2069 6e74 2864 6574 6169 6c73  id = int(details
-00014240: 5b30 5d29 0a20 2020 2020 2020 2020 2020  [0]).           
-00014250: 2020 2020 2069 6620 736f 6e67 5f69 6420       if song_id 
-00014260: 696e 206f 6e6c 793a 0a20 2020 2020 2020  in only:.       
-00014270: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
-00014280: 796c 6973 742e 6170 7065 6e64 2864 6574  ylist.append(det
-00014290: 6169 6c73 290a 0a20 2020 2020 2020 2069  ails)..        i
-000142a0: 6620 6e6f 7420 706c 6179 6c69 7374 3a0a  f not playlist:.
-000142b0: 2020 2020 2020 2020 2020 2020 636c 6963              clic
-000142c0: 6b2e 7365 6368 6f28 224e 6f20 736f 6e67  k.secho("No song
-000142d0: 7320 666f 756e 6420 7769 7468 2074 6865  s found with the
-000142e0: 2067 6976 656e 2049 4473 2e22 2c20 6667   given IDs.", fg
-000142f0: 3d22 7265 6422 290a 2020 2020 2020 2020  ="red").        
-00014300: 2020 2020 7265 7475 726e 0a20 2020 2065      return.    e
-00014310: 6c73 653a 0a20 2020 2020 2020 2069 6620  lse:.        if 
-00014320: 6e6f 7420 7461 6773 3a0a 2020 2020 2020  not tags:.      
-00014330: 2020 2020 2020 7769 7468 206f 7065 6e28        with open(
-00014340: 534f 4e47 535f 494e 464f 5f50 4154 482c  SONGS_INFO_PATH,
-00014350: 2022 7222 2c20 656e 636f 6469 6e67 3d22   "r", encoding="
-00014360: 7574 662d 3822 2920 6173 2073 6f6e 6773  utf-8") as songs
-00014370: 5f66 696c 653a 0a20 2020 2020 2020 2020  _file:.         
-00014380: 2020 2020 2020 2066 6f72 206c 696e 6520         for line 
-00014390: 696e 2073 6f6e 6773 5f66 696c 653a 0a20  in songs_file:. 
-000143a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000143b0: 2020 2064 6574 6169 6c73 203d 206c 696e     details = lin
-000143c0: 652e 7374 7269 7028 292e 7370 6c69 7428  e.strip().split(
-000143d0: 227c 2229 0a20 2020 2020 2020 2020 2020  "|").           
-000143e0: 2020 2020 2020 2020 2070 6c61 796c 6973           playlis
-000143f0: 742e 6170 7065 6e64 2864 6574 6169 6c73  t.append(details
-00014400: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-00014410: 2020 2020 2020 2020 2020 2020 7461 6773              tags
-00014420: 203d 2073 6574 2874 6167 7329 0a20 2020   = set(tags).   
-00014430: 2020 2020 2020 2020 2077 6974 6820 6f70           with op
-00014440: 656e 2853 4f4e 4753 5f49 4e46 4f5f 5041  en(SONGS_INFO_PA
-00014450: 5448 2c20 2272 222c 2065 6e63 6f64 696e  TH, "r", encodin
-00014460: 673d 2275 7466 2d38 2229 2061 7320 736f  g="utf-8") as so
-00014470: 6e67 735f 6669 6c65 3a0a 2020 2020 2020  ngs_file:.      
-00014480: 2020 2020 2020 2020 2020 666f 7220 6c69            for li
-00014490: 6e65 2069 6e20 736f 6e67 735f 6669 6c65  ne in songs_file
-000144a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000144b0: 2020 2020 2020 6465 7461 696c 7320 3d20        details = 
-000144c0: 6c69 6e65 2e73 7472 6970 2829 2e73 706c  line.strip().spl
-000144d0: 6974 2822 7c22 290a 2020 2020 2020 2020  it("|").        
-000144e0: 2020 2020 2020 2020 2020 2020 736f 6e67              song
-000144f0: 5f74 6167 7320 3d20 7365 7428 6465 7461  _tags = set(deta
-00014500: 696c 735b 325d 2e73 706c 6974 2822 2c22  ils[2].split(","
-00014510: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-00014520: 2020 2020 2020 2069 6620 6e6f 7420 6d61         if not ma
-00014530: 7463 685f 616c 6c3a 0a20 2020 2020 2020  tch_all:.       
-00014540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014550: 2069 6620 7461 6773 2026 2073 6f6e 675f   if tags & song_
-00014560: 7461 6773 3a20 2023 2069 6e74 6572 7365  tags:  # interse
-00014570: 6374 696f 6e0a 2020 2020 2020 2020 2020  ction.          
-00014580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014590: 2020 706c 6179 6c69 7374 2e61 7070 656e    playlist.appen
-000145a0: 6428 6465 7461 696c 7329 0a20 2020 2020  d(details).     
-000145b0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-000145c0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-000145d0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000145e0: 7461 6773 203c 3d20 736f 6e67 5f74 6167  tags <= song_tag
-000145f0: 733a 2020 2320 7375 6273 6574 0a20 2020  s:  # subset.   
-00014600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014610: 2020 2020 2020 2020 2070 6c61 796c 6973           playlis
-00014620: 742e 6170 7065 6e64 2864 6574 6169 6c73  t.append(details
-00014630: 290a 0a20 2020 2066 6f72 2064 6574 6169  )..    for detai
-00014640: 6c73 2069 6e20 706c 6179 6c69 7374 3a0a  ls in playlist:.
-00014650: 2020 2020 2020 2020 736f 6e67 5f64 6174          song_dat
-00014660: 6120 3d20 6d75 7369 635f 7461 672e 6c6f  a = music_tag.lo
-00014670: 6164 5f66 696c 6528 6f73 2e70 6174 682e  ad_file(os.path.
-00014680: 6a6f 696e 2853 4f4e 4753 5f44 4952 2c20  join(SONGS_DIR, 
-00014690: 6465 7461 696c 735b 315d 2929 0a20 2020  details[1])).   
-000146a0: 2020 2020 2064 6574 6169 6c73 202b 3d20       details += 
-000146b0: 5b0a 2020 2020 2020 2020 2020 2020 2873  [.            (s
-000146c0: 6f6e 675f 6461 7461 5b22 6172 7469 7374  ong_data["artist
-000146d0: 225d 2e76 616c 7565 206f 7220 2255 6e6b  "].value or "Unk
-000146e0: 6e6f 776e 2041 7274 6973 7422 292c 0a20  nown Artist"),. 
-000146f0: 2020 2020 2020 2020 2020 2028 736f 6e67             (song
-00014700: 5f64 6174 615b 2261 6c62 756d 225d 2e76  _data["album"].v
-00014710: 616c 7565 206f 7220 2255 6e6b 6e6f 776e  alue or "Unknown
-00014720: 2041 6c62 756d 2229 2c0a 2020 2020 2020   Album"),.      
-00014730: 2020 2020 2020 2873 6f6e 675f 6461 7461        (song_data
-00014740: 5b22 616c 6275 6d61 7274 6973 7422 5d2e  ["albumartist"].
-00014750: 7661 6c75 6520 6f72 2022 556e 6b6e 6f77  value or "Unknow
-00014760: 6e20 416c 6275 6d20 4172 7469 7374 2229  n Album Artist")
-00014770: 2c0a 2020 2020 2020 2020 5d0a 0a20 2020  ,.        ]..   
-00014780: 2069 6620 7368 7566 666c 655f 203d 3d20   if shuffle_ == 
-00014790: 303a 0a20 2020 2020 2020 2073 6875 6666  0:.        shuff
-000147a0: 6c65 5f20 3d20 5472 7565 0a20 2020 2020  le_ = True.     
-000147b0: 2020 2072 6573 6875 6666 6c65 203d 2046     reshuffle = F
-000147c0: 616c 7365 0a20 2020 2065 6c69 6620 7368  alse.    elif sh
-000147d0: 7566 666c 655f 203d 3d20 313a 0a20 2020  uffle_ == 1:.   
-000147e0: 2020 2020 2073 6875 6666 6c65 5f20 3d20       shuffle_ = 
-000147f0: 5472 7565 0a20 2020 2020 2020 2072 6573  True.        res
-00014800: 6875 6666 6c65 203d 2054 7275 650a 2020  huffle = True.  
-00014810: 2020 656c 6966 2073 6875 6666 6c65 5f20    elif shuffle_ 
-00014820: 3d3d 2032 3a0a 2020 2020 2020 2020 7368  == 2:.        sh
-00014830: 7566 666c 655f 203d 2046 616c 7365 0a20  uffle_ = False. 
-00014840: 2020 2020 2020 2072 6573 6875 6666 6c65         reshuffle
-00014850: 203d 2054 7275 650a 2020 2020 656c 7365   = True.    else
-00014860: 3a20 2023 2073 6875 6666 6c65 5f20 3d20  :  # shuffle_ = 
-00014870: 4e6f 6e65 0a20 2020 2020 2020 2073 6875  None.        shu
-00014880: 6666 6c65 5f20 3d20 4661 6c73 650a 2020  ffle_ = False.  
-00014890: 2020 2020 2020 7265 7368 7566 666c 6520        reshuffle 
-000148a0: 3d20 4661 6c73 650a 0a20 2020 2069 6620  = False..    if 
-000148b0: 7368 7566 666c 655f 3a0a 2020 2020 2020  shuffle_:.      
-000148c0: 2020 7368 7566 666c 6528 706c 6179 6c69    shuffle(playli
-000148d0: 7374 290a 2020 2020 656c 6966 2072 6576  st).    elif rev
-000148e0: 6572 7365 3a0a 2020 2020 2020 2020 706c  erse:.        pl
-000148f0: 6179 6c69 7374 2e72 6576 6572 7365 2829  aylist.reverse()
-00014900: 0a0a 2020 2020 6966 206e 6f74 2070 6c61  ..    if not pla
-00014910: 796c 6973 743a 0a20 2020 2020 2020 2063  ylist:.        c
-00014920: 6c69 636b 2e73 6563 686f 2822 4e6f 2073  lick.secho("No s
-00014930: 6f6e 6773 2066 6f75 6e64 206d 6174 6368  ongs found match
-00014940: 696e 6720 7461 6720 6372 6974 6572 6961  ing tag criteria
-00014950: 2e22 2c20 6667 3d22 7265 6422 290a 2020  .", fg="red").  
-00014960: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00014970: 766f 6c75 6d65 202f 3d20 3130 300a 2020  volume /= 100.  
-00014980: 2020 2020 2020 6375 7273 6573 2e77 7261        curses.wra
-00014990: 7070 6572 280a 2020 2020 2020 2020 2020  pper(.          
-000149a0: 2020 5f70 6c61 792c 0a20 2020 2020 2020    _play,.       
-000149b0: 2020 2020 2070 6c61 796c 6973 742c 0a20       playlist,. 
-000149c0: 2020 2020 2020 2020 2020 2076 6f6c 756d             volum
-000149d0: 652c 0a20 2020 2020 2020 2020 2020 206c  e,.            l
-000149e0: 6f6f 702c 0a20 2020 2020 2020 2020 2020  oop,.           
-000149f0: 2063 6c69 7073 2c0a 2020 2020 2020 2020   clips,.        
-00014a00: 2020 2020 7265 7368 7566 666c 652c 0a20      reshuffle,. 
-00014a10: 2020 2020 2020 2020 2020 2064 6973 636f             disco
-00014a20: 7264 2061 6e64 2063 616e 5f75 7064 6174  rd and can_updat
-00014a30: 655f 6469 7363 6f72 642c 0a20 2020 2020  e_discord,.     
-00014a40: 2020 2020 2020 2076 6973 7561 6c69 7a65         visualize
-00014a50: 2c0a 2020 2020 2020 2020 290a 0a0a 4063  ,.        )...@c
-00014a60: 6c69 2e63 6f6d 6d61 6e64 2829 0a40 636c  li.command().@cl
-00014a70: 6963 6b2e 6f70 7469 6f6e 280a 2020 2020  ick.option(.    
-00014a80: 222d 542f 2d6e 5422 2c0a 2020 2020 222d  "-T/-nT",.    "-
-00014a90: 2d74 6167 2f2d 2d6e 6f2d 7461 6722 2c0a  -tag/--no-tag",.
-00014aa0: 2020 2020 2272 656e 616d 696e 675f 7461      "renaming_ta
-00014ab0: 6722 2c0a 2020 2020 6465 6661 756c 743d  g",.    default=
-00014ac0: 4661 6c73 652c 0a20 2020 2068 656c 703d  False,.    help=
-00014ad0: 2249 6620 7061 7373 6564 2c20 7265 6e61  "If passed, rena
-00014ae0: 6d65 2074 6167 2069 6e73 7465 6164 206f  me tag instead o
-00014af0: 6620 736f 6e67 2028 7472 6561 7420 7468  f song (treat th
-00014b00: 6520 6172 6775 6d65 6e74 7320 6173 2074  e arguments as t
-00014b10: 6167 7329 2e22 2c0a 290a 4063 6c69 636b  ags).",.).@click
-00014b20: 2e61 7267 756d 656e 7428 226f 7269 6769  .argument("origi
-00014b30: 6e61 6c22 290a 4063 6c69 636b 2e61 7267  nal").@click.arg
-00014b40: 756d 656e 7428 226e 6577 5f6e 616d 6522  ument("new_name"
-00014b50: 290a 6465 6620 7265 6e61 6d65 286f 7269  ).def rename(ori
-00014b60: 6769 6e61 6c2c 206e 6577 5f6e 616d 652c  ginal, new_name,
-00014b70: 2072 656e 616d 696e 675f 7461 6729 3a0a   renaming_tag):.
-00014b80: 2020 2020 2222 220a 2020 2020 5265 6e61      """.    Rena
-00014b90: 6d65 2061 2073 6f6e 672e 0a0a 2020 2020  me a song...    
-00014ba0: 5265 6e61 6d65 7320 7468 6520 736f 6e67  Renames the song
-00014bb0: 2077 6974 6820 7468 6520 4944 204f 5249   with the ID ORI
-00014bc0: 4749 4e41 4c20 746f 204e 4557 5f4e 414d  GINAL to NEW_NAM
-00014bd0: 452e 2054 6865 2065 7874 656e 7369 6f6e  E. The extension
-00014be0: 206f 6620 7468 650a 2020 2020 736f 6e67   of the.    song
-00014bf0: 2028 652e 672e 2027 2e77 6176 272c 2027   (e.g. '.wav', '
-00014c00: 2e6d 7033 2729 2069 7320 7072 6573 6572  .mp3') is preser
-00014c10: 7665 64e2 8094 646f 206e 6f74 2069 6e63  ved...do not inc
-00014c20: 6c75 6465 2069 7420 696e 2074 6865 206e  lude it in the n
-00014c30: 616d 652e 0a0a 2020 2020 4966 2074 6865  ame...    If the
-00014c40: 2027 2d54 2f2d 2d74 6167 2720 666c 6167   '-T/--tag' flag
-00014c50: 2069 7320 7061 7373 6564 2c20 7472 6561   is passed, trea
-00014c60: 7473 204f 5249 4749 4e41 4c20 6173 2061  ts ORIGINAL as a
-00014c70: 2074 6167 2c20 7265 6e61 6d69 6e67 2061   tag, renaming a
-00014c80: 6c6c 0a20 2020 206f 6375 7272 656e 6365  ll.    ocurrence
-00014c90: 7320 6f66 2069 7420 746f 204e 4557 5f4e  s of it to NEW_N
-00014ca0: 414d 45e2 8094 646f 6573 6e27 7420 6368  AME...doesn't ch
-00014cb0: 6563 6b20 6966 2074 6865 2074 6167 204e  eck if the tag N
-00014cc0: 4557 5f4e 414d 4520 616c 7265 6164 792c  EW_NAME already,
-00014cd0: 0a20 2020 2065 7869 7374 732c 2073 6f20  .    exists, so 
-00014ce0: 6265 2063 6172 6566 756c 210a 2020 2020  be careful!.    
-00014cf0: 2222 220a 2020 2020 736f 6e67 735f 6669  """.    songs_fi
-00014d00: 6c65 203d 206f 7065 6e28 534f 4e47 535f  le = open(SONGS_
-00014d10: 494e 464f 5f50 4154 482c 2022 7222 2c20  INFO_PATH, "r", 
-00014d20: 656e 636f 6469 6e67 3d22 7574 662d 3822  encoding="utf-8"
-00014d30: 290a 2020 2020 6c69 6e65 7320 3d20 736f  ).    lines = so
-00014d40: 6e67 735f 6669 6c65 2e72 6561 6428 292e  ngs_file.read().
-00014d50: 7370 6c69 746c 696e 6573 2829 0a20 2020  splitlines().   
-00014d60: 2069 6620 6e6f 7420 7265 6e61 6d69 6e67   if not renaming
-00014d70: 5f74 6167 3a0a 2020 2020 2020 2020 6966  _tag:.        if
-00014d80: 206e 6f74 206f 7269 6769 6e61 6c2e 6973   not original.is
-00014d90: 6e75 6d65 7269 6328 293a 0a20 2020 2020  numeric():.     
-00014da0: 2020 2020 2020 2063 6c69 636b 2e73 6563         click.sec
-00014db0: 686f 280a 2020 2020 2020 2020 2020 2020  ho(.            
-00014dc0: 2020 2020 2253 6f6e 6720 4944 206d 7573      "Song ID mus
-00014dd0: 7420 6265 2061 6e20 696e 7465 6765 722e  t be an integer.
-00014de0: 2054 6f20 7265 6e61 6d65 2061 2074 6167   To rename a tag
-00014df0: 2c20 7061 7373 2074 6865 2027 2d54 2f2d  , pass the '-T/-
-00014e00: 2d74 6167 2720 666c 6167 2e22 2c0a 2020  -tag' flag.",.  
-00014e10: 2020 2020 2020 2020 2020 2020 2020 6667                fg
-00014e20: 3d22 7265 6422 2c0a 2020 2020 2020 2020  ="red",.        
-00014e30: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00014e40: 2020 7265 7475 726e 0a0a 2020 2020 2020    return..      
-00014e50: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-00014e60: 286c 656e 286c 696e 6573 2929 3a0a 2020  (len(lines)):.  
-00014e70: 2020 2020 2020 2020 2020 6465 7461 696c            detail
-00014e80: 7320 3d20 6c69 6e65 735b 695d 2e73 7472  s = lines[i].str
-00014e90: 6970 2829 2e73 706c 6974 2822 7c22 290a  ip().split("|").
-00014ea0: 2020 2020 2020 2020 2020 2020 6966 206f              if o
-00014eb0: 732e 7061 7468 2e73 706c 6974 6578 7428  s.path.splitext(
-00014ec0: 6465 7461 696c 735b 315d 295b 305d 203d  details[1])[0] =
-00014ed0: 3d20 6e65 775f 6e61 6d65 3a0a 2020 2020  = new_name:.    
-00014ee0: 2020 2020 2020 2020 2020 2020 636c 6963              clic
-00014ef0: 6b2e 7365 6368 6f28 0a20 2020 2020 2020  k.secho(.       
-00014f00: 2020 2020 2020 2020 2020 2020 2066 2241               f"A
-00014f10: 2073 6f6e 6720 7769 7468 2074 6865 206e   song with the n
-00014f20: 616d 6520 277b 6e65 775f 6e61 6d65 7d27  ame '{new_name}'
-00014f30: 2061 6c72 6561 6479 2065 7869 7374 732e   already exists.
-00014f40: 2050 6c65 6173 6520 6368 6f6f 7365 2061   Please choose a
-00014f50: 6e6f 7468 6572 206e 616d 652e 222c 0a20  nother name.",. 
-00014f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014f70: 2020 2066 673d 2272 6564 222c 0a20 2020     fg="red",.   
-00014f80: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-00014f90: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00014fa0: 6574 7572 6e0a 0a20 2020 2020 2020 206f  eturn..        o
-00014fb0: 7269 6769 6e61 6c20 3d20 696e 7428 6f72  riginal = int(or
-00014fc0: 6967 696e 616c 290a 2020 2020 2020 2020  iginal).        
-00014fd0: 666f 7220 6920 696e 2072 616e 6765 286c  for i in range(l
-00014fe0: 656e 286c 696e 6573 2929 3a0a 2020 2020  en(lines)):.    
-00014ff0: 2020 2020 2020 2020 6465 7461 696c 7320          details 
-00015000: 3d20 6c69 6e65 735b 695d 2e73 7472 6970  = lines[i].strip
-00015010: 2829 2e73 706c 6974 2822 7c22 290a 2020  ().split("|").  
-00015020: 2020 2020 2020 2020 2020 6966 2069 6e74            if int
-00015030: 2864 6574 6169 6c73 5b30 5d29 203d 3d20  (details[0]) == 
-00015040: 6f72 6967 696e 616c 3a0a 2020 2020 2020  original:.      
-00015050: 2020 2020 2020 2020 2020 6f6c 645f 7061            old_pa
-00015060: 7468 203d 2064 6574 6169 6c73 5b31 5d0a  th = details[1].
-00015070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015080: 6465 7461 696c 735b 315d 203d 206e 6577  details[1] = new
-00015090: 5f6e 616d 6520 2b20 6f73 2e70 6174 682e  _name + os.path.
-000150a0: 7370 6c69 7465 7874 286f 6c64 5f70 6174  splitext(old_pat
-000150b0: 6829 5b31 5d0a 0a20 2020 2020 2020 2020  h)[1]..         
-000150c0: 2020 2020 2020 206c 696e 6573 5b69 5d20         lines[i] 
-000150d0: 3d20 227c 222e 6a6f 696e 2864 6574 6169  = "|".join(detai
-000150e0: 6c73 290a 2020 2020 2020 2020 2020 2020  ls).            
-000150f0: 2020 2020 736f 6e67 735f 6669 6c65 2e63      songs_file.c
-00015100: 6c6f 7365 2829 0a20 2020 2020 2020 2020  lose().         
-00015110: 2020 2020 2020 2073 6f6e 6773 5f66 696c         songs_fil
-00015120: 6520 3d20 6f70 656e 2853 4f4e 4753 5f49  e = open(SONGS_I
-00015130: 4e46 4f5f 5041 5448 2c20 2277 222c 2065  NFO_PATH, "w", e
-00015140: 6e63 6f64 696e 673d 2275 7466 2d38 2229  ncoding="utf-8")
-00015150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015160: 2073 6f6e 6773 5f66 696c 652e 7772 6974   songs_file.writ
-00015170: 6528 225c 6e22 2e6a 6f69 6e28 6c69 6e65  e("\n".join(line
-00015180: 7329 290a 0a20 2020 2020 2020 2020 2020  s))..           
-00015190: 2020 2020 206f 732e 7265 6e61 6d65 280a       os.rename(.
-000151a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000151b0: 2020 2020 6f73 2e70 6174 682e 6a6f 696e      os.path.join
-000151c0: 2853 4f4e 4753 5f44 4952 2c20 6f6c 645f  (SONGS_DIR, old_
-000151d0: 7061 7468 292c 0a20 2020 2020 2020 2020  path),.         
-000151e0: 2020 2020 2020 2020 2020 206f 732e 7061             os.pa
-000151f0: 7468 2e6a 6f69 6e28 534f 4e47 535f 4449  th.join(SONGS_DI
-00015200: 522c 2064 6574 6169 6c73 5b31 5d29 2c0a  R, details[1]),.
-00015210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015220: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
-00015230: 2020 2063 6c69 636b 2e73 6563 686f 280a     click.secho(.
-00015240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015250: 2020 2020 6622 5265 6e61 6d65 6420 736f      f"Renamed so
-00015260: 6e67 2027 7b6f 6c64 5f70 6174 687d 2720  ng '{old_path}' 
-00015270: 7769 7468 2049 4420 7b6f 7269 6769 6e61  with ID {origina
-00015280: 6c7d 2074 6f20 277b 6465 7461 696c 735b  l} to '{details[
-00015290: 315d 7d27 2e22 2c0a 2020 2020 2020 2020  1]}'.",.        
-000152a0: 2020 2020 2020 2020 2020 2020 6667 3d22              fg="
-000152b0: 6772 6565 6e22 2c0a 2020 2020 2020 2020  green",.        
-000152c0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-000152d0: 2020 2020 2020 2020 2020 2062 7265 616b             break
-000152e0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-000152f0: 2020 2020 2020 2020 2020 2063 6c69 636b             click
-00015300: 2e73 6563 686f 2866 2253 6f6e 6720 7769  .secho(f"Song wi
-00015310: 7468 2049 4420 7b6f 7269 6769 6e61 6c7d  th ID {original}
-00015320: 206e 6f74 2066 6f75 6e64 2e22 2c20 6667   not found.", fg
-00015330: 3d22 7265 6422 290a 2020 2020 2020 2020  ="red").        
-00015340: 2020 2020 736f 6e67 735f 6669 6c65 2e63      songs_file.c
-00015350: 6c6f 7365 2829 0a20 2020 2065 6c73 653a  lose().    else:
-00015360: 0a20 2020 2020 2020 2066 6f72 2069 2069  .        for i i
-00015370: 6e20 7261 6e67 6528 6c65 6e28 6c69 6e65  n range(len(line
-00015380: 7329 293a 0a20 2020 2020 2020 2020 2020  s)):.           
-00015390: 2064 6574 6169 6c73 203d 206c 696e 6573   details = lines
-000153a0: 5b69 5d2e 7374 7269 7028 292e 7370 6c69  [i].strip().spli
-000153b0: 7428 227c 2229 0a20 2020 2020 2020 2020  t("|").         
-000153c0: 2020 2074 6167 7320 3d20 6465 7461 696c     tags = detail
-000153d0: 735b 325d 2e73 706c 6974 2822 2c22 290a  s[2].split(",").
-000153e0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000153f0: 7420 696e 2072 616e 6765 286c 656e 2874  t in range(len(t
-00015400: 6167 7329 293a 0a20 2020 2020 2020 2020  ags)):.         
-00015410: 2020 2020 2020 2069 6620 7461 6773 5b74         if tags[t
-00015420: 5d20 3d3d 206f 7269 6769 6e61 6c3a 0a20  ] == original:. 
-00015430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015440: 2020 2074 6167 735b 745d 203d 206e 6577     tags[t] = new
-00015450: 5f6e 616d 650a 2020 2020 2020 2020 2020  _name.          
-00015460: 2020 2020 2020 2020 2020 6465 7461 696c            detail
-00015470: 735b 325d 203d 2022 2c22 2e6a 6f69 6e28  s[2] = ",".join(
-00015480: 7461 6773 290a 0a20 2020 2020 2020 2020  tags)..         
-00015490: 2020 2020 2020 2020 2020 206c 696e 6573             lines
-000154a0: 5b69 5d20 3d20 227c 222e 6a6f 696e 2864  [i] = "|".join(d
-000154b0: 6574 6169 6c73 290a 2020 2020 2020 2020  etails).        
-000154c0: 2020 2020 2020 2020 2020 2020 6272 6561              brea
-000154d0: 6b0a 0a20 2020 2020 2020 2073 6f6e 6773  k..        songs
-000154e0: 5f66 696c 652e 636c 6f73 6528 290a 2020  _file.close().  
-000154f0: 2020 2020 2020 736f 6e67 735f 6669 6c65        songs_file
-00015500: 203d 206f 7065 6e28 534f 4e47 535f 494e   = open(SONGS_IN
-00015510: 464f 5f50 4154 482c 2022 7722 2c20 656e  FO_PATH, "w", en
-00015520: 636f 6469 6e67 3d22 7574 662d 3822 290a  coding="utf-8").
-00015530: 2020 2020 2020 2020 736f 6e67 735f 6669          songs_fi
-00015540: 6c65 2e77 7269 7465 2822 5c6e 222e 6a6f  le.write("\n".jo
-00015550: 696e 286c 696e 6573 2929 0a0a 2020 2020  in(lines))..    
-00015560: 2020 2020 636c 6963 6b2e 7365 6368 6f28      click.secho(
-00015570: 0a20 2020 2020 2020 2020 2020 2066 2252  .            f"R
-00015580: 6570 6c61 6365 6420 616c 6c20 6f63 7572  eplaced all ocur
-00015590: 7265 6e63 6573 206f 6620 7461 6720 277b  rences of tag '{
-000155a0: 6f72 6967 696e 616c 7d27 2074 6f20 277b  original}' to '{
-000155b0: 6e65 775f 6e61 6d65 7d27 2e22 2c0a 2020  new_name}'.",.  
-000155c0: 2020 2020 2020 2020 2020 6667 3d22 6772            fg="gr
-000155d0: 6565 6e22 2c0a 2020 2020 2020 2020 290a  een",.        ).
-000155e0: 0a0a 4063 6c69 2e63 6f6d 6d61 6e64 2829  ..@cli.command()
-000155f0: 0a40 636c 6963 6b2e 6172 6775 6d65 6e74  .@click.argument
-00015600: 2822 7068 7261 7365 2229 0a40 636c 6963  ("phrase").@clic
-00015610: 6b2e 6f70 7469 6f6e 280a 2020 2020 222d  k.option(.    "-
-00015620: 542f 2d6e 5422 2c0a 2020 2020 222d 2d74  T/-nT",.    "--t
-00015630: 6167 2f2d 2d6e 6f2d 7461 6722 2c0a 2020  ag/--no-tag",.  
-00015640: 2020 2273 6561 7263 6869 6e67 5f66 6f72    "searching_for
-00015650: 5f74 6167 7322 2c0a 2020 2020 6465 6661  _tags",.    defa
-00015660: 756c 743d 4661 6c73 652c 0a20 2020 2068  ult=False,.    h
-00015670: 656c 703d 2253 6561 7263 6865 7320 666f  elp="Searches fo
-00015680: 7220 6d61 7463 6869 6e67 2074 6167 7320  r matching tags 
-00015690: 696e 7374 6561 6420 6f66 2073 6f6e 6720  instead of song 
-000156a0: 6e61 6d65 732e 222c 0a29 0a64 6566 2073  names.",.).def s
-000156b0: 6561 7263 6828 7068 7261 7365 2c20 7365  earch(phrase, se
-000156c0: 6172 6368 696e 675f 666f 725f 7461 6773  arching_for_tags
-000156d0: 293a 0a20 2020 2022 2222 5365 6172 6368  ):.    """Search
-000156e0: 6573 2066 6f72 2073 6f6e 6773 2074 6861  es for songs tha
-000156f0: 7420 636f 6e74 6169 6e20 5048 5241 5345  t contain PHRASE
-00015700: 2e20 416c 6c20 736f 6e67 7320 7374 6172  . All songs star
-00015710: 7469 6e67 2077 6974 6820 5048 5241 5345  ting with PHRASE
-00015720: 0a20 2020 2077 696c 6c20 6170 7065 6172  .    will appear
-00015730: 2062 6566 6f72 6520 736f 6e67 7320 636f   before songs co
-00015740: 6e74 6169 6e69 6e67 2062 7574 206e 6f74  ntaining but not
-00015750: 2073 7461 7274 696e 6720 7769 7468 2050   starting with P
-00015760: 4852 4153 452e 2054 6869 730a 2020 2020  HRASE. This.    
-00015770: 7365 6172 6368 2069 7320 6361 7365 2d69  search is case-i
-00015780: 6e73 656e 7369 7469 7665 2e0a 0a20 2020  nsensitive...   
-00015790: 2049 6620 7468 6520 272d 5427 2066 6c61   If the '-T' fla
-000157a0: 6720 6973 2070 6173 7365 642c 2073 6561  g is passed, sea
-000157b0: 7263 6865 7320 666f 7220 7461 6773 2069  rches for tags i
-000157c0: 6e73 7465 6164 206f 6620 736f 6e67 206e  nstead of song n
-000157d0: 616d 6573 2e22 2222 0a20 2020 2070 6872  ames.""".    phr
-000157e0: 6173 6520 3d20 7068 7261 7365 2e6c 6f77  ase = phrase.low
-000157f0: 6572 2829 0a20 2020 2077 6974 6820 6f70  er().    with op
-00015800: 656e 2853 4f4e 4753 5f49 4e46 4f5f 5041  en(SONGS_INFO_PA
-00015810: 5448 2c20 2272 222c 2065 6e63 6f64 696e  TH, "r", encodin
-00015820: 673d 2275 7466 2d38 2229 2061 7320 736f  g="utf-8") as so
-00015830: 6e67 735f 6669 6c65 3a0a 2020 2020 2020  ngs_file:.      
-00015840: 2020 6966 206e 6f74 2073 6561 7263 6869    if not searchi
-00015850: 6e67 5f66 6f72 5f74 6167 733a 0a20 2020  ng_for_tags:.   
-00015860: 2020 2020 2020 2020 2072 6573 756c 7473           results
-00015870: 203d 205b 5d2c 205b 5d20 2023 2073 7461   = [], []  # sta
-00015880: 7274 732c 2063 6f6e 7461 696e 7320 6275  rts, contains bu
-00015890: 7420 646f 6573 206e 6f74 2073 7461 7274  t does not start
-000158a0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-000158b0: 206c 696e 6520 696e 2073 6f6e 6773 5f66   line in songs_f
-000158c0: 696c 653a 0a20 2020 2020 2020 2020 2020  ile:.           
-000158d0: 2020 2020 2073 6f6e 675f 6964 2c20 736f       song_id, so
-000158e0: 6e67 5f6e 616d 652c 2074 6167 732c 202a  ng_name, tags, *
-000158f0: 5f20 3d20 6c69 6e65 2e73 7472 6970 2829  _ = line.strip()
-00015900: 2e73 706c 6974 2822 7c22 290a 2020 2020  .split("|").    
-00015910: 2020 2020 2020 2020 2020 2020 736f 6e67              song
-00015920: 5f69 6420 3d20 696e 7428 736f 6e67 5f69  _id = int(song_i
-00015930: 6429 0a20 2020 2020 2020 2020 2020 2020  d).             
-00015940: 2020 2073 6f6e 675f 6e61 6d65 203d 2073     song_name = s
-00015950: 6f6e 675f 6e61 6d65 2e6c 6f77 6572 2829  ong_name.lower()
-00015960: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015970: 2020 6966 2073 6f6e 675f 6e61 6d65 2e73    if song_name.s
-00015980: 7461 7274 7377 6974 6828 7068 7261 7365  tartswith(phrase
-00015990: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000159a0: 2020 2020 2020 2072 6573 756c 7473 5b30         results[0
-000159b0: 5d2e 6170 7065 6e64 2873 6f6e 675f 6964  ].append(song_id
-000159c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000159d0: 2020 656c 6966 2070 6872 6173 6520 696e    elif phrase in
-000159e0: 2073 6f6e 675f 6e61 6d65 3a0a 2020 2020   song_name:.    
-000159f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015a00: 7265 7375 6c74 735b 315d 2e61 7070 656e  results[1].appen
-00015a10: 6428 736f 6e67 5f69 6429 0a0a 2020 2020  d(song_id)..    
-00015a20: 2020 2020 2020 2020 6966 206e 6f74 2061          if not a
-00015a30: 6e79 2872 6573 756c 7473 293a 0a20 2020  ny(results):.   
-00015a40: 2020 2020 2020 2020 2020 2020 2063 6c69               cli
-00015a50: 636b 2e73 6563 686f 2822 4e6f 2072 6573  ck.secho("No res
-00015a60: 756c 7473 2066 6f75 6e64 2e22 2c20 6667  ults found.", fg
-00015a70: 3d22 7265 6422 290a 2020 2020 2020 2020  ="red").        
-00015a80: 2020 2020 2020 2020 7265 7475 726e 0a0a          return..
-00015a90: 2020 2020 2020 2020 2020 2020 736f 6e67              song
-00015aa0: 735f 6669 6c65 2e73 6565 6b28 3029 0a20  s_file.seek(0). 
-00015ab0: 2020 2020 2020 2020 2020 2066 6f72 206c             for l
-00015ac0: 696e 6520 696e 2073 6f6e 6773 5f66 696c  ine in songs_fil
-00015ad0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00015ae0: 2020 2064 6574 6169 6c73 203d 206c 696e     details = lin
-00015af0: 652e 7374 7269 7028 292e 7370 6c69 7428  e.strip().split(
-00015b00: 227c 2229 0a20 2020 2020 2020 2020 2020  "|").           
-00015b10: 2020 2020 2069 6620 696e 7428 6465 7461       if int(deta
-00015b20: 696c 735b 305d 2920 696e 2072 6573 756c  ils[0]) in resul
-00015b30: 7473 5b30 5d3a 0a20 2020 2020 2020 2020  ts[0]:.         
-00015b40: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00015b50: 5f65 6e74 7279 2864 6574 6169 6c73 2c20  _entry(details, 
-00015b60: 7068 7261 7365 290a 0a20 2020 2020 2020  phrase)..       
-00015b70: 2020 2020 2073 6f6e 6773 5f66 696c 652e       songs_file.
-00015b80: 7365 656b 2830 290a 2020 2020 2020 2020  seek(0).        
-00015b90: 2020 2020 666f 7220 6c69 6e65 2069 6e20      for line in 
-00015ba0: 736f 6e67 735f 6669 6c65 3a0a 2020 2020  songs_file:.    
-00015bb0: 2020 2020 2020 2020 2020 2020 6465 7461              deta
-00015bc0: 696c 7320 3d20 6c69 6e65 2e73 7472 6970  ils = line.strip
-00015bd0: 2829 2e73 706c 6974 2822 7c22 290a 2020  ().split("|").  
-00015be0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00015bf0: 2069 6e74 2864 6574 6169 6c73 5b30 5d29   int(details[0])
-00015c00: 2069 6e20 7265 7375 6c74 735b 315d 3a0a   in results[1]:.
-00015c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015c20: 2020 2020 7072 696e 745f 656e 7472 7928      print_entry(
-00015c30: 6465 7461 696c 732c 2070 6872 6173 6529  details, phrase)
-00015c40: 0a0a 2020 2020 2020 2020 2020 2020 636c  ..            cl
-00015c50: 6963 6b2e 7365 6368 6f28 0a20 2020 2020  ick.secho(.     
-00015c60: 2020 2020 2020 2020 2020 2066 2246 6f75             f"Fou
-00015c70: 6e64 207b 6c65 6e28 7265 7375 6c74 735b  nd {len(results[
-00015c80: 305d 2920 2b20 6c65 6e28 7265 7375 6c74  0]) + len(result
-00015c90: 735b 315d 297d 2073 6f6e 6728 7329 2e22  s[1])} song(s)."
-00015ca0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00015cb0: 2020 6667 3d22 6772 6565 6e22 2c0a 2020    fg="green",.  
-00015cc0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00015cd0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00015ce0: 2020 2020 2020 7265 7375 6c74 7320 3d20        results = 
-00015cf0: 7365 7428 292c 2073 6574 2829 2020 2320  set(), set()  # 
-00015d00: 7374 6172 7473 2c20 636f 6e74 6169 6e73  starts, contains
-00015d10: 2062 7574 2064 6f65 7320 6e6f 7420 7374   but does not st
-00015d20: 6172 740a 2020 2020 2020 2020 2020 2020  art.            
-00015d30: 666f 7220 6c69 6e65 2069 6e20 736f 6e67  for line in song
-00015d40: 735f 6669 6c65 3a0a 2020 2020 2020 2020  s_file:.        
-00015d50: 2020 2020 2020 2020 736f 6e67 5f69 642c          song_id,
-00015d60: 2073 6f6e 675f 6e61 6d65 2c20 7461 6773   song_name, tags
-00015d70: 2c20 2a5f 203d 206c 696e 652e 7374 7269  , *_ = line.stri
-00015d80: 7028 292e 7370 6c69 7428 227c 2229 0a20  p().split("|"). 
-00015d90: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00015da0: 6620 7461 6773 3a0a 2020 2020 2020 2020  f tags:.        
-00015db0: 2020 2020 2020 2020 2020 2020 7461 6773              tags
-00015dc0: 203d 2074 6167 732e 7370 6c69 7428 222c   = tags.split(",
-00015dd0: 2229 0a0a 2020 2020 2020 2020 2020 2020  ")..            
-00015de0: 2020 2020 2020 2020 666f 7220 7461 6720          for tag 
-00015df0: 696e 2074 6167 733a 0a20 2020 2020 2020  in tags:.       
-00015e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015e10: 2074 6167 5f6c 6f77 6572 203d 2074 6167   tag_lower = tag
-00015e20: 2e6c 6f77 6572 2829 0a20 2020 2020 2020  .lower().       
-00015e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015e40: 2069 6620 7461 675f 6c6f 7765 722e 7374   if tag_lower.st
-00015e50: 6172 7473 7769 7468 2870 6872 6173 6529  artswith(phrase)
-00015e60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00015e70: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00015e80: 7375 6c74 735b 305d 2e61 6464 2874 6167  sults[0].add(tag
-00015e90: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00015ea0: 2020 2020 2020 2020 2020 656c 6966 2070            elif p
-00015eb0: 6872 6173 6520 696e 2074 6167 5f6c 6f77  hrase in tag_low
-00015ec0: 6572 3a0a 2020 2020 2020 2020 2020 2020  er:.            
-00015ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015ee0: 7265 7375 6c74 735b 315d 2e61 6464 2874  results[1].add(t
-00015ef0: 6167 290a 0a20 2020 2020 2020 2020 2020  ag)..           
-00015f00: 2069 6620 6e6f 7420 616e 7928 7265 7375   if not any(resu
-00015f10: 6c74 7329 3a0a 2020 2020 2020 2020 2020  lts):.          
-00015f20: 2020 2020 2020 636c 6963 6b2e 7365 6368        click.sech
-00015f30: 6f28 224e 6f20 7265 7375 6c74 7320 666f  o("No results fo
-00015f40: 756e 642e 222c 2066 673d 2272 6564 2229  und.", fg="red")
-00015f50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015f60: 2072 6574 7572 6e0a 0a20 2020 2020 2020   return..       
-00015f70: 2020 2020 2066 6f72 2074 6167 2069 6e20       for tag in 
-00015f80: 7265 7375 6c74 735b 305d 3a0a 2020 2020  results[0]:.    
-00015f90: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00015fa0: 7428 7461 6729 0a0a 2020 2020 2020 2020  t(tag)..        
-00015fb0: 2020 2020 666f 7220 7461 6720 696e 2072      for tag in r
-00015fc0: 6573 756c 7473 5b31 5d3a 0a20 2020 2020  esults[1]:.     
-00015fd0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00015fe0: 2874 6167 290a 0a20 2020 2020 2020 2020  (tag)..         
-00015ff0: 2020 2063 6c69 636b 2e73 6563 686f 280a     click.secho(.
-00016000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016010: 6622 466f 756e 6420 7b6c 656e 2872 6573  f"Found {len(res
-00016020: 756c 7473 5b30 5d29 202b 206c 656e 2872  ults[0]) + len(r
-00016030: 6573 756c 7473 5b31 5d29 7d20 7461 6728  esults[1])} tag(
-00016040: 7329 2e22 2c20 6667 3d22 6772 6565 6e22  s).", fg="green"
-00016050: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-00016060: 0a40 636c 692e 636f 6d6d 616e 6428 6e61  .@cli.command(na
-00016070: 6d65 3d22 6c69 7374 2229 0a40 636c 6963  me="list").@clic
-00016080: 6b2e 6172 6775 6d65 6e74 2822 7365 6172  k.argument("sear
-00016090: 6368 5f74 6167 7322 2c20 6d65 7461 7661  ch_tags", metava
-000160a0: 723d 2254 4147 5322 2c20 6e61 7267 733d  r="TAGS", nargs=
-000160b0: 2d31 290a 4063 6c69 636b 2e6f 7074 696f  -1).@click.optio
-000160c0: 6e28 0a20 2020 2022 2d73 222c 0a20 2020  n(.    "-s",.   
-000160d0: 2022 2d2d 736f 7274 222c 0a20 2020 2022   "--sort",.    "
-000160e0: 736f 7274 5f22 2c0a 2020 2020 7479 7065  sort_",.    type
-000160f0: 3d63 6c69 636b 2e43 686f 6963 6528 0a20  =click.Choice(. 
-00016100: 2020 2020 2020 2028 0a20 2020 2020 2020         (.       
-00016110: 2020 2020 2022 6e6f 6e65 222c 0a20 2020       "none",.   
-00016120: 2020 2020 2020 2020 2022 6e61 6d65 222c           "name",
-00016130: 0a20 2020 2020 2020 2020 2020 2022 6e22  .            "n"
-00016140: 2c0a 2020 2020 2020 2020 2020 2020 2273  ,.            "s
-00016150: 6563 732d 6c69 7374 656e 6564 222c 0a20  ecs-listened",. 
-00016160: 2020 2020 2020 2020 2020 2022 7322 2c0a             "s",.
-00016170: 2020 2020 2020 2020 2020 2020 2264 7572              "dur
-00016180: 6174 696f 6e22 2c0a 2020 2020 2020 2020  ation",.        
-00016190: 2020 2020 2264 222c 0a20 2020 2020 2020      "d",.       
-000161a0: 2020 2020 2022 7469 6d65 732d 6c69 7374       "times-list
-000161b0: 656e 6564 222c 0a20 2020 2020 2020 2020  ened",.         
-000161c0: 2020 2022 7422 2c0a 2020 2020 2020 2020     "t",.        
-000161d0: 290a 2020 2020 292c 0a20 2020 2068 656c  ).    ),.    hel
-000161e0: 703d 2253 6f72 7420 6279 206e 616d 652c  p="Sort by name,
-000161f0: 2073 6563 6f6e 6473 206c 6973 7465 6e65   seconds listene
-00016200: 642c 206f 7220 7469 6d65 7320 6c69 7374  d, or times list
-00016210: 656e 6564 2028 7365 636f 6e64 732f 736f  ened (seconds/so
-00016220: 6e67 2064 7572 6174 696f 6e29 2e20 4772  ng duration). Gr
-00016230: 6561 7465 7374 2066 6972 7374 2e22 2c0a  eatest first.",.
-00016240: 2020 2020 6465 6661 756c 743d 226e 6f6e      default="non
-00016250: 6522 2c0a 2020 2020 7368 6f77 5f64 6566  e",.    show_def
-00016260: 6175 6c74 3d54 7275 652c 0a29 0a40 636c  ault=True,.).@cl
-00016270: 6963 6b2e 6f70 7469 6f6e 280a 2020 2020  ick.option(.    
-00016280: 222d 522f 2d6e 5222 2c0a 2020 2020 222d  "-R/-nR",.    "-
-00016290: 2d72 6576 6572 7365 2f2d 2d6e 6f2d 7265  -reverse/--no-re
-000162a0: 7665 7273 6522 2c0a 2020 2020 2272 6576  verse",.    "rev
-000162b0: 6572 7365 5f22 2c0a 2020 2020 6465 6661  erse_",.    defa
-000162c0: 756c 743d 4661 6c73 652c 0a20 2020 2068  ult=False,.    h
-000162d0: 656c 703d 2252 6576 6572 7365 2074 6865  elp="Reverse the
-000162e0: 2073 6f72 7469 6e67 206f 7264 6572 2028   sorting order (
-000162f0: 6772 6561 7465 7374 2066 6972 7374 292e  greatest first).
-00016300: 222c 0a29 0a40 636c 6963 6b2e 6f70 7469  ",.).@click.opti
-00016310: 6f6e 280a 2020 2020 222d 542f 2d6e 5422  on(.    "-T/-nT"
-00016320: 2c0a 2020 2020 222d 2d74 6167 2f2d 2d6e  ,.    "--tag/--n
-00016330: 6f2d 7461 6722 2c0a 2020 2020 226c 6973  o-tag",.    "lis
-00016340: 7469 6e67 5f74 6167 7322 2c0a 2020 2020  ting_tags",.    
-00016350: 6465 6661 756c 743d 4661 6c73 652c 0a20  default=False,. 
-00016360: 2020 2068 656c 703d 224c 6973 7420 7461     help="List ta
-00016370: 6773 206d 6174 6368 696e 6720 5441 4753  gs matching TAGS
-00016380: 2069 6e73 7465 6164 206f 6620 736f 6e67   instead of song
-00016390: 732e 222c 0a29 0a40 636c 6963 6b2e 6f70  s.",.).@click.op
-000163a0: 7469 6f6e 280a 2020 2020 222d 7922 2c0a  tion(.    "-y",.
-000163b0: 2020 2020 222d 2d79 6561 7222 2c0a 2020      "--year",.  
-000163c0: 2020 2279 6561 7222 2c0a 2020 2020 6865    "year",.    he
-000163d0: 6c70 3d22 5368 6f77 2074 696d 6520 6c69  lp="Show time li
-000163e0: 7374 656e 6564 2066 6f72 2061 2073 7065  stened for a spe
-000163f0: 6369 6669 6320 7965 6172 2c20 696e 7374  cific year, inst
-00016400: 6561 6420 6f66 2074 6865 2074 6f74 616c  ead of the total
-00016410: 2e20 5061 7373 696e 6720 2763 7572 2720  . Passing 'cur' 
-00016420: 7769 6c6c 2073 686f 7720 7468 6520 7469  will show the ti
-00016430: 6d65 206c 6973 7465 6e65 6420 666f 7220  me listened for 
-00016440: 7468 6520 6375 7272 656e 7420 7965 6172  the current year
-00016450: 2e22 2c0a 290a 4063 6c69 636b 2e6f 7074  .",.).@click.opt
-00016460: 696f 6e28 222d 7422 2c20 222d 2d74 6f70  ion("-t", "--top
-00016470: 222c 2022 746f 7022 2c20 7479 7065 3d69  ", "top", type=i
-00016480: 6e74 2c20 6865 6c70 3d22 5368 6f77 2074  nt, help="Show t
-00016490: 6865 2074 6f70 206e 2073 6f6e 6773 2f74  he top n songs/t
-000164a0: 6167 732e 2229 0a40 636c 6963 6b2e 6f70  ags.").@click.op
-000164b0: 7469 6f6e 280a 2020 2020 222d 4d2f 2d6e  tion(.    "-M/-n
-000164c0: 4d22 2c0a 2020 2020 222d 2d6d 6174 6368  M",.    "--match
-000164d0: 2d61 6c6c 2f2d 2d6e 6f2d 6d61 7463 682d  -all/--no-match-
-000164e0: 616c 6c22 2c0a 2020 2020 226d 6174 6368  all",.    "match
-000164f0: 5f61 6c6c 222c 0a20 2020 2064 6566 6175  _all",.    defau
-00016500: 6c74 3d46 616c 7365 2c0a 2020 2020 6865  lt=False,.    he
-00016510: 6c70 3d22 5368 6f77 7320 736f 6e67 7320  lp="Shows songs 
-00016520: 7468 6174 206d 6174 6368 2061 6c6c 2074  that match all t
-00016530: 6167 7320 696e 7374 6561 6420 6f66 2061  ags instead of a
-00016540: 6e79 2074 6167 2e20 4967 6e6f 7265 6420  ny tag. Ignored 
-00016550: 6966 2027 2d74 2f2d 2d74 6167 2720 6973  if '-t/--tag' is
-00016560: 2070 6173 7365 642e 222c 0a29 0a64 6566   passed.",.).def
-00016570: 206c 6973 745f 2873 6561 7263 685f 7461   list_(search_ta
-00016580: 6773 2c20 6c69 7374 696e 675f 7461 6773  gs, listing_tags
-00016590: 2c20 7965 6172 2c20 736f 7274 5f2c 2074  , year, sort_, t
-000165a0: 6f70 2c20 7265 7665 7273 655f 2c20 6d61  op, reverse_, ma
-000165b0: 7463 685f 616c 6c29 3a0a 2020 2020 2222  tch_all):.    ""
-000165c0: 224c 6973 7420 7468 6520 656e 7472 6965  "List the entrie
-000165d0: 7320 666f 7220 616c 6c20 736f 6e67 732e  s for all songs.
-000165e0: 0a0a 2020 2020 4f75 7470 7574 2066 6f72  ..    Output for
-000165f0: 6d61 743a 2049 442c 206e 616d 652c 2064  mat: ID, name, d
-00016600: 7572 6174 696f 6e2c 206c 6973 7465 6e20  uration, listen 
-00016610: 7469 6d65 2c20 7469 6d65 7320 6c69 7374  time, times list
-00016620: 656e 6564 2c20 5b63 6c69 702d 7374 6172  ened, [clip-star
-00016630: 742c 2063 6c69 702d 656e 645d 2069 6620  t, clip-end] if 
-00016640: 636c 6970 2065 7869 7374 732c 2063 6f6d  clip exists, com
-00016650: 6d61 2d73 6570 6172 6174 6564 2074 6167  ma-separated tag
-00016660: 7320 6966 2061 6e79 0a0a 2020 2020 4966  s if any..    If
-00016670: 2074 6865 2027 2d54 2720 666c 6167 2069   the '-T' flag i
-00016680: 7320 7061 7373 6564 2c20 7461 6773 2077  s passed, tags w
-00016690: 696c 6c20 6265 206c 6973 7465 6420 696e  ill be listed in
-000166a0: 7374 6561 6420 6f66 2073 6f6e 6773 2e0a  stead of songs..
-000166b0: 0a20 2020 204f 7574 7075 7420 666f 726d  .    Output form
-000166c0: 6174 3a20 7461 672c 2064 7572 6174 696f  at: tag, duratio
-000166d0: 6e2c 206c 6973 7465 6e20 7469 6d65 2c20  n, listen time, 
-000166e0: 7469 6d65 7320 6c69 7374 656e 6564 0a0a  times listened..
-000166f0: 2020 2020 4966 2054 4147 5320 6172 6520      If TAGS are 
-00016700: 7061 7373 6564 2c20 616e 7920 7461 672f  passed, any tag/
-00016710: 736f 6e67 206d 6174 6368 696e 6720 616e  song matching an
-00016720: 7920 7461 6720 696e 2054 4147 5320 7769  y tag in TAGS wi
-00016730: 6c6c 2062 6520 6c69 7374 6564 2c0a 2020  ll be listed,.  
-00016740: 2020 756e 6c65 7373 2074 6865 2027 2d4d    unless the '-M
-00016750: 2f2d 2d6d 6174 6368 2d61 6c6c 2720 666c  /--match-all' fl
-00016760: 6167 2069 7320 7061 7373 6564 2c20 696e  ag is passed, in
-00016770: 2077 6869 6368 2063 6173 6520 6576 6572   which case ever
-00016780: 7920 7461 6720 6d75 7374 0a20 2020 2062  y tag must.    b
-00016790: 6520 6d61 7463 6865 6420 2869 676e 6f72  e matched (ignor
-000167a0: 6564 2069 6620 6c69 7374 696e 6720 7461  ed if listing ta
-000167b0: 6773 292e 0a20 2020 2022 2222 0a20 2020  gs)..    """.   
-000167c0: 2069 6620 746f 7020 6973 206e 6f74 204e   if top is not N
-000167d0: 6f6e 653a 0a20 2020 2020 2020 2069 6620  one:.        if 
-000167e0: 746f 7020 3c20 313a 0a20 2020 2020 2020  top < 1:.       
-000167f0: 2020 2020 2063 6c69 636b 2e73 6563 686f       click.secho
-00016800: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00016810: 2020 2254 6865 206f 7074 696f 6e20 272d    "The option '-
-00016820: 742f 2d2d 746f 7027 206d 7573 7420 6265  t/--top' must be
-00016830: 2061 2070 6f73 6974 6976 6520 6e75 6d62   a positive numb
-00016840: 6572 2e22 2c20 6667 3d22 7265 6422 0a20  er.", fg="red". 
-00016850: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00016860: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
-00016870: 0a20 2020 2069 6620 7965 6172 2069 7320  .    if year is 
-00016880: 4e6f 6e65 3a0a 2020 2020 2020 2020 7374  None:.        st
-00016890: 6174 735f 7061 7468 203d 2054 4f54 414c  ats_path = TOTAL
-000168a0: 5f53 5441 5453 5f50 4154 480a 2020 2020  _STATS_PATH.    
-000168b0: 656c 7365 3a0a 2020 2020 2020 2020 6966  else:.        if
-000168c0: 2079 6561 7220 3d3d 2022 6375 7222 3a0a   year == "cur":.
-000168d0: 2020 2020 2020 2020 2020 2020 7965 6172              year
-000168e0: 203d 2043 5552 5f59 4541 520a 2020 2020   = CUR_YEAR.    
-000168f0: 2020 2020 2020 2020 7374 6174 735f 7061          stats_pa
-00016900: 7468 203d 2043 5552 5f59 4541 525f 5354  th = CUR_YEAR_ST
-00016910: 4154 535f 5041 5448 0a20 2020 2020 2020  ATS_PATH.       
-00016920: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00016930: 2020 2069 6620 6e6f 7420 7965 6172 2e69     if not year.i
-00016940: 7364 6967 6974 2829 3a0a 2020 2020 2020  sdigit():.      
-00016950: 2020 2020 2020 2020 2020 636c 6963 6b2e            click.
-00016960: 7365 6368 6f28 2259 6561 7220 6d75 7374  secho("Year must
-00016970: 2062 6520 6120 6e75 6d62 6572 206f 7220   be a number or 
-00016980: 2763 7572 272e 222c 2066 673d 2272 6564  'cur'.", fg="red
-00016990: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-000169a0: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
-000169b0: 2020 2020 2020 7374 6174 735f 7061 7468        stats_path
-000169c0: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
-000169d0: 5354 4154 535f 4449 522c 2066 227b 7965  STATS_DIR, f"{ye
-000169e0: 6172 7d2e 7478 7422 290a 2020 2020 2020  ar}.txt").      
-000169f0: 2020 2020 2020 6966 206e 6f74 206f 732e        if not os.
-00016a00: 7061 7468 2e65 7869 7374 7328 7374 6174  path.exists(stat
-00016a10: 735f 7061 7468 293a 0a20 2020 2020 2020  s_path):.       
-00016a20: 2020 2020 2020 2020 2063 6c69 636b 2e73           click.s
-00016a30: 6563 686f 2866 224e 6f20 7374 6174 7320  echo(f"No stats 
-00016a40: 666f 756e 6420 666f 7220 7965 6172 207b  found for year {
-00016a50: 7965 6172 7d2e 222c 2066 673d 2272 6564  year}.", fg="red
-00016a60: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-00016a70: 2020 2072 6574 7572 6e0a 0a20 2020 2069     return..    i
-00016a80: 6620 7365 6172 6368 5f74 6167 733a 0a20  f search_tags:. 
-00016a90: 2020 2020 2020 2073 6561 7263 685f 7461         search_ta
-00016aa0: 6773 203d 2073 6574 2873 6561 7263 685f  gs = set(search_
-00016ab0: 7461 6773 290a 0a20 2020 206e 756d 5f6c  tags)..    num_l
-00016ac0: 696e 6573 203d 2030 0a0a 2020 2020 6966  ines = 0..    if
-00016ad0: 206c 6973 7469 6e67 5f74 6167 733a 0a20   listing_tags:. 
-00016ae0: 2020 2020 2020 2077 6974 6820 280a 2020         with (.  
-00016af0: 2020 2020 2020 2020 2020 6f70 656e 2853            open(S
-00016b00: 4f4e 4753 5f49 4e46 4f5f 5041 5448 2c20  ONGS_INFO_PATH, 
-00016b10: 2272 222c 2065 6e63 6f64 696e 673d 2275  "r", encoding="u
-00016b20: 7466 2d38 2229 2061 7320 736f 6e67 735f  tf-8") as songs_
-00016b30: 6669 6c65 2c0a 2020 2020 2020 2020 2020  file,.          
-00016b40: 2020 6f70 656e 2873 7461 7473 5f70 6174    open(stats_pat
-00016b50: 682c 2022 7222 2c20 656e 636f 6469 6e67  h, "r", encoding
-00016b60: 3d22 7574 662d 3822 2920 6173 2073 7461  ="utf-8") as sta
-00016b70: 7473 5f66 696c 652c 0a20 2020 2020 2020  ts_file,.       
-00016b80: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
-00016b90: 736f 6e67 735f 6c69 6e65 7320 3d20 736f  songs_lines = so
-00016ba0: 6e67 735f 6669 6c65 2e72 6561 646c 696e  ngs_file.readlin
-00016bb0: 6573 2829 0a20 2020 2020 2020 2020 2020  es().           
-00016bc0: 2073 7461 7473 203d 2064 6963 7428 0a20   stats = dict(. 
-00016bd0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00016be0: 6170 280a 2020 2020 2020 2020 2020 2020  ap(.            
-00016bf0: 2020 2020 2020 2020 6c61 6d62 6461 2074          lambda t
-00016c00: 3a20 2869 6e74 2874 5b30 5d29 2c29 202b  : (int(t[0]),) +
-00016c10: 2074 5b31 3a5d 2c0a 2020 2020 2020 2020   t[1:],.        
-00016c20: 2020 2020 2020 2020 2020 2020 6d61 7028              map(
-00016c30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016c40: 2020 2020 2020 2020 206c 616d 6264 6120           lambda 
-00016c50: 783a 2074 7570 6c65 286d 6170 2866 6c6f  x: tuple(map(flo
-00016c60: 6174 2c20 782e 7374 7269 7028 292e 7370  at, x.strip().sp
-00016c70: 6c69 7428 227c 2229 2929 2c0a 2020 2020  lit("|"))),.    
-00016c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016c90: 2020 2020 7374 6174 735f 6669 6c65 2e72      stats_file.r
-00016ca0: 6561 646c 696e 6573 2829 2c0a 2020 2020  eadlines(),.    
-00016cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016cc0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00016cd0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00016ce0: 2029 0a0a 2020 2020 2020 2020 2020 2020   )..            
-00016cf0: 7461 6773 203d 2064 6566 6175 6c74 6469  tags = defaultdi
-00016d00: 6374 286c 616d 6264 613a 2028 302e 302c  ct(lambda: (0.0,
-00016d10: 2030 2e30 2929 0a0a 2020 2020 2020 2020   0.0))..        
-00016d20: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-00016d30: 6765 286c 656e 2873 6f6e 6773 5f6c 696e  ge(len(songs_lin
-00016d40: 6573 2929 3a0a 2020 2020 2020 2020 2020  es)):.          
-00016d50: 2020 2020 2020 736f 6e67 5f69 642c 2073        song_id, s
-00016d60: 6f6e 675f 6e61 6d65 2c20 7461 675f 7374  ong_name, tag_st
-00016d70: 7269 6e67 203d 2028 0a20 2020 2020 2020  ring = (.       
-00016d80: 2020 2020 2020 2020 2020 2020 2073 6f6e               son
-00016d90: 6773 5f6c 696e 6573 5b69 5d2e 7374 7269  gs_lines[i].stri
-00016da0: 7028 292e 7370 6c69 7428 227c 2229 5b30  p().split("|")[0
-00016db0: 3a33 5d0a 2020 2020 2020 2020 2020 2020  :3].            
-00016dc0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00016dd0: 2020 2020 2020 736f 6e67 5f69 6420 3d20        song_id = 
-00016de0: 696e 7428 736f 6e67 5f69 6429 0a20 2020  int(song_id).   
-00016df0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00016e00: 7461 675f 7374 7269 6e67 3a0a 2020 2020  tag_string:.    
-00016e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016e20: 666f 7220 7461 6720 696e 2074 6167 5f73  for tag in tag_s
-00016e30: 7472 696e 672e 7370 6c69 7428 222c 2229  tring.split(",")
-00016e40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00016e50: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-00016e60: 2073 6561 7263 685f 7461 6773 206f 7220   search_tags or 
-00016e70: 7461 6720 696e 2073 6561 7263 685f 7461  tag in search_ta
-00016e80: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-00016e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ea0: 7461 6773 5b74 6167 5d20 3d20 280a 2020  tags[tag] = (.  
-00016eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ec0: 2020 2020 2020 2020 2020 2020 2020 7461                ta
-00016ed0: 6773 5b74 6167 5d5b 305d 202b 2073 7461  gs[tag][0] + sta
-00016ee0: 7473 5b73 6f6e 675f 6964 5d2c 0a20 2020  ts[song_id],.   
-00016ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016f00: 2020 2020 2020 2020 2020 2020 2074 6167               tag
-00016f10: 735b 7461 675d 5b31 5d0a 2020 2020 2020  s[tag][1].      
-00016f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016f30: 2020 2020 2020 2020 2020 2b20 6d75 7369            + musi
-00016f40: 635f 7461 672e 6c6f 6164 5f66 696c 6528  c_tag.load_file(
-00016f50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016f70: 2020 2020 206f 732e 7061 7468 2e6a 6f69       os.path.joi
-00016f80: 6e28 534f 4e47 535f 4449 522c 2073 6f6e  n(SONGS_DIR, son
-00016f90: 675f 6e61 6d65 290a 2020 2020 2020 2020  g_name).        
-00016fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016fb0: 2020 2020 2020 2020 295b 2223 6c65 6e67          )["#leng
-00016fc0: 7468 225d 2e76 616c 7565 2c0a 2020 2020  th"].value,.    
-00016fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016fe0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-00016ff0: 2020 2020 2020 2074 6167 5f69 7465 6d73         tag_items
-00017000: 203d 206c 6973 7428 7461 6773 2e69 7465   = list(tags.ite
-00017010: 6d73 2829 290a 0a20 2020 2020 2020 2020  ms())..         
-00017020: 2020 2069 6620 736f 7274 5f20 213d 2022     if sort_ != "
-00017030: 6e6f 6e65 223a 0a20 2020 2020 2020 2020  none":.         
-00017040: 2020 2020 2020 2069 6620 736f 7274 5f20         if sort_ 
-00017050: 696e 2028 226e 616d 6522 2c20 226e 2229  in ("name", "n")
-00017060: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00017070: 2020 2020 2020 736f 7274 5f6b 6579 203d        sort_key =
-00017080: 206c 616d 6264 6120 743a 2074 5b30 5d0a   lambda t: t[0].
-00017090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000170a0: 656c 6966 2073 6f72 745f 2069 6e20 2822  elif sort_ in ("
-000170b0: 7365 6373 2d6c 6973 7465 6e65 6422 2c20  secs-listened", 
-000170c0: 2273 2229 3a0a 2020 2020 2020 2020 2020  "s"):.          
-000170d0: 2020 2020 2020 2020 2020 736f 7274 5f6b            sort_k
-000170e0: 6579 203d 206c 616d 6264 6120 743a 2074  ey = lambda t: t
-000170f0: 5b31 5d5b 305d 0a20 2020 2020 2020 2020  [1][0].         
-00017100: 2020 2020 2020 2065 6c69 6620 736f 7274         elif sort
-00017110: 5f20 696e 2028 2264 7572 6174 696f 6e22  _ in ("duration"
-00017120: 2c20 2264 2229 3a0a 2020 2020 2020 2020  , "d"):.        
-00017130: 2020 2020 2020 2020 2020 2020 736f 7274              sort
-00017140: 5f6b 6579 203d 206c 616d 6264 6120 743a  _key = lambda t:
-00017150: 2074 5b31 5d5b 315d 0a20 2020 2020 2020   t[1][1].       
-00017160: 2020 2020 2020 2020 2065 6c69 6620 736f           elif so
-00017170: 7274 5f20 696e 2028 2274 696d 6573 2d6c  rt_ in ("times-l
-00017180: 6973 7465 6e65 6422 2c20 2274 2229 3a0a  istened", "t"):.
-00017190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000171a0: 2020 2020 736f 7274 5f6b 6579 203d 206c      sort_key = l
-000171b0: 616d 6264 6120 743a 2074 5b31 5d5b 305d  ambda t: t[1][0]
-000171c0: 202f 2074 5b31 5d5b 315d 0a20 2020 2020   / t[1][1].     
-000171d0: 2020 2020 2020 2020 2020 2074 6167 5f69             tag_i
-000171e0: 7465 6d73 2e73 6f72 7428 0a20 2020 2020  tems.sort(.     
-000171f0: 2020 2020 2020 2020 2020 2020 2020 206b                 k
-00017200: 6579 3d73 6f72 745f 6b65 792c 0a20 2020  ey=sort_key,.   
-00017210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017220: 2072 6576 6572 7365 3d6e 6f74 2072 6576   reverse=not rev
-00017230: 6572 7365 5f2c 0a20 2020 2020 2020 2020  erse_,.         
-00017240: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00017250: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00017260: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-00017270: 7420 7265 7665 7273 655f 3a0a 2020 2020  t reverse_:.    
-00017280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017290: 7461 675f 6974 656d 732e 7265 7665 7273  tag_items.revers
-000172a0: 6528 290a 0a20 2020 2020 2020 2020 2020  e()..           
-000172b0: 2066 6f72 2074 6167 2c20 286c 6973 7465   for tag, (liste
-000172c0: 6e5f 7469 6d65 2c20 746f 7461 6c5f 6475  n_time, total_du
-000172d0: 7261 7469 6f6e 2920 696e 2074 6167 5f69  ration) in tag_i
-000172e0: 7465 6d73 3a0a 2020 2020 2020 2020 2020  tems:.          
-000172f0: 2020 2020 2020 636c 6963 6b2e 6563 686f        click.echo
-00017300: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00017310: 2020 2020 2020 6622 7b74 6167 7d20 7b63        f"{tag} {c
-00017320: 6c69 636b 2e73 7479 6c65 2866 6f72 6d61  lick.style(forma
-00017330: 745f 7365 636f 6e64 7328 746f 7461 6c5f  t_seconds(total_
-00017340: 6475 7261 7469 6f6e 2c20 7368 6f77 5f64  duration, show_d
-00017350: 6563 696d 616c 3d54 7275 6529 2c20 6667  ecimal=True), fg
-00017360: 3d27 6272 6967 6874 5f62 6c61 636b 2729  ='bright_black')
-00017370: 7d20 7b63 6c69 636b 2e73 7479 6c65 2866  } {click.style(f
-00017380: 6f72 6d61 745f 7365 636f 6e64 7328 6c69  ormat_seconds(li
-00017390: 7374 656e 5f74 696d 652c 2073 686f 775f  sten_time, show_
-000173a0: 6465 6369 6d61 6c3d 5472 7565 292c 2066  decimal=True), f
-000173b0: 673d 2779 656c 6c6f 7727 297d 207b 636c  g='yellow')} {cl
-000173c0: 6963 6b2e 7374 796c 6528 2725 2e32 6627  ick.style('%.2f'
-000173d0: 2528 6c69 7374 656e 5f74 696d 652f 746f  %(listen_time/to
-000173e0: 7461 6c5f 6475 7261 7469 6f6e 292c 2066  tal_duration), f
-000173f0: 673d 2767 7265 656e 2729 7d22 0a20 2020  g='green')}".   
-00017400: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-00017410: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00017420: 756d 5f6c 696e 6573 202b 3d20 310a 2020  um_lines += 1.  
-00017430: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00017440: 2074 6f70 2069 7320 6e6f 7420 4e6f 6e65   top is not None
-00017450: 2061 6e64 206e 756d 5f6c 696e 6573 203d   and num_lines =
-00017460: 3d20 746f 703a 0a20 2020 2020 2020 2020  = top:.         
-00017470: 2020 2020 2020 2020 2020 2062 7265 616b             break
-00017480: 0a20 2020 2020 2020 2072 6574 7572 6e0a  .        return.
-00017490: 0a20 2020 206e 6f5f 7265 7375 6c74 7320  .    no_results 
-000174a0: 3d20 5472 7565 0a20 2020 2077 6974 6820  = True.    with 
-000174b0: 280a 2020 2020 2020 2020 6f70 656e 2853  (.        open(S
-000174c0: 4f4e 4753 5f49 4e46 4f5f 5041 5448 2c20  ONGS_INFO_PATH, 
-000174d0: 2272 222c 2065 6e63 6f64 696e 673d 2275  "r", encoding="u
-000174e0: 7466 2d38 2229 2061 7320 736f 6e67 735f  tf-8") as songs_
-000174f0: 6669 6c65 2c0a 2020 2020 2020 2020 6f70  file,.        op
-00017500: 656e 2873 7461 7473 5f70 6174 682c 2022  en(stats_path, "
-00017510: 7222 2c20 656e 636f 6469 6e67 3d22 7574  r", encoding="ut
-00017520: 662d 3822 2920 6173 2073 7461 7473 5f66  f-8") as stats_f
-00017530: 696c 652c 0a20 2020 2029 3a0a 2020 2020  ile,.    ):.    
-00017540: 2020 2020 6c69 6e65 7320 3d20 736f 6e67      lines = song
-00017550: 735f 6669 6c65 2e72 6561 646c 696e 6573  s_file.readlines
-00017560: 2829 0a20 2020 2020 2020 2073 7461 7473  ().        stats
-00017570: 203d 2064 6963 7428 0a20 2020 2020 2020   = dict(.       
-00017580: 2020 2020 206d 6170 280a 2020 2020 2020       map(.      
-00017590: 2020 2020 2020 2020 2020 6c61 6d62 6461            lambda
-000175a0: 2074 3a20 2869 6e74 2874 5b30 5d29 2c29   t: (int(t[0]),)
-000175b0: 202b 2074 5b31 3a5d 2c0a 2020 2020 2020   + t[1:],.      
-000175c0: 2020 2020 2020 2020 2020 6d61 7028 0a20            map(. 
-000175d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000175e0: 2020 206c 616d 6264 6120 783a 2074 7570     lambda x: tup
-000175f0: 6c65 286d 6170 2866 6c6f 6174 2c20 782e  le(map(float, x.
-00017600: 7374 7269 7028 292e 7370 6c69 7428 227c  strip().split("|
-00017610: 2229 2929 2c0a 2020 2020 2020 2020 2020  "))),.          
-00017620: 2020 2020 2020 2020 2020 7374 6174 735f            stats_
-00017630: 6669 6c65 2e72 6561 646c 696e 6573 2829  file.readlines()
-00017640: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00017650: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
-00017660: 2029 0a20 2020 2020 2020 2029 0a0a 2020   ).        )..  
-00017670: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
-00017680: 616e 6765 286c 656e 286c 696e 6573 2929  ange(len(lines))
-00017690: 3a0a 2020 2020 2020 2020 2020 2020 6465  :.            de
-000176a0: 7461 696c 7320 3d20 6c69 6e65 735b 695d  tails = lines[i]
-000176b0: 2e73 7472 6970 2829 2e73 706c 6974 2822  .strip().split("
-000176c0: 7c22 290a 2020 2020 2020 2020 2020 2020  |").            
-000176d0: 736f 6e67 5f69 6420 3d20 696e 7428 6465  song_id = int(de
-000176e0: 7461 696c 735b 305d 290a 0a20 2020 2020  tails[0])..     
-000176f0: 2020 2020 2020 2074 6167 7320 3d20 7365         tags = se
-00017700: 7428 6465 7461 696c 735b 325d 2e73 706c  t(details[2].spl
-00017710: 6974 2822 2c22 2929 0a20 2020 2020 2020  it(",")).       
-00017720: 2020 2020 2069 6620 7365 6172 6368 5f74       if search_t
-00017730: 6167 733a 0a20 2020 2020 2020 2020 2020  ags:.           
-00017740: 2020 2020 2069 6620 6d61 7463 685f 616c       if match_al
-00017750: 6c3a 0a20 2020 2020 2020 2020 2020 2020  l:.             
-00017760: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
-00017770: 6172 6368 5f74 6167 7320 3c3d 2074 6167  arch_tags <= tag
-00017780: 733a 2020 2320 7375 6273 6574 0a20 2020  s:  # subset.   
-00017790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000177a0: 2020 2020 206c 696e 6573 5b69 5d20 3d20       lines[i] = 
-000177b0: 2222 0a20 2020 2020 2020 2020 2020 2020  "".             
-000177c0: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
-000177d0: 6e75 650a 2020 2020 2020 2020 2020 2020  nue.            
-000177e0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-000177f0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00017800: 206e 6f74 2073 6561 7263 685f 7461 6773   not search_tags
-00017810: 2026 2074 6167 733a 2020 2320 696e 7465   & tags:  # inte
-00017820: 7273 6563 7469 6f6e 0a20 2020 2020 2020  rsection.       
-00017830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017840: 206c 696e 6573 5b69 5d20 3d20 2222 0a20   lines[i] = "". 
-00017850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017860: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
-00017870: 0a20 2020 2020 2020 2020 2020 2074 696d  .            tim
-00017880: 655f 6c69 7374 656e 6564 203d 2073 7461  e_listened = sta
-00017890: 7473 5b73 6f6e 675f 6964 5d0a 2020 2020  ts[song_id].    
-000178a0: 2020 2020 2020 2020 6c69 6e65 735b 695d          lines[i]
-000178b0: 203d 2074 7570 6c65 2864 6574 6169 6c73   = tuple(details
-000178c0: 2920 2b20 280a 2020 2020 2020 2020 2020  ) + (.          
-000178d0: 2020 2020 2020 7469 6d65 5f6c 6973 7465        time_liste
-000178e0: 6e65 642c 0a20 2020 2020 2020 2020 2020  ned,.           
-000178f0: 2020 2020 206d 7573 6963 5f74 6167 2e6c       music_tag.l
-00017900: 6f61 645f 6669 6c65 286f 732e 7061 7468  oad_file(os.path
-00017910: 2e6a 6f69 6e28 534f 4e47 535f 4449 522c  .join(SONGS_DIR,
-00017920: 2064 6574 6169 6c73 5b31 5d29 295b 0a20   details[1]))[. 
-00017930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017940: 2020 2022 236c 656e 6774 6822 0a20 2020     "#length".   
-00017950: 2020 2020 2020 2020 2020 2020 205d 2e76               ].v
-00017960: 616c 7565 2c0a 2020 2020 2020 2020 2020  alue,.          
-00017970: 2020 290a 0a20 2020 2020 2020 206c 696e    )..        lin
-00017980: 6573 203d 205b 6c69 6e65 2066 6f72 206c  es = [line for l
-00017990: 696e 6520 696e 206c 696e 6573 2069 6620  ine in lines if 
-000179a0: 6c69 6e65 5d0a 0a20 2020 2020 2020 2069  line]..        i
-000179b0: 6620 736f 7274 5f20 213d 2022 6e6f 6e65  f sort_ != "none
-000179c0: 223a 0a20 2020 2020 2020 2020 2020 2069  ":.            i
-000179d0: 6620 736f 7274 5f20 696e 2028 226e 616d  f sort_ in ("nam
-000179e0: 6522 2c20 226e 2229 3a0a 2020 2020 2020  e", "n"):.      
-000179f0: 2020 2020 2020 2020 2020 736f 7274 5f6b            sort_k
-00017a00: 6579 203d 206c 616d 6264 6120 743a 2074  ey = lambda t: t
-00017a10: 5b31 5d0a 2020 2020 2020 2020 2020 2020  [1].            
-00017a20: 656c 6966 2073 6f72 745f 2069 6e20 2822  elif sort_ in ("
-00017a30: 7365 6373 2d6c 6973 7465 6e65 6422 2c20  secs-listened", 
-00017a40: 2273 2229 3a0a 2020 2020 2020 2020 2020  "s"):.          
-00017a50: 2020 2020 2020 736f 7274 5f6b 6579 203d        sort_key =
-00017a60: 206c 616d 6264 6120 743a 2066 6c6f 6174   lambda t: float
-00017a70: 2874 5b2d 325d 290a 2020 2020 2020 2020  (t[-2]).        
-00017a80: 2020 2020 656c 6966 2073 6f72 745f 2069      elif sort_ i
-00017a90: 6e20 2822 6475 7261 7469 6f6e 222c 2022  n ("duration", "
-00017aa0: 6422 293a 0a20 2020 2020 2020 2020 2020  d"):.           
-00017ab0: 2020 2020 2073 6f72 745f 6b65 7920 3d20       sort_key = 
-00017ac0: 6c61 6d62 6461 2074 3a20 666c 6f61 7428  lambda t: float(
-00017ad0: 745b 2d31 5d29 0a20 2020 2020 2020 2020  t[-1]).         
-00017ae0: 2020 2065 6c69 6620 736f 7274 5f20 696e     elif sort_ in
-00017af0: 2028 2274 696d 6573 2d6c 6973 7465 6e65   ("times-listene
-00017b00: 6422 2c20 2274 2229 3a0a 2020 2020 2020  d", "t"):.      
-00017b10: 2020 2020 2020 2020 2020 736f 7274 5f6b            sort_k
-00017b20: 6579 203d 206c 616d 6264 6120 743a 2066  ey = lambda t: f
-00017b30: 6c6f 6174 2874 5b2d 325d 2920 2f20 666c  loat(t[-2]) / fl
-00017b40: 6f61 7428 745b 2d31 5d29 0a20 2020 2020  oat(t[-1]).     
-00017b50: 2020 2020 2020 206c 696e 6573 2e73 6f72         lines.sor
-00017b60: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
-00017b70: 2020 206b 6579 3d73 6f72 745f 6b65 792c     key=sort_key,
-00017b80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017b90: 2072 6576 6572 7365 3d6e 6f74 2072 6576   reverse=not rev
-00017ba0: 6572 7365 5f2c 0a20 2020 2020 2020 2020  erse_,.         
-00017bb0: 2020 2029 0a20 2020 2020 2020 2065 6c73     ).        els
-00017bc0: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
-00017bd0: 6620 6e6f 7420 7265 7665 7273 655f 3a0a  f not reverse_:.
-00017be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017bf0: 6c69 6e65 732e 7265 7665 7273 6528 290a  lines.reverse().
-00017c00: 0a20 2020 2020 2020 2066 6f72 2064 6574  .        for det
-00017c10: 6169 6c73 2069 6e20 6c69 6e65 733a 0a20  ails in lines:. 
-00017c20: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00017c30: 5f65 6e74 7279 2864 6574 6169 6c73 290a  _entry(details).
-00017c40: 2020 2020 2020 2020 2020 2020 6e75 6d5f              num_
-00017c50: 6c69 6e65 7320 2b3d 2031 0a20 2020 2020  lines += 1.     
-00017c60: 2020 2020 2020 206e 6f5f 7265 7375 6c74         no_result
-00017c70: 7320 3d20 4661 6c73 650a 2020 2020 2020  s = False.      
-00017c80: 2020 2020 2020 6966 2074 6f70 2069 7320        if top is 
-00017c90: 6e6f 7420 4e6f 6e65 2061 6e64 206e 756d  not None and num
-00017ca0: 5f6c 696e 6573 203d 3d20 746f 703a 0a20  _lines == top:. 
-00017cb0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-00017cc0: 7265 616b 0a0a 2020 2020 6966 206e 6f5f  reak..    if no_
-00017cd0: 7265 7375 6c74 7320 616e 6420 7365 6172  results and sear
-00017ce0: 6368 5f74 6167 733a 0a20 2020 2020 2020  ch_tags:.       
-00017cf0: 2063 6c69 636b 2e73 6563 686f 2822 4e6f   click.secho("No
-00017d00: 2073 6f6e 6773 2066 6f75 6e64 206d 6174   songs found mat
-00017d10: 6368 696e 6720 7461 6773 2e22 2c20 6667  ching tags.", fg
-00017d20: 3d22 7265 6422 290a 2020 2020 656c 6966  ="red").    elif
-00017d30: 206e 6f5f 7265 7375 6c74 733a 0a20 2020   no_results:.   
-00017d40: 2020 2020 2063 6c69 636b 2e73 6563 686f       click.secho
-00017d50: 280a 2020 2020 2020 2020 2020 2020 224e  (.            "N
-00017d60: 6f20 736f 6e67 7320 666f 756e 642e 2055  o songs found. U
-00017d70: 7365 2027 6d61 6573 7472 6f20 6164 6427  se 'maestro add'
-00017d80: 2074 6f20 6164 6420 6120 736f 6e67 2e22   to add a song."
-00017d90: 2c20 6667 3d22 7265 6422 0a20 2020 2020  , fg="red".     
-00017da0: 2020 2029 0a0a 0a40 636c 692e 636f 6d6d     )...@cli.comm
-00017db0: 616e 6428 290a 4063 6c69 636b 2e6f 7074  and().@click.opt
-00017dc0: 696f 6e28 0a20 2020 2022 2d79 222c 0a20  ion(.    "-y",. 
-00017dd0: 2020 2022 2d2d 7965 6172 222c 0a20 2020     "--year",.   
-00017de0: 2022 7965 6172 222c 0a20 2020 2068 656c   "year",.    hel
-00017df0: 703d 2253 686f 7720 7469 6d65 206c 6973  p="Show time lis
-00017e00: 7465 6e65 6420 666f 7220 6120 7370 6563  tened for a spec
-00017e10: 6966 6963 2079 6561 722c 2069 6e73 7465  ific year, inste
-00017e20: 6164 206f 6620 7468 6520 746f 7461 6c2e  ad of the total.
-00017e30: 2050 6173 7369 6e67 2027 6375 7227 2077   Passing 'cur' w
-00017e40: 696c 6c20 7368 6f77 2074 6865 2074 696d  ill show the tim
-00017e50: 6520 6c69 7374 656e 6564 2066 6f72 2074  e listened for t
-00017e60: 6865 2063 7572 7265 6e74 2079 6561 722e  he current year.
-00017e70: 222c 0a29 0a40 636c 6963 6b2e 6f70 7469  ",.).@click.opti
-00017e80: 6f6e 280a 2020 2020 222d 492f 2d6e 4922  on(.    "-I/-nI"
-00017e90: 2c0a 2020 2020 222d 2d73 6f6e 672d 696e  ,.    "--song-in
-00017ea0: 666f 2f2d 2d6e 6f2d 736f 6e67 2d69 6e66  fo/--no-song-inf
-00017eb0: 6f22 2c0a 2020 2020 2273 6f6e 675f 696e  o",.    "song_in
-00017ec0: 666f 222c 0a20 2020 2064 6566 6175 6c74  fo",.    default
-00017ed0: 3d46 616c 7365 2c0a 2020 2020 6865 6c70  =False,.    help
-00017ee0: 3d22 5368 6f77 2074 6865 2061 7274 6973  ="Show the artis
-00017ef0: 742c 2061 6c62 756d 2c20 616e 6420 616c  t, album, and al
-00017f00: 6275 6d20 6172 7469 7374 2066 6f72 2065  bum artist for e
-00017f10: 6163 6820 736f 6e67 2e22 2c0a 290a 4063  ach song.",.).@c
-00017f20: 6c69 636b 2e61 7267 756d 656e 7428 2273  lick.argument("s
-00017f30: 6f6e 675f 6964 7322 2c20 7479 7065 3d63  ong_ids", type=c
-00017f40: 6c69 636b 2e49 4e54 2c20 6e61 7267 733d  lick.INT, nargs=
-00017f50: 2d31 2c20 7265 7175 6972 6564 3d54 7275  -1, required=Tru
-00017f60: 6529 0a64 6566 2065 6e74 7279 2873 6f6e  e).def entry(son
-00017f70: 675f 6964 732c 2079 6561 722c 2073 6f6e  g_ids, year, son
-00017f80: 675f 696e 666f 293a 0a20 2020 2022 2222  g_info):.    """
-00017f90: 0a20 2020 2056 6965 7720 7468 6520 6465  .    View the de
-00017fa0: 7461 696c 7320 666f 7220 7370 6563 6966  tails for specif
-00017fb0: 6963 2073 6f6e 6728 7329 2e0a 0a20 2020  ic song(s)...   
-00017fc0: 2050 7269 6e74 7320 7468 6520 6465 7461   Prints the deta
-00017fd0: 696c 7320 6f66 2074 6865 2073 6f6e 6728  ils of the song(
-00017fe0: 7329 2077 6974 6820 7468 6520 4944 2873  s) with the ID(s
-00017ff0: 2920 534f 4e47 5f49 4453 2e0a 0a20 2020  ) SONG_IDS...   
-00018000: 205c 620a 2020 2020 4f75 7470 7574 2066   \b.    Output f
-00018010: 6f72 6d61 743a 0a20 2020 2020 2020 2049  ormat:.        I
-00018020: 442c 206e 616d 652c 2064 7572 6174 696f  D, name, duratio
-00018030: 6e2c 206c 6973 7465 6e20 7469 6d65 2c20  n, listen time, 
-00018040: 7469 6d65 7320 6c69 7374 656e 6564 2c20  times listened, 
-00018050: 5b63 6c69 702d 7374 6172 742c 2063 6c69  [clip-start, cli
-00018060: 702d 656e 645d 2069 6620 636c 6970 2065  p-end] if clip e
-00018070: 7869 7374 732c 2063 6f6d 6d61 2d73 6570  xists, comma-sep
-00018080: 6172 6174 6564 2074 6167 7320 6966 2061  arated tags if a
-00018090: 6e79 0a20 2020 2020 2020 2061 7274 6973  ny.        artis
-000180a0: 7420 2d20 616c 6275 6d20 2861 6c62 756d  t - album (album
-000180b0: 2061 7274 6973 7429 2069 6620 2d49 2f2d   artist) if -I/-
-000180c0: 2d73 6f6e 672d 696e 666f 2069 7320 7061  -song-info is pa
-000180d0: 7373 6564 0a20 2020 2022 2222 0a20 2020  ssed.    """.   
-000180e0: 2073 6f6e 675f 6964 7320 3d20 7365 7428   song_ids = set(
-000180f0: 736f 6e67 5f69 6473 290a 0a20 2020 2069  song_ids)..    i
-00018100: 6620 7965 6172 2069 7320 4e6f 6e65 3a0a  f year is None:.
-00018110: 2020 2020 2020 2020 7374 6174 735f 7061          stats_pa
-00018120: 7468 203d 2054 4f54 414c 5f53 5441 5453  th = TOTAL_STATS
-00018130: 5f50 4154 480a 2020 2020 656c 7365 3a0a  _PATH.    else:.
-00018140: 2020 2020 2020 2020 6966 2079 6561 7220          if year 
-00018150: 3d3d 2022 6375 7222 3a0a 2020 2020 2020  == "cur":.      
-00018160: 2020 2020 2020 7965 6172 203d 2043 5552        year = CUR
-00018170: 5f59 4541 520a 2020 2020 2020 2020 2020  _YEAR.          
-00018180: 2020 7374 6174 735f 7061 7468 203d 2043    stats_path = C
-00018190: 5552 5f59 4541 525f 5354 4154 535f 5041  UR_YEAR_STATS_PA
-000181a0: 5448 0a20 2020 2020 2020 2065 6c73 653a  TH.        else:
-000181b0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000181c0: 6e6f 7420 7965 6172 2e69 7364 6967 6974  not year.isdigit
-000181d0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-000181e0: 2020 2020 636c 6963 6b2e 7365 6368 6f28      click.secho(
-000181f0: 2259 6561 7220 6d75 7374 2062 6520 6120  "Year must be a 
-00018200: 6e75 6d62 6572 2e22 2c20 6667 3d22 7265  number.", fg="re
-00018210: 6422 290a 2020 2020 2020 2020 2020 2020  d").            
-00018220: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-00018230: 2020 2020 2020 2073 7461 7473 5f70 6174         stats_pat
-00018240: 6820 3d20 6f73 2e70 6174 682e 6a6f 696e  h = os.path.join
-00018250: 2853 5441 5453 5f44 4952 2c20 6622 7b79  (STATS_DIR, f"{y
-00018260: 6561 727d 2e74 7874 2229 0a0a 2020 2020  ear}.txt")..    
-00018270: 7472 793a 0a20 2020 2020 2020 2077 6974  try:.        wit
-00018280: 6820 280a 2020 2020 2020 2020 2020 2020  h (.            
-00018290: 6f70 656e 2853 4f4e 4753 5f49 4e46 4f5f  open(SONGS_INFO_
-000182a0: 5041 5448 2c20 2272 222c 2065 6e63 6f64  PATH, "r", encod
-000182b0: 696e 673d 2275 7466 2d38 2229 2061 7320  ing="utf-8") as 
-000182c0: 736f 6e67 735f 6669 6c65 2c0a 2020 2020  songs_file,.    
-000182d0: 2020 2020 2020 2020 6f70 656e 2873 7461          open(sta
-000182e0: 7473 5f70 6174 682c 2022 7222 2c20 656e  ts_path, "r", en
-000182f0: 636f 6469 6e67 3d22 7574 662d 3822 2920  coding="utf-8") 
-00018300: 6173 2073 7461 7473 5f66 696c 652c 0a20  as stats_file,. 
-00018310: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
-00018320: 2020 2020 2020 6c69 6e65 7320 3d20 736f        lines = so
-00018330: 6e67 735f 6669 6c65 2e72 6561 646c 696e  ngs_file.readlin
-00018340: 6573 2829 0a20 2020 2020 2020 2020 2020  es().           
-00018350: 2073 7461 7473 203d 2064 6963 7428 0a20   stats = dict(. 
-00018360: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00018370: 6170 280a 2020 2020 2020 2020 2020 2020  ap(.            
-00018380: 2020 2020 2020 2020 6c61 6d62 6461 2074          lambda t
-00018390: 3a20 2869 6e74 2874 5b30 5d29 2c29 202b  : (int(t[0]),) +
-000183a0: 2074 5b31 3a5d 2c20 2023 2063 6f6e 7665   t[1:],  # conve
-000183b0: 7274 206b 6579 2074 6f20 696e 740a 2020  rt key to int.  
-000183c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000183d0: 2020 6d61 7028 0a20 2020 2020 2020 2020    map(.         
-000183e0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-000183f0: 616d 6264 6120 783a 2074 7570 6c65 286d  ambda x: tuple(m
-00018400: 6170 2866 6c6f 6174 2c20 782e 7374 7269  ap(float, x.stri
-00018410: 7028 292e 7370 6c69 7428 227c 2229 2929  p().split("|")))
-00018420: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00018430: 2020 2020 2020 2020 2020 7374 6174 735f            stats_
-00018440: 6669 6c65 2e72 6561 646c 696e 6573 2829  file.readlines()
-00018450: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00018460: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
-00018470: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00018480: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00018490: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
-000184a0: 6e67 6528 6c65 6e28 6c69 6e65 7329 293a  nge(len(lines)):
-000184b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000184c0: 2064 6574 6169 6c73 203d 206c 696e 6573   details = lines
-000184d0: 5b69 5d2e 7374 7269 7028 292e 7370 6c69  [i].strip().spli
-000184e0: 7428 227c 2229 0a20 2020 2020 2020 2020  t("|").         
-000184f0: 2020 2020 2020 2073 6f6e 675f 6964 203d         song_id =
-00018500: 2069 6e74 2864 6574 6169 6c73 5b30 5d29   int(details[0])
-00018510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018520: 2069 6620 736f 6e67 5f69 6420 696e 2073   if song_id in s
-00018530: 6f6e 675f 6964 733a 0a20 2020 2020 2020  ong_ids:.       
-00018540: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-00018550: 6e74 5f65 6e74 7279 280a 2020 2020 2020  nt_entry(.      
-00018560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018570: 2020 6465 7461 696c 730a 2020 2020 2020    details.      
-00018580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018590: 2020 2b20 5b0a 2020 2020 2020 2020 2020    + [.          
-000185a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000185b0: 2020 7374 6174 735b 736f 6e67 5f69 645d    stats[song_id]
-000185c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000185d0: 2020 2020 2020 2020 2020 2020 2020 6d75                mu
-000185e0: 7369 635f 7461 672e 6c6f 6164 5f66 696c  sic_tag.load_fil
-000185f0: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
-00018600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018610: 2020 206f 732e 7061 7468 2e6a 6f69 6e28     os.path.join(
-00018620: 534f 4e47 535f 4449 522c 2064 6574 6169  SONGS_DIR, detai
-00018630: 6c73 5b31 5d29 0a20 2020 2020 2020 2020  ls[1]).         
-00018640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018650: 2020 2029 5b22 236c 656e 6774 6822 5d2e     )["#length"].
-00018660: 7661 6c75 652c 0a20 2020 2020 2020 2020  value,.         
-00018670: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
-00018680: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00018690: 2020 2020 2020 2020 2020 7368 6f77 5f73            show_s
-000186a0: 6f6e 675f 696e 666f 3d73 6f6e 675f 696e  ong_info=song_in
-000186b0: 666f 2c0a 2020 2020 2020 2020 2020 2020  fo,.            
-000186c0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-000186d0: 2020 2020 2020 2020 2020 2020 2020 736f                so
-000186e0: 6e67 5f69 6473 2e72 656d 6f76 6528 736f  ng_ids.remove(so
-000186f0: 6e67 5f69 6429 0a20 2020 2065 7863 6570  ng_id).    excep
-00018700: 7420 4669 6c65 4e6f 7446 6f75 6e64 4572  t FileNotFoundEr
-00018710: 726f 723a 0a20 2020 2020 2020 2063 6c69  ror:.        cli
-00018720: 636b 2e73 6563 686f 2866 224e 6f20 7374  ck.secho(f"No st
-00018730: 6174 7320 666f 756e 6420 666f 7220 7965  ats found for ye
-00018740: 6172 207b 7965 6172 7d2e 222c 2066 673d  ar {year}.", fg=
-00018750: 2272 6564 2229 0a0a 2020 2020 6966 2073  "red")..    if s
-00018760: 6f6e 675f 6964 733a 0a20 2020 2020 2020  ong_ids:.       
-00018770: 2073 6f6e 675f 6964 7320 3d20 5b73 7472   song_ids = [str
-00018780: 2869 645f 2920 666f 7220 6964 5f20 696e  (id_) for id_ in
-00018790: 2073 6f6e 675f 6964 735d 0a20 2020 2020   song_ids].     
-000187a0: 2020 2063 6c69 636b 2e73 6563 686f 280a     click.secho(.
-000187b0: 2020 2020 2020 2020 2020 2020 6622 4e6f              f"No
-000187c0: 2073 6f6e 6773 2066 6f75 6e64 2077 6974   songs found wit
-000187d0: 6820 4944 733a 207b 272c 2027 2e6a 6f69  h IDs: {', '.joi
-000187e0: 6e28 736f 6e67 5f69 6473 297d 2e22 2c20  n(song_ids)}.", 
-000187f0: 6667 3d22 7265 6422 0a20 2020 2020 2020  fg="red".       
-00018800: 2029 0a0a 0a40 636c 692e 636f 6d6d 616e   )...@cli.comman
-00018810: 6428 290a 4063 6c69 636b 2e61 7267 756d  d().@click.argum
-00018820: 656e 7428 2273 6f6e 6722 2c20 7265 7175  ent("song", requ
-00018830: 6972 6564 3d54 7275 6529 0a40 636c 6963  ired=True).@clic
-00018840: 6b2e 6f70 7469 6f6e 280a 2020 2020 222d  k.option(.    "-
-00018850: 4e2f 2d6e 4e22 2c0a 2020 2020 222d 2d6e  N/-nN",.    "--n
-00018860: 616d 652f 2d2d 6e6f 2d6e 616d 6522 2c0a  ame/--no-name",.
-00018870: 2020 2020 2274 6974 6c65 222c 0a20 2020      "title",.   
-00018880: 2064 6566 6175 6c74 3d46 616c 7365 2c0a   default=False,.
-00018890: 2020 2020 6865 6c70 3d22 5472 6561 7420      help="Treat 
-000188a0: 534f 4e47 2061 7320 6120 736f 6e67 206e  SONG as a song n
-000188b0: 616d 6520 696e 7374 6561 6420 6f66 2061  ame instead of a
-000188c0: 6e20 4944 2e22 2c0a 290a 6465 6620 7265  n ID.",.).def re
-000188d0: 636f 6d6d 656e 6428 736f 6e67 2c20 7469  commend(song, ti
-000188e0: 746c 6529 3a0a 2020 2020 2222 220a 2020  tle):.    """.  
-000188f0: 2020 4765 7420 7265 636f 6d6d 656e 6461    Get recommenda
-00018900: 7469 6f6e 7320 6672 6f6d 2059 5420 4d75  tions from YT Mu
-00018910: 7369 6320 6261 7365 6420 6f6e 2073 6f6e  sic based on son
-00018920: 6720 7469 746c 6573 2e20 4e6f 7465 3a20  g titles. Note: 
-00018930: 7468 6973 2066 6561 7475 7265 0a20 2020  this feature.   
-00018940: 2069 7320 6578 7065 7269 6d65 6e74 616c   is experimental
-00018950: 2e0a 0a20 2020 2052 6563 6f6d 6d65 6e64  ...    Recommend
-00018960: 7320 736f 6e67 7320 2870 6f73 7369 626c  s songs (possibl
-00018970: 7920 6578 706c 6963 6974 2920 7573 696e  y explicit) usin
-00018980: 6720 7468 6520 596f 7554 7562 6520 4d75  g the YouTube Mu
-00018990: 7369 6320 4150 4920 7369 6d69 6c61 720a  sic API similar.
-000189a0: 2020 2020 746f 2074 6865 2073 6f6e 6720      to the song 
-000189b0: 7769 7468 2049 4420 534f 4e47 2074 6f20  with ID SONG to 
-000189c0: 6c69 7374 656e 2074 6f2e 0a0a 2020 2020  listen to...    
-000189d0: 4966 2074 6865 2027 2d4e 2720 666c 6167  If the '-N' flag
-000189e0: 2069 7320 7061 7373 6564 2c20 534f 4e47   is passed, SONG
-000189f0: 2069 7320 7472 6561 7465 6420 6173 2061   is treated as a
-00018a00: 2073 6f6e 6720 6e61 6d65 2074 6f20 7365   song name to se
-00018a10: 6172 6368 2066 6f72 0a20 2020 206f 6e20  arch for.    on 
-00018a20: 596f 7554 7562 6520 4d75 7369 632e 2222  YouTube Music.""
-00018a30: 220a 2020 2020 7472 793a 0a20 2020 2020  ".    try:.     
-00018a40: 2020 2066 726f 6d20 7974 6d75 7369 6361     from ytmusica
-00018a50: 7069 2069 6d70 6f72 7420 5954 4d75 7369  pi import YTMusi
-00018a60: 630a 2020 2020 6578 6365 7074 2049 6d70  c.    except Imp
-00018a70: 6f72 7445 7272 6f72 3a0a 2020 2020 2020  ortError:.      
-00018a80: 2020 636c 6963 6b2e 7365 6368 6f28 0a20    click.secho(. 
-00018a90: 2020 2020 2020 2020 2020 2022 5468 6520             "The 
-00018aa0: 2772 6563 6f6d 6d65 6e64 2720 636f 6d6d  'recommend' comm
-00018ab0: 616e 6420 7265 7175 6972 6573 2074 6865  and requires the
-00018ac0: 2027 7974 6d75 7369 6361 7069 2720 7061   'ytmusicapi' pa
-00018ad0: 636b 6167 6520 746f 2062 6520 696e 7374  ckage to be inst
-00018ae0: 616c 6c65 642e 2052 756e 2027 7069 7020  alled. Run 'pip 
-00018af0: 696e 7374 616c 6c20 7974 6d75 7369 6361  install ytmusica
-00018b00: 7069 2720 746f 2069 6e73 7461 6c6c 2069  pi' to install i
-00018b10: 742e 222c 0a20 2020 2020 2020 2020 2020  t.",.           
-00018b20: 2066 673d 2272 6564 222c 0a20 2020 2020   fg="red",.     
-00018b30: 2020 2029 0a20 2020 2020 2020 2072 6574     ).        ret
-00018b40: 7572 6e0a 0a20 2020 2079 746d 7573 6963  urn..    ytmusic
-00018b50: 203d 2059 544d 7573 6963 2829 0a0a 2020   = YTMusic()..  
-00018b60: 2020 6966 2074 6974 6c65 3a0a 2020 2020    if title:.    
-00018b70: 2020 2020 7265 7375 6c74 7320 3d20 7974      results = yt
-00018b80: 6d75 7369 632e 7365 6172 6368 2873 6f6e  music.search(son
-00018b90: 672c 2066 696c 7465 723d 2273 6f6e 6773  g, filter="songs
-00018ba0: 2229 0a20 2020 2065 6c73 653a 0a20 2020  ").    else:.   
-00018bb0: 2020 2020 2069 6620 6e6f 7420 736f 6e67       if not song
-00018bc0: 2e69 7364 6967 6974 2829 3a0a 2020 2020  .isdigit():.    
-00018bd0: 2020 2020 2020 2020 636c 6963 6b2e 7365          click.se
-00018be0: 6368 6f28 0a20 2020 2020 2020 2020 2020  cho(.           
-00018bf0: 2020 2020 2022 536f 6e67 2049 4420 6d75       "Song ID mu
-00018c00: 7374 2062 6520 6120 6e75 6d62 6572 2e20  st be a number. 
-00018c10: 546f 2067 6574 2072 6563 6f6d 6d65 6e64  To get recommend
-00018c20: 6174 696f 6e73 2062 7920 6e61 6d65 2c20  ations by name, 
-00018c30: 7061 7373 2074 6865 2027 2d4e 2f2d 2d6e  pass the '-N/--n
-00018c40: 616d 6527 2066 6c61 672e 222c 0a20 2020  ame' flag.",.   
-00018c50: 2020 2020 2020 2020 2020 2020 2066 673d               fg=
-00018c60: 2272 6564 222c 0a20 2020 2020 2020 2020  "red",.         
-00018c70: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00018c80: 2072 6574 7572 6e0a 0a20 2020 2020 2020   return..       
-00018c90: 2077 6974 6820 6f70 656e 2853 4f4e 4753   with open(SONGS
-00018ca0: 5f49 4e46 4f5f 5041 5448 2c20 2272 222c  _INFO_PATH, "r",
-00018cb0: 2065 6e63 6f64 696e 673d 2275 7466 2d38   encoding="utf-8
-00018cc0: 2229 2061 7320 736f 6e67 735f 6669 6c65  ") as songs_file
-00018cd0: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
-00018ce0: 7220 6c69 6e65 2069 6e20 736f 6e67 735f  r line in songs_
-00018cf0: 6669 6c65 3a0a 2020 2020 2020 2020 2020  file:.          
-00018d00: 2020 2020 2020 6465 7461 696c 7320 3d20        details = 
-00018d10: 6c69 6e65 2e73 7472 6970 2829 2e73 706c  line.strip().spl
-00018d20: 6974 2822 7c22 290a 2020 2020 2020 2020  it("|").        
-00018d30: 2020 2020 2020 2020 6966 2064 6574 6169          if detai
-00018d40: 6c73 5b30 5d20 3d3d 2073 6f6e 673a 0a20  ls[0] == song:. 
+000116b0: 6622 4172 6520 796f 7520 7375 7265 2079  f"Are you sure y
+000116c0: 6f75 2077 616e 7420 746f 2064 656c 6574  ou want to delet
+000116d0: 6520 7b6c 656e 2873 6f6e 675f 6964 7329  e {len(song_ids)
+000116e0: 7d20 736f 6e67 2873 293f 205b 792f 6e5d  } song(s)? [y/n]
+000116f0: 2022 0a20 2020 2020 2020 2020 2020 2029   ".            )
+00011700: 0a0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00011710: 2063 6861 722e 6c6f 7765 7228 2920 213d   char.lower() !=
+00011720: 2022 7922 3a0a 2020 2020 2020 2020 2020   "y":.          
+00011730: 2020 2020 2020 7072 696e 7428 2244 6964        print("Did
+00011740: 206e 6f74 2064 656c 6574 652e 2229 0a20   not delete."). 
+00011750: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00011760: 6574 7572 6e0a 0a20 2020 2020 2020 2077  eturn..        w
+00011770: 6974 6820 6f70 656e 2853 4f4e 4753 5f49  ith open(SONGS_I
+00011780: 4e46 4f5f 5041 5448 2c20 2272 222c 2065  NFO_PATH, "r", e
+00011790: 6e63 6f64 696e 673d 2275 7466 2d38 2229  ncoding="utf-8")
+000117a0: 2061 7320 736f 6e67 735f 6669 6c65 3a0a   as songs_file:.
+000117b0: 2020 2020 2020 2020 2020 2020 6c69 6e65              line
+000117c0: 7320 3d20 736f 6e67 735f 6669 6c65 2e72  s = songs_file.r
+000117d0: 6561 6428 292e 7370 6c69 746c 696e 6573  ead().splitlines
+000117e0: 2829 0a0a 2020 2020 2020 2020 2020 2020  ()..            
+000117f0: 746f 5f62 655f 6465 6c65 7465 6420 3d20  to_be_deleted = 
+00011800: 5b5d 0a20 2020 2020 2020 2020 2020 2066  [].            f
+00011810: 6f72 2069 2069 6e20 7261 6e67 6528 6c65  or i in range(le
+00011820: 6e28 6c69 6e65 7329 293a 0a20 2020 2020  n(lines)):.     
+00011830: 2020 2020 2020 2020 2020 2064 6574 6169             detai
+00011840: 6c73 203d 206c 696e 6573 5b69 5d2e 7374  ls = lines[i].st
+00011850: 7269 7028 292e 7370 6c69 7428 227c 2229  rip().split("|")
+00011860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011870: 2073 6f6e 675f 6964 203d 2069 6e74 2864   song_id = int(d
+00011880: 6574 6169 6c73 5b30 5d29 0a20 2020 2020  etails[0]).     
+00011890: 2020 2020 2020 2020 2020 2069 6620 736f             if so
+000118a0: 6e67 5f69 6420 696e 2072 656d 6169 6e69  ng_id in remaini
+000118b0: 6e67 5f73 6f6e 675f 6964 733a 0a20 2020  ng_song_ids:.   
+000118c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000118d0: 2072 656d 6169 6e69 6e67 5f73 6f6e 675f   remaining_song_
+000118e0: 6964 732e 7265 6d6f 7665 2873 6f6e 675f  ids.remove(song_
+000118f0: 6964 290a 2020 2020 2020 2020 2020 2020  id).            
+00011900: 2020 2020 2020 2020 746f 5f62 655f 6465          to_be_de
+00011910: 6c65 7465 642e 6170 7065 6e64 2869 290a  leted.append(i).
+00011920: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011930: 2020 2020 2073 6f6e 675f 6e61 6d65 203d       song_name =
+00011940: 2064 6574 6169 6c73 5b31 5d0a 2020 2020   details[1].    
+00011950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011960: 6f73 2e72 656d 6f76 6528 2020 2320 7265  os.remove(  # re
+00011970: 6d6f 7665 2061 6374 7561 6c20 736f 6e67  move actual song
+00011980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011990: 2020 2020 2020 2020 206f 732e 7061 7468           os.path
+000119a0: 2e6a 6f69 6e28 534f 4e47 535f 4449 522c  .join(SONGS_DIR,
+000119b0: 2073 6f6e 675f 6e61 6d65 290a 2020 2020   song_name).    
+000119c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000119d0: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
+000119e0: 2020 2020 2020 2063 6c69 636b 2e73 6563         click.sec
+000119f0: 686f 280a 2020 2020 2020 2020 2020 2020  ho(.            
+00011a00: 2020 2020 2020 2020 2020 2020 6622 5265              f"Re
+00011a10: 6d6f 7665 6420 736f 6e67 2027 7b73 6f6e  moved song '{son
+00011a20: 675f 6e61 6d65 7d27 2077 6974 6820 4944  g_name}' with ID
+00011a30: 207b 736f 6e67 5f69 647d 2e22 2c0a 2020   {song_id}.",.  
+00011a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a50: 2020 2020 2020 6667 3d22 6772 6565 6e22        fg="green"
+00011a60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00011a70: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00011a80: 2066 6f72 2069 2069 6e20 7265 7665 7273   for i in revers
+00011a90: 6564 2874 6f5f 6265 5f64 656c 6574 6564  ed(to_be_deleted
+00011aa0: 293a 0a20 2020 2020 2020 2020 2020 2064  ):.            d
+00011ab0: 656c 206c 696e 6573 5b69 5d0a 0a20 2020  el lines[i]..   
+00011ac0: 2020 2020 2077 6974 6820 6f70 656e 2853       with open(S
+00011ad0: 4f4e 4753 5f49 4e46 4f5f 5041 5448 2c20  ONGS_INFO_PATH, 
+00011ae0: 2277 222c 2065 6e63 6f64 696e 673d 2275  "w", encoding="u
+00011af0: 7466 2d38 2229 2061 7320 736f 6e67 735f  tf-8") as songs_
+00011b00: 6669 6c65 3a0a 2020 2020 2020 2020 2020  file:.          
+00011b10: 2020 736f 6e67 735f 6669 6c65 2e77 7269    songs_file.wri
+00011b20: 7465 2822 5c6e 222e 6a6f 696e 286c 696e  te("\n".join(lin
+00011b30: 6573 2929 0a0a 2020 2020 2020 2020 666f  es))..        fo
+00011b40: 7220 7374 6174 735f 6669 6c65 2069 6e20  r stats_file in 
+00011b50: 6f73 2e6c 6973 7464 6972 2853 5441 5453  os.listdir(STATS
+00011b60: 5f44 4952 293a 0a20 2020 2020 2020 2020  _DIR):.         
+00011b70: 2020 2069 6620 6e6f 7420 7374 6174 735f     if not stats_
+00011b80: 6669 6c65 2e65 6e64 7377 6974 6828 222e  file.endswith(".
+00011b90: 7478 7422 293a 0a20 2020 2020 2020 2020  txt"):.         
+00011ba0: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
+00011bb0: 0a20 2020 2020 2020 2020 2020 2073 7461  .            sta
+00011bc0: 7473 5f70 6174 6820 3d20 6f73 2e70 6174  ts_path = os.pat
+00011bd0: 682e 6a6f 696e 2853 5441 5453 5f44 4952  h.join(STATS_DIR
+00011be0: 2c20 7374 6174 735f 6669 6c65 290a 2020  , stats_file).  
+00011bf0: 2020 2020 2020 2020 2020 7769 7468 206f            with o
+00011c00: 7065 6e28 7374 6174 735f 7061 7468 2c20  pen(stats_path, 
+00011c10: 2272 222c 2065 6e63 6f64 696e 673d 2275  "r", encoding="u
+00011c20: 7466 2d38 2229 2061 7320 7374 6174 735f  tf-8") as stats_
+00011c30: 6669 6c65 3a0a 2020 2020 2020 2020 2020  file:.          
+00011c40: 2020 2020 2020 7374 6174 735f 6c69 6e65        stats_line
+00011c50: 7320 3d20 7374 6174 735f 6669 6c65 2e72  s = stats_file.r
+00011c60: 6561 6428 292e 7370 6c69 746c 696e 6573  ead().splitlines
+00011c70: 2829 0a0a 2020 2020 2020 2020 2020 2020  ()..            
+00011c80: 2020 2020 746f 5f62 655f 6465 6c65 7465      to_be_delete
+00011c90: 6420 3d20 5b5d 0a20 2020 2020 2020 2020  d = [].         
+00011ca0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+00011cb0: 7261 6e67 6528 6c65 6e28 7374 6174 735f  range(len(stats_
+00011cc0: 6c69 6e65 7329 293a 0a20 2020 2020 2020  lines)):.       
+00011cd0: 2020 2020 2020 2020 2020 2020 2064 6574               det
+00011ce0: 6169 6c73 203d 2073 7461 7473 5f6c 696e  ails = stats_lin
+00011cf0: 6573 5b69 5d2e 7374 7269 7028 292e 7370  es[i].strip().sp
+00011d00: 6c69 7428 227c 2229 0a20 2020 2020 2020  lit("|").       
+00011d10: 2020 2020 2020 2020 2020 2020 2073 6f6e               son
+00011d20: 675f 6964 203d 2069 6e74 2864 6574 6169  g_id = int(detai
+00011d30: 6c73 5b30 5d29 0a20 2020 2020 2020 2020  ls[0]).         
+00011d40: 2020 2020 2020 2020 2020 2069 6620 736f             if so
+00011d50: 6e67 5f69 6420 696e 2073 6f6e 675f 6964  ng_id in song_id
+00011d60: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+00011d70: 2020 2020 2020 2020 2020 2074 6f5f 6265             to_be
+00011d80: 5f64 656c 6574 6564 2e61 7070 656e 6428  _deleted.append(
+00011d90: 6929 0a0a 2020 2020 2020 2020 2020 2020  i)..            
+00011da0: 666f 7220 6920 696e 2072 6576 6572 7365  for i in reverse
+00011db0: 6428 746f 5f62 655f 6465 6c65 7465 6429  d(to_be_deleted)
+00011dc0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00011dd0: 2020 6465 6c20 7374 6174 735f 6c69 6e65    del stats_line
+00011de0: 735b 695d 0a0a 2020 2020 2020 2020 2020  s[i]..          
+00011df0: 2020 7769 7468 206f 7065 6e28 7374 6174    with open(stat
+00011e00: 735f 7061 7468 2c20 2277 222c 2065 6e63  s_path, "w", enc
+00011e10: 6f64 696e 673d 2275 7466 2d38 2229 2061  oding="utf-8") a
+00011e20: 7320 7374 6174 735f 6669 6c65 3a0a 2020  s stats_file:.  
+00011e30: 2020 2020 2020 2020 2020 2020 2020 7374                st
+00011e40: 6174 735f 6669 6c65 2e77 7269 7465 2822  ats_file.write("
+00011e50: 5c6e 222e 6a6f 696e 2873 7461 7473 5f6c  \n".join(stats_l
+00011e60: 696e 6573 2929 0a0a 2020 2020 2020 2020  ines))..        
+00011e70: 6966 2072 656d 6169 6e69 6e67 5f73 6f6e  if remaining_son
+00011e80: 675f 6964 733a 0a20 2020 2020 2020 2020  g_ids:.         
+00011e90: 2020 2063 6c69 636b 2e73 6563 686f 280a     click.secho(.
+00011ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011eb0: 6622 436f 756c 6420 6e6f 7420 6669 6e64  f"Could not find
+00011ec0: 2074 6865 2066 6f6c 6c6f 7769 6e67 2073   the following s
+00011ed0: 6f6e 6720 4944 733a 207b 272c 2027 2e6a  ong IDs: {', '.j
+00011ee0: 6f69 6e28 6d61 7028 7374 722c 2072 656d  oin(map(str, rem
+00011ef0: 6169 6e69 6e67 5f73 6f6e 675f 6964 7329  aining_song_ids)
+00011f00: 297d 2e22 2c0a 2020 2020 2020 2020 2020  )}.",.          
+00011f10: 2020 2020 2020 6667 3d22 7265 6422 2c0a        fg="red",.
+00011f20: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00011f30: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00011f40: 7461 6773 5f74 6f5f 7265 6d6f 7665 203d  tags_to_remove =
+00011f50: 2073 6574 2861 7267 7329 0a20 2020 2020   set(args).     
+00011f60: 2020 2069 6620 6e6f 7420 666f 7263 653a     if not force:
+00011f70: 0a20 2020 2020 2020 2020 2020 2063 6861  .            cha
+00011f80: 7220 3d20 696e 7075 7428 0a20 2020 2020  r = input(.     
+00011f90: 2020 2020 2020 2020 2020 2066 2241 7265             f"Are
+00011fa0: 2079 6f75 2073 7572 6520 796f 7520 7761   you sure you wa
+00011fb0: 6e74 2074 6f20 6465 6c65 7465 207b 6c65  nt to delete {le
+00011fc0: 6e28 7461 6773 5f74 6f5f 7265 6d6f 7665  n(tags_to_remove
+00011fd0: 297d 2074 6167 2873 293f 205b 792f 6e5d  )} tag(s)? [y/n]
+00011fe0: 2022 0a20 2020 2020 2020 2020 2020 2029   ".            )
+00011ff0: 0a0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00012000: 2063 6861 722e 6c6f 7765 7228 2920 213d   char.lower() !=
+00012010: 2022 7922 3a0a 2020 2020 2020 2020 2020   "y":.          
+00012020: 2020 2020 2020 7072 696e 7428 2244 6964        print("Did
+00012030: 206e 6f74 2064 656c 6574 652e 2229 0a20   not delete."). 
+00012040: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00012050: 6574 7572 6e0a 0a20 2020 2020 2020 2077  eturn..        w
+00012060: 6974 6820 6f70 656e 2853 4f4e 4753 5f49  ith open(SONGS_I
+00012070: 4e46 4f5f 5041 5448 2c20 2272 222c 2065  NFO_PATH, "r", e
+00012080: 6e63 6f64 696e 673d 2275 7466 2d38 2229  ncoding="utf-8")
+00012090: 2061 7320 736f 6e67 735f 6669 6c65 3a0a   as songs_file:.
+000120a0: 2020 2020 2020 2020 2020 2020 6c69 6e65              line
+000120b0: 7320 3d20 736f 6e67 735f 6669 6c65 2e72  s = songs_file.r
+000120c0: 6561 6428 292e 7370 6c69 746c 696e 6573  ead().splitlines
+000120d0: 2829 0a20 2020 2020 2020 2020 2020 2066  ().            f
+000120e0: 6f72 2069 2069 6e20 7261 6e67 6528 6c65  or i in range(le
+000120f0: 6e28 6c69 6e65 7329 293a 0a20 2020 2020  n(lines)):.     
+00012100: 2020 2020 2020 2020 2020 2064 6574 6169             detai
+00012110: 6c73 203d 206c 696e 6573 5b69 5d2e 7374  ls = lines[i].st
+00012120: 7269 7028 292e 7370 6c69 7428 227c 2229  rip().split("|")
+00012130: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012140: 2074 6167 7320 3d20 6465 7461 696c 735b   tags = details[
+00012150: 325d 2e73 706c 6974 2822 2c22 290a 2020  2].split(",").  
+00012160: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00012170: 7220 6a20 696e 2072 616e 6765 286c 656e  r j in range(len
+00012180: 2874 6167 7329 293a 0a20 2020 2020 2020  (tags)):.       
+00012190: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000121a0: 7461 6773 5b6a 5d20 696e 2074 6167 735f  tags[j] in tags_
+000121b0: 746f 5f72 656d 6f76 653a 0a20 2020 2020  to_remove:.     
+000121c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000121d0: 2020 2064 656c 2074 6167 735b 6a5d 0a20     del tags[j]. 
+000121e0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+000121f0: 6574 6169 6c73 5b32 5d20 3d20 222c 222e  etails[2] = ",".
+00012200: 6a6f 696e 2874 6167 7329 0a20 2020 2020  join(tags).     
+00012210: 2020 2020 2020 2020 2020 206c 696e 6573             lines
+00012220: 5b69 5d20 3d20 227c 222e 6a6f 696e 2864  [i] = "|".join(d
+00012230: 6574 6169 6c73 290a 0a20 2020 2020 2020  etails)..       
+00012240: 2077 6974 6820 6f70 656e 2853 4f4e 4753   with open(SONGS
+00012250: 5f49 4e46 4f5f 5041 5448 2c20 2277 222c  _INFO_PATH, "w",
+00012260: 2065 6e63 6f64 696e 673d 2275 7466 2d38   encoding="utf-8
+00012270: 2229 2061 7320 736f 6e67 735f 6669 6c65  ") as songs_file
+00012280: 3a0a 2020 2020 2020 2020 2020 2020 736f  :.            so
+00012290: 6e67 735f 6669 6c65 2e77 7269 7465 2822  ngs_file.write("
+000122a0: 5c6e 222e 6a6f 696e 286c 696e 6573 2929  \n".join(lines))
+000122b0: 0a0a 2020 2020 2020 2020 636c 6963 6b2e  ..        click.
+000122c0: 7365 6368 6f28 0a20 2020 2020 2020 2020  secho(.         
+000122d0: 2020 2066 2244 656c 6574 6564 2061 6c6c     f"Deleted all
+000122e0: 206f 6363 7572 7265 6e63 6573 206f 6620   occurrences of 
+000122f0: 7b6c 656e 2874 6167 735f 746f 5f72 656d  {len(tags_to_rem
+00012300: 6f76 6529 7d20 7461 6728 7329 2e22 2c0a  ove)} tag(s).",.
+00012310: 2020 2020 2020 2020 2020 2020 6667 3d22              fg="
+00012320: 6772 6565 6e22 2c0a 2020 2020 2020 2020  green",.        
+00012330: 290a 0a0a 4063 6c69 2e63 6f6d 6d61 6e64  )...@cli.command
+00012340: 286e 616d 653d 2274 6167 2229 0a40 636c  (name="tag").@cl
+00012350: 6963 6b2e 6172 6775 6d65 6e74 2822 736f  ick.argument("so
+00012360: 6e67 5f69 6473 222c 2074 7970 653d 636c  ng_ids", type=cl
+00012370: 6963 6b2e 494e 542c 2072 6571 7569 7265  ick.INT, require
+00012380: 643d 5472 7565 2c20 6e61 7267 733d 2d31  d=True, nargs=-1
+00012390: 290a 4063 6c69 636b 2e6f 7074 696f 6e28  ).@click.option(
+000123a0: 0a20 2020 2022 2d74 222c 0a20 2020 2022  .    "-t",.    "
+000123b0: 2d2d 7461 6722 2c0a 2020 2020 2274 6167  --tag",.    "tag
+000123c0: 7322 2c0a 2020 2020 6865 6c70 3d22 5461  s",.    help="Ta
+000123d0: 6773 2074 6f20 6164 642e 222c 0a20 2020  gs to add.",.   
+000123e0: 206d 756c 7469 706c 653d 5472 7565 2c0a   multiple=True,.
+000123f0: 290a 6465 6620 7461 675f 2873 6f6e 675f  ).def tag_(song_
+00012400: 6964 732c 2074 6167 7329 3a0a 2020 2020  ids, tags):.    
+00012410: 2222 2241 6464 2074 6167 7320 746f 2061  """Add tags to a
+00012420: 2073 6f6e 6720 2870 6173 7365 6420 6173   song (passed as
+00012430: 2049 4429 2e20 5461 6773 2063 616e 6e6f   ID). Tags canno
+00012440: 7420 636f 6e74 6169 6e20 7468 6520 6368  t contain the ch
+00012450: 6172 6163 7465 7273 0a20 2020 2027 2c27  aracters.    ','
+00012460: 206f 7220 277c 272e 2222 220a 2020 2020   or '|'.""".    
+00012470: 736f 6e67 5f69 6473 203d 2073 6574 2873  song_ids = set(s
+00012480: 6f6e 675f 6964 7329 0a20 2020 206e 756d  ong_ids).    num
+00012490: 5f73 6f6e 6773 203d 206c 656e 2873 6f6e  _songs = len(son
+000124a0: 675f 6964 7329 0a20 2020 2074 6167 7320  g_ids).    tags 
+000124b0: 3d20 7365 7428 7461 6773 290a 2020 2020  = set(tags).    
+000124c0: 666f 7220 7461 6720 696e 2074 6167 733a  for tag in tags:
+000124d0: 0a20 2020 2020 2020 2069 6620 222c 2220  .        if "," 
+000124e0: 696e 2074 6167 206f 7220 227c 2220 696e  in tag or "|" in
+000124f0: 2074 6167 3a0a 2020 2020 2020 2020 2020   tag:.          
+00012500: 2020 636c 6963 6b2e 7365 6368 6f28 2254    click.secho("T
+00012510: 6167 7320 6361 6e6e 6f74 2063 6f6e 7461  ags cannot conta
+00012520: 696e 2027 2c27 206f 7220 277c 272e 222c  in ',' or '|'.",
+00012530: 2066 673d 2272 6564 2229 0a20 2020 2020   fg="red").     
+00012540: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+00012550: 2020 6966 2074 6167 733a 0a20 2020 2020    if tags:.     
+00012560: 2020 2073 6f6e 6773 5f66 696c 6520 3d20     songs_file = 
+00012570: 6f70 656e 2853 4f4e 4753 5f49 4e46 4f5f  open(SONGS_INFO_
+00012580: 5041 5448 2c20 2272 222c 2065 6e63 6f64  PATH, "r", encod
+00012590: 696e 673d 2275 7466 2d38 2229 0a20 2020  ing="utf-8").   
+000125a0: 2020 2020 206c 696e 6573 203d 2073 6f6e       lines = son
+000125b0: 6773 5f66 696c 652e 7265 6164 2829 2e73  gs_file.read().s
+000125c0: 706c 6974 6c69 6e65 7328 290a 2020 2020  plitlines().    
+000125d0: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+000125e0: 6765 286c 656e 286c 696e 6573 2929 3a0a  ge(len(lines)):.
+000125f0: 2020 2020 2020 2020 2020 2020 6465 7461              deta
+00012600: 696c 7320 3d20 6c69 6e65 735b 695d 2e73  ils = lines[i].s
+00012610: 7472 6970 2829 2e73 706c 6974 2822 7c22  trip().split("|"
+00012620: 290a 2020 2020 2020 2020 2020 2020 736f  ).            so
+00012630: 6e67 5f69 6420 3d20 696e 7428 6465 7461  ng_id = int(deta
+00012640: 696c 735b 305d 290a 2020 2020 2020 2020  ils[0]).        
+00012650: 2020 2020 6966 2073 6f6e 675f 6964 2069      if song_id i
+00012660: 6e20 736f 6e67 5f69 6473 3a0a 2020 2020  n song_ids:.    
+00012670: 2020 2020 2020 2020 2020 2020 736f 6e67              song
+00012680: 5f69 6473 2e72 656d 6f76 6528 736f 6e67  _ids.remove(song
+00012690: 5f69 6429 0a0a 2020 2020 2020 2020 2020  _id)..          
+000126a0: 2020 2020 2020 6966 2064 6574 6169 6c73        if details
+000126b0: 5b32 5d3a 0a20 2020 2020 2020 2020 2020  [2]:.           
+000126c0: 2020 2020 2020 2020 206e 6577 5f74 6167           new_tag
+000126d0: 7320 3d20 6465 7461 696c 735b 325d 2e73  s = details[2].s
+000126e0: 706c 6974 2822 2c22 290a 2020 2020 2020  plit(",").      
+000126f0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00012700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012710: 2020 2020 6e65 775f 7461 6773 203d 205b      new_tags = [
+00012720: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00012730: 2020 6e65 775f 7461 6773 202b 3d20 5b74    new_tags += [t
+00012740: 6167 2066 6f72 2074 6167 2069 6e20 7461  ag for tag in ta
+00012750: 6773 2069 6620 7461 6720 6e6f 7420 696e  gs if tag not in
+00012760: 206e 6577 5f74 6167 735d 0a20 2020 2020   new_tags].     
+00012770: 2020 2020 2020 2020 2020 2064 6574 6169             detai
+00012780: 6c73 5b32 5d20 3d20 222c 222e 6a6f 696e  ls[2] = ",".join
+00012790: 286e 6577 5f74 6167 7329 0a20 2020 2020  (new_tags).     
+000127a0: 2020 2020 2020 2020 2020 206c 696e 6573             lines
+000127b0: 5b69 5d20 3d20 227c 222e 6a6f 696e 2864  [i] = "|".join(d
+000127c0: 6574 6169 6c73 290a 2020 2020 2020 2020  etails).        
+000127d0: 736f 6e67 735f 6669 6c65 2e63 6c6f 7365  songs_file.close
+000127e0: 2829 0a0a 2020 2020 2020 2020 736f 6e67  ()..        song
+000127f0: 735f 6669 6c65 203d 206f 7065 6e28 534f  s_file = open(SO
+00012800: 4e47 535f 494e 464f 5f50 4154 482c 2022  NGS_INFO_PATH, "
+00012810: 7722 2c20 656e 636f 6469 6e67 3d22 7574  w", encoding="ut
+00012820: 662d 3822 290a 2020 2020 2020 2020 736f  f-8").        so
+00012830: 6e67 735f 6669 6c65 2e77 7269 7465 2822  ngs_file.write("
+00012840: 5c6e 222e 6a6f 696e 286c 696e 6573 2929  \n".join(lines))
+00012850: 0a20 2020 2020 2020 2073 6f6e 6773 5f66  .        songs_f
+00012860: 696c 652e 636c 6f73 6528 290a 0a20 2020  ile.close()..   
+00012870: 2020 2020 2069 6620 736f 6e67 5f69 6473       if song_ids
+00012880: 3a0a 2020 2020 2020 2020 2020 2020 636c  :.            cl
+00012890: 6963 6b2e 7365 6368 6f28 0a20 2020 2020  ick.secho(.     
+000128a0: 2020 2020 2020 2020 2020 2066 2243 6f75             f"Cou
+000128b0: 6c64 206e 6f74 2066 696e 6420 736f 6e67  ld not find song
+000128c0: 2873 2920 7769 7468 2049 4428 7329 207b  (s) with ID(s) {
+000128d0: 272c 2027 2e6a 6f69 6e28 6d61 7028 7374  ', '.join(map(st
+000128e0: 722c 2073 6f6e 675f 6964 7329 297d 2e22  r, song_ids))}."
+000128f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00012900: 2020 6667 3d22 7265 6422 2c0a 2020 2020    fg="red",.    
+00012910: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00012920: 2020 2020 2020 6966 206c 656e 2873 6f6e        if len(son
+00012930: 675f 6964 7329 203d 3d20 6e75 6d5f 736f  g_ids) == num_so
+00012940: 6e67 733a 0a20 2020 2020 2020 2020 2020  ngs:.           
+00012950: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+00012960: 2020 2020 636c 6963 6b2e 7365 6368 6f28      click.secho(
+00012970: 0a20 2020 2020 2020 2020 2020 2066 2241  .            f"A
+00012980: 6464 6564 207b 6c65 6e28 7461 6773 297d  dded {len(tags)}
+00012990: 2074 6167 2873 2920 746f 207b 6e75 6d5f   tag(s) to {num_
+000129a0: 736f 6e67 7320 2d20 6c65 6e28 736f 6e67  songs - len(song
+000129b0: 5f69 6473 297d 2073 6f6e 6728 7329 2e22  _ids)} song(s)."
+000129c0: 2c0a 2020 2020 2020 2020 2020 2020 6667  ,.            fg
+000129d0: 3d22 6772 6565 6e22 2c0a 2020 2020 2020  ="green",.      
+000129e0: 2020 290a 2020 2020 656c 7365 3a0a 2020    ).    else:.  
+000129f0: 2020 2020 2020 636c 6963 6b2e 7365 6368        click.sech
+00012a00: 6f28 224e 6f20 7461 6773 2070 6173 7365  o("No tags passe
+00012a10: 642e 222c 2066 673d 2272 6564 2229 0a0a  d.", fg="red")..
+00012a20: 0a40 636c 692e 636f 6d6d 616e 6428 290a  .@cli.command().
+00012a30: 4063 6c69 636b 2e61 7267 756d 656e 7428  @click.argument(
+00012a40: 2273 6f6e 675f 6964 7322 2c20 7479 7065  "song_ids", type
+00012a50: 3d63 6c69 636b 2e49 4e54 2c20 7265 7175  =click.INT, requ
+00012a60: 6972 6564 3d54 7275 652c 206e 6172 6773  ired=True, nargs
+00012a70: 3d2d 3129 0a40 636c 6963 6b2e 6f70 7469  =-1).@click.opti
+00012a80: 6f6e 280a 2020 2020 222d 7422 2c0a 2020  on(.    "-t",.  
+00012a90: 2020 222d 2d74 6167 222c 0a20 2020 2022    "--tag",.    "
+00012aa0: 7461 6773 222c 0a20 2020 2068 656c 703d  tags",.    help=
+00012ab0: 2254 6167 7320 746f 2072 656d 6f76 652e  "Tags to remove.
+00012ac0: 222c 0a20 2020 206d 756c 7469 706c 653d  ",.    multiple=
+00012ad0: 5472 7565 2c0a 290a 4063 6c69 636b 2e6f  True,.).@click.o
+00012ae0: 7074 696f 6e28 222d 412f 2d6e 4122 2c20  ption("-A/-nA", 
+00012af0: 222d 2d61 6c6c 2f2d 2d6e 6f2d 616c 6c22  "--all/--no-all"
+00012b00: 2c20 2261 6c6c 5f22 2c20 6465 6661 756c  , "all_", defaul
+00012b10: 743d 4661 6c73 6529 0a64 6566 2075 6e74  t=False).def unt
+00012b20: 6167 2873 6f6e 675f 6964 732c 2074 6167  ag(song_ids, tag
+00012b30: 732c 2061 6c6c 5f29 3a0a 2020 2020 2222  s, all_):.    ""
+00012b40: 2252 656d 6f76 6520 7461 6773 2066 726f  "Remove tags fro
+00012b50: 6d20 6120 7370 6563 6966 6963 2073 6f6e  m a specific son
+00012b60: 6720 2870 6173 7365 6420 6173 2049 4429  g (passed as ID)
+00012b70: 2e20 5461 6773 2074 6861 7420 7468 6520  . Tags that the 
+00012b80: 736f 6e67 0a20 2020 2064 6f65 736e 2774  song.    doesn't
+00012b90: 2068 6176 6520 7769 6c6c 2062 6520 6967   have will be ig
+00012ba0: 6e6f 7265 642e 0a0a 2020 2020 5061 7373  nored...    Pass
+00012bb0: 696e 6720 7468 6520 272d 412f 2d2d 616c  ing the '-A/--al
+00012bc0: 6c27 2066 6c61 6720 7769 6c6c 2072 656d  l' flag will rem
+00012bd0: 6f76 6520 616c 6c20 7461 6773 2066 726f  ove all tags fro
+00012be0: 6d20 7468 6520 736f 6e67 2c20 756e 6c65  m the song, unle
+00012bf0: 7373 2054 4147 530a 2020 2020 6973 2070  ss TAGS.    is p
+00012c00: 6173 7365 6420 2869 6e20 7768 6963 6820  assed (in which 
+00012c10: 6361 7365 2074 6865 2066 6c61 6720 6973  case the flag is
+00012c20: 2069 676e 6f72 6564 292e 2222 220a 2020   ignored).""".  
+00012c30: 2020 736f 6e67 5f69 6473 203d 2073 6574    song_ids = set
+00012c40: 2873 6f6e 675f 6964 7329 0a20 2020 206e  (song_ids).    n
+00012c50: 756d 5f73 6f6e 6773 203d 206c 656e 2873  um_songs = len(s
+00012c60: 6f6e 675f 6964 7329 0a20 2020 2074 6167  ong_ids).    tag
+00012c70: 7320 3d20 7365 7428 7461 6773 290a 2020  s = set(tags).  
+00012c80: 2020 6966 2074 6167 733a 0a20 2020 2020    if tags:.     
+00012c90: 2020 2073 6f6e 6773 5f66 696c 6520 3d20     songs_file = 
+00012ca0: 6f70 656e 2853 4f4e 4753 5f49 4e46 4f5f  open(SONGS_INFO_
+00012cb0: 5041 5448 2c20 2272 222c 2065 6e63 6f64  PATH, "r", encod
+00012cc0: 696e 673d 2275 7466 2d38 2229 0a20 2020  ing="utf-8").   
+00012cd0: 2020 2020 206c 696e 6573 203d 2073 6f6e       lines = son
+00012ce0: 6773 5f66 696c 652e 7265 6164 2829 2e73  gs_file.read().s
+00012cf0: 706c 6974 6c69 6e65 7328 290a 2020 2020  plitlines().    
+00012d00: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+00012d10: 6765 286c 656e 286c 696e 6573 2929 3a0a  ge(len(lines)):.
+00012d20: 2020 2020 2020 2020 2020 2020 6465 7461              deta
+00012d30: 696c 7320 3d20 6c69 6e65 735b 695d 2e73  ils = lines[i].s
+00012d40: 7472 6970 2829 2e73 706c 6974 2822 7c22  trip().split("|"
+00012d50: 290a 2020 2020 2020 2020 2020 2020 736f  ).            so
+00012d60: 6e67 5f69 6420 3d20 696e 7428 6465 7461  ng_id = int(deta
+00012d70: 696c 735b 305d 290a 2020 2020 2020 2020  ils[0]).        
+00012d80: 2020 2020 6966 2073 6f6e 675f 6964 2069      if song_id i
+00012d90: 6e20 736f 6e67 5f69 6473 3a0a 2020 2020  n song_ids:.    
+00012da0: 2020 2020 2020 2020 2020 2020 736f 6e67              song
+00012db0: 5f69 6473 2e72 656d 6f76 6528 736f 6e67  _ids.remove(song
+00012dc0: 5f69 6429 0a0a 2020 2020 2020 2020 2020  _id)..          
+00012dd0: 2020 2020 2020 7461 6773 5f74 6f5f 6b65        tags_to_ke
+00012de0: 6570 203d 205b 0a20 2020 2020 2020 2020  ep = [.         
+00012df0: 2020 2020 2020 2020 2020 2074 6167 2066             tag f
+00012e00: 6f72 2074 6167 2069 6e20 6465 7461 696c  or tag in detail
+00012e10: 735b 325d 2e73 706c 6974 2822 2c22 2920  s[2].split(",") 
+00012e20: 6966 2074 6167 206e 6f74 2069 6e20 7461  if tag not in ta
+00012e30: 6773 0a20 2020 2020 2020 2020 2020 2020  gs.             
+00012e40: 2020 205d 0a20 2020 2020 2020 2020 2020     ].           
+00012e50: 2020 2020 206c 696e 6573 5b69 5d20 3d20       lines[i] = 
+00012e60: 227c 222e 6a6f 696e 280a 2020 2020 2020  "|".join(.      
+00012e70: 2020 2020 2020 2020 2020 2020 2020 6465                de
+00012e80: 7461 696c 735b 3a32 5d20 2b20 5b22 2c22  tails[:2] + [","
+00012e90: 2e6a 6f69 6e28 7461 6773 5f74 6f5f 6b65  .join(tags_to_ke
+00012ea0: 6570 295d 202b 2064 6574 6169 6c73 5b33  ep)] + details[3
+00012eb0: 3a5d 0a20 2020 2020 2020 2020 2020 2020  :].             
+00012ec0: 2020 2029 0a20 2020 2020 2020 2073 6f6e     ).        son
+00012ed0: 6773 5f66 696c 652e 636c 6f73 6528 290a  gs_file.close().
+00012ee0: 0a20 2020 2020 2020 2073 6f6e 6773 5f66  .        songs_f
+00012ef0: 696c 6520 3d20 6f70 656e 2853 4f4e 4753  ile = open(SONGS
+00012f00: 5f49 4e46 4f5f 5041 5448 2c20 2277 222c  _INFO_PATH, "w",
+00012f10: 2065 6e63 6f64 696e 673d 2275 7466 2d38   encoding="utf-8
+00012f20: 2229 0a20 2020 2020 2020 2073 6f6e 6773  ").        songs
+00012f30: 5f66 696c 652e 7772 6974 6528 225c 6e22  _file.write("\n"
+00012f40: 2e6a 6f69 6e28 6c69 6e65 7329 290a 2020  .join(lines)).  
+00012f50: 2020 2020 2020 736f 6e67 735f 6669 6c65        songs_file
+00012f60: 2e63 6c6f 7365 2829 0a0a 2020 2020 2020  .close()..      
+00012f70: 2020 6966 2073 6f6e 675f 6964 733a 0a20    if song_ids:. 
+00012f80: 2020 2020 2020 2020 2020 2063 6c69 636b             click
+00012f90: 2e73 6563 686f 280a 2020 2020 2020 2020  .secho(.        
+00012fa0: 2020 2020 2020 2020 6622 436f 756c 6420          f"Could 
+00012fb0: 6e6f 7420 6669 6e64 2073 6f6e 6728 7329  not find song(s)
+00012fc0: 2077 6974 6820 4944 2873 2920 7b27 2c20   with ID(s) {', 
+00012fd0: 272e 6a6f 696e 286d 6170 2873 7472 2c20  '.join(map(str, 
+00012fe0: 736f 6e67 5f69 6473 2929 7d2e 222c 0a20  song_ids))}.",. 
+00012ff0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00013000: 673d 2272 6564 222c 0a20 2020 2020 2020  g="red",.       
+00013010: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00013020: 2020 2069 6620 6c65 6e28 736f 6e67 5f69     if len(song_i
+00013030: 6473 2920 3d3d 206e 756d 5f73 6f6e 6773  ds) == num_songs
+00013040: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00013050: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+00013060: 2063 6c69 636b 2e73 6563 686f 280a 2020   click.secho(.  
+00013070: 2020 2020 2020 2020 2020 6622 5265 6d6f            f"Remo
+00013080: 7665 6420 616e 7920 6f63 6375 7272 656e  ved any occurren
+00013090: 6365 7320 6f66 207b 6c65 6e28 7461 6773  ces of {len(tags
+000130a0: 297d 2074 6167 2873 2920 6672 6f6d 207b  )} tag(s) from {
+000130b0: 6e75 6d5f 736f 6e67 7320 2d20 6c65 6e28  num_songs - len(
+000130c0: 736f 6e67 5f69 6473 297d 2073 6f6e 6728  song_ids)} song(
+000130d0: 7329 2e22 2c0a 2020 2020 2020 2020 2020  s).",.          
+000130e0: 2020 6667 3d22 6772 6565 6e22 2c0a 2020    fg="green",.  
+000130f0: 2020 2020 2020 290a 2020 2020 656c 7365        ).    else
+00013100: 3a0a 2020 2020 2020 2020 6966 206e 6f74  :.        if not
+00013110: 2061 6c6c 5f3a 0a20 2020 2020 2020 2020   all_:.         
+00013120: 2020 2063 6c69 636b 2e73 6563 686f 280a     click.secho(.
+00013130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013140: 224e 6f20 7461 6773 2070 6173 7365 64e2  "No tags passed.
+00013150: 8094 746f 2072 656d 6f76 6520 616c 6c20  ..to remove all 
+00013160: 7461 6773 2c20 7061 7373 2074 6865 2027  tags, pass the '
+00013170: 2d41 2f2d 2d61 6c6c 2720 666c 6167 2e22  -A/--all' flag."
+00013180: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00013190: 2020 6667 3d22 7265 6422 2c0a 2020 2020    fg="red",.    
+000131a0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+000131b0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+000131c0: 2020 2020 736f 6e67 735f 6669 6c65 203d      songs_file =
+000131d0: 206f 7065 6e28 534f 4e47 535f 494e 464f   open(SONGS_INFO
+000131e0: 5f50 4154 482c 2022 7222 2c20 656e 636f  _PATH, "r", enco
+000131f0: 6469 6e67 3d22 7574 662d 3822 290a 2020  ding="utf-8").  
+00013200: 2020 2020 2020 2020 2020 6c69 6e65 7320            lines 
+00013210: 3d20 736f 6e67 735f 6669 6c65 2e72 6561  = songs_file.rea
+00013220: 6428 292e 7370 6c69 746c 696e 6573 2829  d().splitlines()
+00013230: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00013240: 2069 2069 6e20 7261 6e67 6528 6c65 6e28   i in range(len(
+00013250: 6c69 6e65 7329 293a 0a20 2020 2020 2020  lines)):.       
+00013260: 2020 2020 2020 2020 206c 696e 6520 3d20           line = 
+00013270: 6c69 6e65 735b 695d 0a20 2020 2020 2020  lines[i].       
+00013280: 2020 2020 2020 2020 2064 6574 6169 6c73           details
+00013290: 203d 206c 696e 652e 7374 7269 7028 292e   = line.strip().
+000132a0: 7370 6c69 7428 227c 2229 0a20 2020 2020  split("|").     
+000132b0: 2020 2020 2020 2020 2020 2069 6620 696e             if in
+000132c0: 7428 6465 7461 696c 735b 305d 2920 696e  t(details[0]) in
+000132d0: 2073 6f6e 675f 6964 733a 0a20 2020 2020   song_ids:.     
+000132e0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+000132f0: 696e 6573 5b69 5d20 3d20 227c 222e 6a6f  ines[i] = "|".jo
+00013300: 696e 2864 6574 6169 6c73 5b3a 325d 202b  in(details[:2] +
+00013310: 205b 2222 5d20 2b20 6465 7461 696c 735b   [""] + details[
+00013320: 333a 5d29 0a20 2020 2020 2020 2020 2020  3:]).           
+00013330: 2073 6f6e 6773 5f66 696c 652e 636c 6f73   songs_file.clos
+00013340: 6528 290a 0a20 2020 2020 2020 2020 2020  e()..           
+00013350: 2073 6f6e 6773 5f66 696c 6520 3d20 6f70   songs_file = op
+00013360: 656e 2853 4f4e 4753 5f49 4e46 4f5f 5041  en(SONGS_INFO_PA
+00013370: 5448 2c20 2277 222c 2065 6e63 6f64 696e  TH, "w", encodin
+00013380: 673d 2275 7466 2d38 2229 0a20 2020 2020  g="utf-8").     
+00013390: 2020 2020 2020 2073 6f6e 6773 5f66 696c         songs_fil
+000133a0: 652e 7772 6974 6528 225c 6e22 2e6a 6f69  e.write("\n".joi
+000133b0: 6e28 6c69 6e65 7329 290a 2020 2020 2020  n(lines)).      
+000133c0: 2020 2020 2020 736f 6e67 735f 6669 6c65        songs_file
+000133d0: 2e63 6c6f 7365 2829 0a0a 2020 2020 2020  .close()..      
+000133e0: 2020 2020 2020 636c 6963 6b2e 7365 6368        click.sech
+000133f0: 6f28 0a20 2020 2020 2020 2020 2020 2020  o(.             
+00013400: 2020 2066 2252 656d 6f76 6564 207b 6c65     f"Removed {le
+00013410: 6e28 7461 6773 297d 2074 6167 2873 2920  n(tags)} tag(s) 
+00013420: 6672 6f6d 207b 6c65 6e28 736f 6e67 5f69  from {len(song_i
+00013430: 6473 297d 2073 6f6e 6728 7329 2e22 2c0a  ds)} song(s).",.
+00013440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013450: 6667 3d22 6772 6565 6e22 2c0a 2020 2020  fg="green",.    
+00013460: 2020 2020 2020 2020 290a 0a0a 4063 6c69          )...@cli
+00013470: 2e63 6f6d 6d61 6e64 2829 0a40 636c 6963  .command().@clic
+00013480: 6b2e 6172 6775 6d65 6e74 2822 7461 6773  k.argument("tags
+00013490: 222c 206e 6172 6773 3d2d 3129 0a40 636c  ", nargs=-1).@cl
+000134a0: 6963 6b2e 6f70 7469 6f6e 280a 2020 2020  ick.option(.    
+000134b0: 222d 7322 2c0a 2020 2020 222d 2d73 6875  "-s",.    "--shu
+000134c0: 6666 6c65 222c 0a20 2020 2022 7368 7566  ffle",.    "shuf
+000134d0: 666c 655f 222c 0a20 2020 2074 7970 653d  fle_",.    type=
+000134e0: 636c 6963 6b2e 496e 7452 616e 6765 2830  click.IntRange(0
+000134f0: 2c20 3229 2c0a 2020 2020 6865 6c70 3d22  , 2),.    help="
+00013500: 303a 2073 6875 6666 6c65 206f 6e63 652c  0: shuffle once,
+00013510: 2031 3a20 7368 7566 666c 6520 6576 6572   1: shuffle ever
+00013520: 7920 6c6f 6f70 2c20 323a 2073 6875 6666  y loop, 2: shuff
+00013530: 6c65 2065 7665 7279 206c 6f6f 7020 6578  le every loop ex
+00013540: 6365 7074 2066 6f72 2074 6865 2066 6972  cept for the fir
+00013550: 7374 206f 6e65 2e22 2c0a 290a 4063 6c69  st one.",.).@cli
+00013560: 636b 2e6f 7074 696f 6e28 0a20 2020 2022  ck.option(.    "
+00013570: 2d52 2f2d 6e52 222c 0a20 2020 2022 2d2d  -R/-nR",.    "--
+00013580: 7265 7665 7273 652f 2d2d 6e6f 2d72 6576  reverse/--no-rev
+00013590: 6572 7365 222c 0a20 2020 2022 7265 7665  erse",.    "reve
+000135a0: 7273 6522 2c0a 2020 2020 6465 6661 756c  rse",.    defaul
+000135b0: 743d 4661 6c73 652c 0a20 2020 2068 656c  t=False,.    hel
+000135c0: 703d 2250 6c61 7920 736f 6e67 7320 696e  p="Play songs in
+000135d0: 2072 6576 6572 7365 2028 6d6f 7374 2072   reverse (most r
+000135e0: 6563 656e 746c 7920 6164 6465 6420 6669  ecently added fi
+000135f0: 7273 7429 2e22 2c0a 290a 4063 6c69 636b  rst).",.).@click
+00013600: 2e6f 7074 696f 6e28 0a20 2020 2022 2d6f  .option(.    "-o
+00013610: 222c 0a20 2020 2022 2d2d 6f6e 6c79 222c  ",.    "--only",
+00013620: 0a20 2020 2022 6f6e 6c79 222c 0a20 2020  .    "only",.   
+00013630: 2074 7970 653d 636c 6963 6b2e 494e 542c   type=click.INT,
+00013640: 0a20 2020 206d 756c 7469 706c 653d 5472  .    multiple=Tr
+00013650: 7565 2c0a 2020 2020 6865 6c70 3d22 506c  ue,.    help="Pl
+00013660: 6179 206f 6e6c 7920 7468 6973 2f74 6865  ay only this/the
+00013670: 7365 2073 6f6e 6728 7329 2028 6361 6e20  se song(s) (can 
+00013680: 6265 2070 6173 7365 6420 6d75 6c74 6970  be passed multip
+00013690: 6c65 2074 696d 6573 2c20 652e 672e 2027  le times, e.g. '
+000136a0: 6d61 6573 7472 6f20 706c 6179 202d 6f20  maestro play -o 
+000136b0: 3120 2d6f 2031 3727 292e 222c 0a29 0a40  1 -o 17').",.).@
+000136c0: 636c 6963 6b2e 6f70 7469 6f6e 280a 2020  click.option(.  
+000136d0: 2020 222d 7622 2c0a 2020 2020 222d 2d76    "-v",.    "--v
+000136e0: 6f6c 756d 6522 2c0a 2020 2020 2276 6f6c  olume",.    "vol
+000136f0: 756d 6522 2c0a 2020 2020 7479 7065 3d63  ume",.    type=c
+00013700: 6c69 636b 2e49 6e74 5261 6e67 6528 302c  lick.IntRange(0,
+00013710: 2031 3030 292c 0a20 2020 2064 6566 6175   100),.    defau
+00013720: 6c74 3d31 3030 2c0a 2020 2020 7368 6f77  lt=100,.    show
+00013730: 5f64 6566 6175 6c74 3d54 7275 652c 0a29  _default=True,.)
+00013740: 0a40 636c 6963 6b2e 6f70 7469 6f6e 280a  .@click.option(.
+00013750: 2020 2020 222d 4c2f 2d6e 4c22 2c0a 2020      "-L/-nL",.  
+00013760: 2020 222d 2d6c 6f6f 702f 2d2d 6e6f 2d6c    "--loop/--no-l
+00013770: 6f6f 7022 2c0a 2020 2020 226c 6f6f 7022  oop",.    "loop"
+00013780: 2c0a 2020 2020 6465 6661 756c 743d 4661  ,.    default=Fa
+00013790: 6c73 652c 0a20 2020 2068 656c 703d 224c  lse,.    help="L
+000137a0: 6f6f 7020 7468 6520 706c 6179 6c69 7374  oop the playlist
+000137b0: 2e22 2c0a 290a 4063 6c69 636b 2e6f 7074  .",.).@click.opt
+000137c0: 696f 6e28 0a20 2020 2022 2d43 2f2d 6e43  ion(.    "-C/-nC
+000137d0: 222c 0a20 2020 2022 2d2d 636c 6970 732f  ",.    "--clips/
+000137e0: 2d2d 6e6f 2d63 6c69 7073 222c 0a20 2020  --no-clips",.   
+000137f0: 2022 636c 6970 7322 2c0a 2020 2020 6465   "clips",.    de
+00013800: 6661 756c 743d 4661 6c73 652c 0a20 2020  fault=False,.   
+00013810: 2068 656c 703d 2253 7461 7274 2069 6e20   help="Start in 
+00013820: 636c 6970 206d 6f64 652e 2043 616e 2062  clip mode. Can b
+00013830: 6520 746f 6767 6c65 6420 7769 7468 2027  e toggled with '
+00013840: 6327 2e22 2c0a 290a 4063 6c69 636b 2e6f  c'.",.).@click.o
+00013850: 7074 696f 6e28 0a20 2020 2022 2d44 2f2d  ption(.    "-D/-
+00013860: 6e44 222c 0a20 2020 2022 2d2d 6469 7363  nD",.    "--disc
+00013870: 6f72 642f 2d2d 6e6f 2d64 6973 636f 7264  ord/--no-discord
+00013880: 222c 0a20 2020 2022 6469 7363 6f72 6422  ",.    "discord"
+00013890: 2c0a 2020 2020 6465 6661 756c 743d 4661  ,.    default=Fa
+000138a0: 6c73 652c 0a20 2020 2068 656c 703d 2244  lse,.    help="D
+000138b0: 6973 636f 7264 2072 6963 6820 7072 6573  iscord rich pres
+000138c0: 656e 6365 2e20 4967 6e6f 7265 6420 6966  ence. Ignored if
+000138d0: 2072 6571 7569 7265 6420 6465 7065 6e64   required depend
+000138e0: 656e 6369 6573 2061 7265 206e 6f74 2069  encies are not i
+000138f0: 6e73 7461 6c6c 6564 2e20 5769 6c6c 2066  nstalled. Will f
+00013900: 6169 6c20 7369 6c65 6e74 6c79 2061 6e64  ail silently and
+00013910: 2072 6574 7279 2065 7665 7279 2074 696d   retry every tim
+00013920: 6520 7468 6520 736f 6e67 2063 6861 6e67  e the song chang
+00013930: 6573 2069 6620 4469 7363 6f72 6420 636f  es if Discord co
+00013940: 6e6e 6563 7469 6f6e 2066 6169 6c73 2028  nnection fails (
+00013950: 652e 672e 2044 6973 636f 7264 206e 6f74  e.g. Discord not
+00013960: 206f 7065 6e29 2e22 2c0a 290a 4063 6c69   open).",.).@cli
+00013970: 636b 2e6f 7074 696f 6e28 0a20 2020 2022  ck.option(.    "
+00013980: 2d4d 2f2d 6e4d 222c 0a20 2020 2022 2d2d  -M/-nM",.    "--
+00013990: 6d61 7463 682d 616c 6c2f 2d2d 6e6f 2d6d  match-all/--no-m
+000139a0: 6174 6368 2d61 6c6c 222c 0a20 2020 2022  atch-all",.    "
+000139b0: 6d61 7463 685f 616c 6c22 2c0a 2020 2020  match_all",.    
+000139c0: 6465 6661 756c 743d 4661 6c73 652c 0a20  default=False,. 
+000139d0: 2020 2068 656c 703d 2250 6c61 7920 736f     help="Play so
+000139e0: 6e67 7320 7468 6174 206d 6174 6368 2061  ngs that match a
+000139f0: 6c6c 2074 6167 732c 206e 6f74 2061 6e79  ll tags, not any
+00013a00: 2e22 2c0a 290a 4063 6c69 636b 2e6f 7074  .",.).@click.opt
+00013a10: 696f 6e28 0a20 2020 2022 2d56 2f2d 6e56  ion(.    "-V/-nV
+00013a20: 222c 0a20 2020 2022 2d2d 7669 7375 616c  ",.    "--visual
+00013a30: 697a 652f 2d2d 6e6f 2d76 6973 7561 6c69  ize/--no-visuali
+00013a40: 7a65 222c 0a20 2020 2022 7669 7375 616c  ze",.    "visual
+00013a50: 697a 6522 2c0a 2020 2020 6465 6661 756c  ize",.    defaul
+00013a60: 743d 4661 6c73 652c 0a20 2020 2068 656c  t=False,.    hel
+00013a70: 703d 2256 6973 7561 6c69 7a65 2074 6865  p="Visualize the
+00013a80: 2073 6f6e 6720 6265 696e 6720 706c 6179   song being play
+00013a90: 6564 2e20 4967 6e6f 7265 6420 6966 2072  ed. Ignored if r
+00013aa0: 6571 7569 7265 6420 6465 7065 6e64 656e  equired dependen
+00013ab0: 6369 6573 2061 7265 206e 6f74 2069 6e73  cies are not ins
+00013ac0: 7461 6c6c 6564 2e22 2c0a 290a 6465 6620  talled.",.).def 
+00013ad0: 706c 6179 280a 2020 2020 7461 6773 2c0a  play(.    tags,.
+00013ae0: 2020 2020 7368 7566 666c 655f 2c0a 2020      shuffle_,.  
+00013af0: 2020 7265 7665 7273 652c 0a20 2020 206f    reverse,.    o
+00013b00: 6e6c 792c 0a20 2020 2076 6f6c 756d 652c  nly,.    volume,
+00013b10: 0a20 2020 206c 6f6f 702c 0a20 2020 2063  .    loop,.    c
+00013b20: 6c69 7073 2c0a 2020 2020 6469 7363 6f72  lips,.    discor
+00013b30: 642c 0a20 2020 206d 6174 6368 5f61 6c6c  d,.    match_all
+00013b40: 2c0a 2020 2020 7669 7375 616c 697a 652c  ,.    visualize,
+00013b50: 0a29 3a0a 2020 2020 2222 2250 6c61 7920  .):.    """Play 
+00013b60: 796f 7572 2073 6f6e 6773 2e20 4966 2074  your songs. If t
+00013b70: 6167 7320 6172 6520 7061 7373 6564 2c20  ags are passed, 
+00013b80: 616e 7920 736f 6e67 206d 6174 6368 696e  any song matchin
+00013b90: 6720 616e 7920 7461 6720 7769 6c6c 2062  g any tag will b
+00013ba0: 6520 696e 0a20 2020 2079 6f75 7220 706c  e in.    your pl
+00013bb0: 6179 6c69 7374 2c20 756e 6c65 7373 2074  aylist, unless t
+00013bc0: 6865 2027 2d4d 2f2d 2d6d 6174 6368 2d61  he '-M/--match-a
+00013bd0: 6c6c 2720 666c 6167 2069 7320 7061 7373  ll' flag is pass
+00013be0: 6564 2c20 696e 2077 6869 6368 2063 6173  ed, in which cas
+00013bf0: 650a 2020 2020 6576 6572 7920 7461 6720  e.    every tag 
+00013c00: 6d75 7374 2062 6520 6d61 7463 6865 642e  must be matched.
+00013c10: 0a0a 2020 2020 5c62 0a20 2020 205c 7831  ..    \b.    \x1
+00013c20: 625b 316d 5350 4143 455c 7831 625b 306d  b[1mSPACE\x1b[0m
+00013c30: 2020 746f 2070 6175 7365 2f70 6c61 790a    to pause/play.
+00013c40: 2020 2020 5c78 3162 5b31 6d62 5c78 3162      \x1b[1mb\x1b
+00013c50: 5b30 6d20 2074 6f20 676f 205b 625d 6163  [0m  to go [b]ac
+00013c60: 6b20 746f 2070 7265 7669 6f75 7320 736f  k to previous so
+00013c70: 6e67 0a20 2020 205c 7831 625b 316d 725c  ng.    \x1b[1mr\
+00013c80: 7831 625b 306d 2020 746f 205b 725d 6570  x1b[0m  to [r]ep
+00013c90: 6c61 7920 736f 6e67 0a20 2020 205c 7831  lay song.    \x1
+00013ca0: 625b 316d 6e5c 7831 625b 306d 2020 746f  b[1mn\x1b[0m  to
+00013cb0: 2073 6b69 7020 746f 205b 6e5d 6578 7420   skip to [n]ext 
+00013cc0: 736f 6e67 0a20 2020 205c 7831 625b 316d  song.    \x1b[1m
+00013cd0: 6c5c 7831 625b 306d 2020 746f 205b 6c5d  l\x1b[0m  to [l]
+00013ce0: 6f6f 7020 7468 6520 6375 7272 656e 7420  oop the current 
+00013cf0: 736f 6e67 206f 6e63 6520 2827 6c27 2069  song once ('l' i
+00013d00: 6e20 7374 6174 7573 2062 6172 292e 2070  n status bar). p
+00013d10: 7265 7373 2061 6761 696e 2074 6f20 6c6f  ress again to lo
+00013d20: 6f70 2069 6e66 696e 6974 656c 7920 2827  op infinitely ('
+00013d30: 4c27 2069 6e20 7374 6174 7573 2062 6172  L' in status bar
+00013d40: 292e 2070 7265 7373 206f 6e63 6520 6167  ). press once ag
+00013d50: 6169 6e20 746f 2074 7572 6e20 6f66 6620  ain to turn off 
+00013d60: 6c6f 6f70 696e 670a 2020 2020 5c78 3162  looping.    \x1b
+00013d70: 5b31 6d63 5c78 3162 5b30 6d20 2074 6f20  [1mc\x1b[0m  to 
+00013d80: 746f 6767 6c65 205b 635d 6c69 7020 6d6f  toggle [c]lip mo
+00013d90: 6465 0a20 2020 205c 7831 625b 316d 765c  de.    \x1b[1mv\
+00013da0: 7831 625b 306d 2020 746f 2074 6f67 676c  x1b[0m  to toggl
+00013db0: 6520 5b76 5d69 7375 616c 697a 6174 696f  e [v]isualizatio
+00013dc0: 6e0a 2020 2020 5c78 3162 5b31 6d4c 4546  n.    \x1b[1mLEF
+00013dd0: 545c 7831 625b 306d 2020 746f 2072 6577  T\x1b[0m  to rew
+00013de0: 696e 6420 3573 0a20 2020 205c 7831 625b  ind 5s.    \x1b[
+00013df0: 316d 5249 4748 545c 7831 625b 306d 2020  1mRIGHT\x1b[0m  
+00013e00: 746f 2066 6173 7420 666f 7277 6172 6420  to fast forward 
+00013e10: 3573 0a20 2020 205c 7831 625b 316d 5b5c  5s.    \x1b[1m[\
+00013e20: 7831 625b 306d 2020 746f 2064 6563 7265  x1b[0m  to decre
+00013e30: 6173 6520 766f 6c75 6d65 0a20 2020 205c  ase volume.    \
+00013e40: 7831 625b 316d 5d5c 7831 625b 306d 2020  x1b[1m]\x1b[0m  
+00013e50: 746f 2069 6e63 7265 6173 6520 766f 6c75  to increase volu
+00013e60: 6d65 0a20 2020 205c 7831 625b 316d 6d5c  me.    \x1b[1mm\
+00013e70: 7831 625b 306d 2020 746f 205b 6d5d 7574  x1b[0m  to [m]ut
+00013e80: 652f 756e 6d75 7465 0a20 2020 205c 7831  e/unmute.    \x1
+00013e90: 625b 316d 655c 7831 625b 306d 2020 746f  b[1me\x1b[0m  to
+00013ea0: 205b 655d 6e64 2074 6865 2073 6f6e 6720   [e]nd the song 
+00013eb0: 706c 6179 6572 2061 6674 6572 2074 6865  player after the
+00013ec0: 2063 7572 7265 6e74 2073 6f6e 6720 6669   current song fi
+00013ed0: 6e69 7368 6573 2028 696e 6469 6361 746f  nishes (indicato
+00013ee0: 7220 696e 2073 7461 7475 7320 6261 722c  r in status bar,
+00013ef0: 2027 6527 2074 6f20 6361 6e63 656c 290a   'e' to cancel).
+00013f00: 2020 2020 5c78 3162 5b31 6d71 5c78 3162      \x1b[1mq\x1b
+00013f10: 5b30 6d20 2074 6f20 5b71 5d75 6974 2074  [0m  to [q]uit t
+00013f20: 6865 2073 6f6e 6720 706c 6179 6572 2069  he song player i
+00013f30: 6d6d 6564 6961 7465 6c79 0a20 2020 205c  mmediately.    \
+00013f40: 7831 625b 316d 5550 2f44 4f57 4e5c 7831  x1b[1mUP/DOWN\x1
+00013f50: 625b 306d 2020 746f 2073 6372 6f6c 6c20  b[0m  to scroll 
+00013f60: 7468 726f 7567 6820 7468 6520 706c 6179  through the play
+00013f70: 6c69 7374 2028 6d6f 7573 6520 7363 726f  list (mouse scro
+00013f80: 6c6c 696e 6720 7368 6f75 6c64 2061 6c73  lling should als
+00013f90: 6f20 776f 726b 290a 2020 2020 5c78 3162  o work).    \x1b
+00013fa0: 5b31 6d70 5c78 3162 5b30 6d20 2074 6f20  [1mp\x1b[0m  to 
+00013fb0: 736e 615b 705d 2062 6163 6b20 746f 2074  sna[p] back to t
+00013fc0: 6865 2063 7572 7265 6e74 6c79 2070 6c61  he currently pla
+00013fd0: 7969 6e67 2073 6f6e 670a 2020 2020 5c78  ying song.    \x
+00013fe0: 3162 5b31 6d67 5c78 3162 5b30 6d20 2074  1b[1mg\x1b[0m  t
+00013ff0: 6f20 676f 2074 6f20 7468 6520 6e65 7874  o go to the next
+00014000: 2070 615b 675d 652f 6c6f 6f70 206f 6620   pa[g]e/loop of 
+00014010: 7468 6520 706c 6179 6c69 7374 2028 6967  the playlist (ig
+00014020: 6e6f 7265 6420 6966 206e 6f74 2072 6570  nored if not rep
+00014030: 6561 7469 6e67 2070 6c61 796c 6973 7429  eating playlist)
+00014040: 0a20 2020 205c 7831 625b 316d 4241 434b  .    \x1b[1mBACK
+00014050: 5350 4143 452f 4445 4c45 5445 5c78 3162  SPACE/DELETE\x1b
+00014060: 5b30 6d20 2064 656c 6574 6520 7468 6520  [0m  delete the 
+00014070: 7365 6c65 6374 6564 2028 6e6f 7420 6e65  selected (not ne
+00014080: 6365 7373 6172 696c 7920 6375 7272 656e  cessarily curren
+00014090: 746c 7920 706c 6179 696e 6721 2920 736f  tly playing!) so
+000140a0: 6e67 2066 726f 6d20 7468 6520 7175 6575  ng from the queu
+000140b0: 650a 2020 2020 5c78 3162 5b31 6d64 5c78  e.    \x1b[1md\x
+000140c0: 3162 5b30 6d20 2074 6f20 746f 6767 6c65  1b[0m  to toggle
+000140d0: 205b 445d 6973 636f 7264 2072 6963 6820   [D]iscord rich 
+000140e0: 7072 6573 656e 6365 0a20 2020 205c 7831  presence.    \x1
+000140f0: 625b 316d 615c 7831 625b 306d 2020 746f  b[1ma\x1b[0m  to
+00014100: 2061 6464 2061 2073 6f6e 6720 2862 7920   add a song (by 
+00014110: 4944 2920 746f 2074 6865 2065 6e64 206f  ID) to the end o
+00014120: 6620 7468 6520 706c 6179 6c69 7374 2e20  f the playlist. 
+00014130: 4f70 656e 7320 6120 7072 6f6d 7074 2074  Opens a prompt t
+00014140: 6f20 656e 7465 7220 7468 6520 4944 3a20  o enter the ID: 
+00014150: 454e 5445 5220 746f 2063 6f6e 6669 726d  ENTER to confirm
+00014160: 2c20 4553 4320 746f 2063 616e 6365 6c2e  , ESC to cancel.
+00014170: 0a20 2020 205c 7831 625b 316d 695c 7831  .    \x1b[1mi\x1
+00014180: 625b 306d 2020 746f 2069 6e73 6572 7420  b[0m  to insert 
+00014190: 6120 736f 6e67 2028 6279 2049 4429 2069  a song (by ID) i
+000141a0: 6e20 7468 6520 706c 6179 6c69 7374 2061  n the playlist a
+000141b0: 6674 6572 2074 6865 2073 656c 6563 7465  fter the selecte
+000141c0: 6420 736f 6e67 2e20 4f70 656e 7320 6120  d song. Opens a 
+000141d0: 7072 6f6d 7074 206c 696b 6520 2761 272e  prompt like 'a'.
+000141e0: 0a20 2020 205c 7831 625b 316d 745c 7831  .    \x1b[1mt\x1
+000141f0: 625b 306d 2020 746f 2061 6464 2061 2074  b[0m  to add a t
+00014200: 6167 2074 6f20 616c 6c20 736f 6e67 7320  ag to all songs 
+00014210: 696e 2074 6865 2070 6c61 796c 6973 742e  in the playlist.
+00014220: 204f 7065 6e73 2061 2070 726f 6d70 7420   Opens a prompt 
+00014230: 746f 2065 6e74 6572 2074 6865 2074 6167  to enter the tag
+00014240: 3a20 454e 5445 5220 746f 2063 6f6e 6669  : ENTER to confi
+00014250: 726d 2c20 4553 4320 746f 2063 616e 6365  rm, ESC to cance
+00014260: 6c2e 0a0a 2020 2020 5c62 0a20 2020 2073  l...    \b.    s
+00014270: 6f6e 6720 636f 6c6f 7220 696e 6469 6361  ong color indica
+00014280: 7465 7320 6d6f 6465 3a0a 2020 2020 2020  tes mode:.      
+00014290: 2020 5c78 3162 5b31 3b33 346d 626c 7565    \x1b[1;34mblue
+000142a0: 5c78 3162 5b30 6d20 2020 2020 6e6f 726d  \x1b[0m     norm
+000142b0: 616c 0a20 2020 2020 2020 205c 7831 625b  al.        \x1b[
+000142c0: 313b 3333 6d79 656c 6c6f 775c 7831 625b  1;33myellow\x1b[
+000142d0: 306d 2020 206c 6f6f 7069 6e67 2063 7572  0m   looping cur
+000142e0: 7265 6e74 2073 6f6e 6720 286f 6e63 6520  rent song (once 
+000142f0: 6f72 2072 6570 6561 7465 646c 7929 0a0a  or repeatedly)..
+00014300: 2020 2020 5c62 0a20 2020 2070 726f 6772      \b.    progr
+00014310: 6573 7320 6261 7220 636f 6c6f 7220 696e  ess bar color in
+00014320: 6469 6361 7465 7320 7374 6174 7573 3a0a  dicates status:.
+00014330: 2020 2020 2020 2020 5c78 3162 5b31 3b33          \x1b[1;3
+00014340: 336d 7965 6c6c 6f77 5c78 3162 5b30 6d20  3myellow\x1b[0m 
+00014350: 2020 6e6f 726d 616c 2028 6f72 2063 7572    normal (or cur
+00014360: 7265 6e74 2073 6f6e 6720 646f 6573 6e27  rent song doesn'
+00014370: 7420 6861 7665 2061 2063 6c69 7029 0a20  t have a clip). 
+00014380: 2020 2020 2020 205c 7831 625b 313b 3335         \x1b[1;35
+00014390: 6d6d 6167 656e 7461 5c78 3162 5b30 6d20  mmagenta\x1b[0m 
+000143a0: 2070 6c61 7969 6e67 2063 6c69 700a 0a20   playing clip.. 
+000143b0: 2020 2046 6f72 2074 6865 2063 6f6c 6f72     For the color
+000143c0: 2076 6973 696f 6e20 6465 6669 6369 656e   vision deficien
+000143d0: 742c 2062 6f74 6820 6d6f 6465 7320 616c  t, both modes al
+000143e0: 736f 2068 6176 6520 696e 6469 6361 746f  so have indicato
+000143f0: 7273 2069 6e20 7468 6520 7374 6174 7573  rs in the status
+00014400: 2062 6172 2e0a 2020 2020 2222 220a 2020   bar..    """.  
+00014410: 2020 706c 6179 6c69 7374 203d 205b 5d0a    playlist = [].
+00014420: 2020 2020 736f 6e67 735f 6e6f 745f 666f      songs_not_fo
+00014430: 756e 6420 3d20 5b5d 0a0a 2020 2020 6966  und = []..    if
+00014440: 206f 6e6c 793a 0a20 2020 2020 2020 206f   only:.        o
+00014450: 6e6c 7920 3d20 7365 7428 6f6e 6c79 290a  nly = set(only).
+00014460: 2020 2020 2020 2020 7769 7468 206f 7065          with ope
+00014470: 6e28 534f 4e47 535f 494e 464f 5f50 4154  n(SONGS_INFO_PAT
+00014480: 482c 2022 7222 2c20 656e 636f 6469 6e67  H, "r", encoding
+00014490: 3d22 7574 662d 3822 2920 6173 2073 6f6e  ="utf-8") as son
+000144a0: 6773 5f66 696c 653a 0a20 2020 2020 2020  gs_file:.       
+000144b0: 2020 2020 2066 6f72 206c 696e 6520 696e       for line in
+000144c0: 2073 6f6e 6773 5f66 696c 653a 0a20 2020   songs_file:.   
+000144d0: 2020 2020 2020 2020 2020 2020 2064 6574               det
+000144e0: 6169 6c73 203d 206c 696e 652e 7374 7269  ails = line.stri
+000144f0: 7028 292e 7370 6c69 7428 227c 2229 0a20  p().split("|"). 
+00014500: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00014510: 6f6e 675f 6964 203d 2069 6e74 2864 6574  ong_id = int(det
+00014520: 6169 6c73 5b30 5d29 0a20 2020 2020 2020  ails[0]).       
+00014530: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+00014540: 6f73 2e70 6174 682e 6578 6973 7473 286f  os.path.exists(o
+00014550: 732e 7061 7468 2e6a 6f69 6e28 534f 4e47  s.path.join(SONG
+00014560: 535f 4449 522c 2064 6574 6169 6c73 5b31  S_DIR, details[1
+00014570: 5d29 293a 0a20 2020 2020 2020 2020 2020  ])):.           
+00014580: 2020 2020 2020 2020 2073 6f6e 6773 5f6e           songs_n
+00014590: 6f74 5f66 6f75 6e64 2e61 7070 656e 6428  ot_found.append(
+000145a0: 6465 7461 696c 7329 0a20 2020 2020 2020  details).       
+000145b0: 2020 2020 2020 2020 2065 6c69 6620 736f           elif so
+000145c0: 6e67 5f69 6420 696e 206f 6e6c 793a 0a20  ng_id in only:. 
+000145d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000145e0: 2020 2070 6c61 796c 6973 742e 6170 7065     playlist.appe
+000145f0: 6e64 2864 6574 6169 6c73 290a 0a20 2020  nd(details)..   
+00014600: 2020 2020 2069 6620 6e6f 7420 706c 6179       if not play
+00014610: 6c69 7374 3a0a 2020 2020 2020 2020 2020  list:.          
+00014620: 2020 636c 6963 6b2e 7365 6368 6f28 224e    click.secho("N
+00014630: 6f20 736f 6e67 7320 666f 756e 6420 7769  o songs found wi
+00014640: 7468 2074 6865 2067 6976 656e 2049 4473  th the given IDs
+00014650: 2e22 2c20 6667 3d22 7265 6422 290a 2020  .", fg="red").  
+00014660: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00014670: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+00014680: 2020 2069 6620 6e6f 7420 7461 6773 3a0a     if not tags:.
+00014690: 2020 2020 2020 2020 2020 2020 7769 7468              with
+000146a0: 206f 7065 6e28 534f 4e47 535f 494e 464f   open(SONGS_INFO
+000146b0: 5f50 4154 482c 2022 7222 2c20 656e 636f  _PATH, "r", enco
+000146c0: 6469 6e67 3d22 7574 662d 3822 2920 6173  ding="utf-8") as
+000146d0: 2073 6f6e 6773 5f66 696c 653a 0a20 2020   songs_file:.   
+000146e0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+000146f0: 206c 696e 6520 696e 2073 6f6e 6773 5f66   line in songs_f
+00014700: 696c 653a 0a20 2020 2020 2020 2020 2020  ile:.           
+00014710: 2020 2020 2020 2020 2064 6574 6169 6c73           details
+00014720: 203d 206c 696e 652e 7374 7269 7028 292e   = line.strip().
+00014730: 7370 6c69 7428 227c 2229 0a20 2020 2020  split("|").     
+00014740: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00014750: 6620 6e6f 7420 6f73 2e70 6174 682e 6578  f not os.path.ex
+00014760: 6973 7473 286f 732e 7061 7468 2e6a 6f69  ists(os.path.joi
+00014770: 6e28 534f 4e47 535f 4449 522c 2064 6574  n(SONGS_DIR, det
+00014780: 6169 6c73 5b31 5d29 293a 0a20 2020 2020  ails[1])):.     
+00014790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000147a0: 2020 2073 6f6e 6773 5f6e 6f74 5f66 6f75     songs_not_fou
+000147b0: 6e64 2e61 7070 656e 6428 6465 7461 696c  nd.append(detail
+000147c0: 7329 0a20 2020 2020 2020 2020 2020 2020  s).             
+000147d0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+000147e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000147f0: 2020 2020 2070 6c61 796c 6973 742e 6170       playlist.ap
+00014800: 7065 6e64 2864 6574 6169 6c73 290a 2020  pend(details).  
+00014810: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00014820: 2020 2020 2020 2020 7461 6773 203d 2073          tags = s
+00014830: 6574 2874 6167 7329 0a20 2020 2020 2020  et(tags).       
+00014840: 2020 2020 2077 6974 6820 6f70 656e 2853       with open(S
+00014850: 4f4e 4753 5f49 4e46 4f5f 5041 5448 2c20  ONGS_INFO_PATH, 
+00014860: 2272 222c 2065 6e63 6f64 696e 673d 2275  "r", encoding="u
+00014870: 7466 2d38 2229 2061 7320 736f 6e67 735f  tf-8") as songs_
+00014880: 6669 6c65 3a0a 2020 2020 2020 2020 2020  file:.          
+00014890: 2020 2020 2020 666f 7220 6c69 6e65 2069        for line i
+000148a0: 6e20 736f 6e67 735f 6669 6c65 3a0a 2020  n songs_file:.  
+000148b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000148c0: 2020 6465 7461 696c 7320 3d20 6c69 6e65    details = line
+000148d0: 2e73 7472 6970 2829 2e73 706c 6974 2822  .strip().split("
+000148e0: 7c22 290a 2020 2020 2020 2020 2020 2020  |").            
+000148f0: 2020 2020 2020 2020 736f 6e67 5f74 6167          song_tag
+00014900: 7320 3d20 7365 7428 6465 7461 696c 735b  s = set(details[
+00014910: 325d 2e73 706c 6974 2822 2c22 2929 0a20  2].split(",")). 
+00014920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014930: 2020 2069 6620 6e6f 7420 6f73 2e70 6174     if not os.pat
+00014940: 682e 6578 6973 7473 286f 732e 7061 7468  h.exists(os.path
+00014950: 2e6a 6f69 6e28 534f 4e47 535f 4449 522c  .join(SONGS_DIR,
+00014960: 2064 6574 6169 6c73 5b31 5d29 293a 0a20   details[1])):. 
+00014970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014980: 2020 2020 2020 2073 6f6e 6773 5f6e 6f74         songs_not
+00014990: 5f66 6f75 6e64 2e61 7070 656e 6428 6465  _found.append(de
+000149a0: 7461 696c 7329 0a20 2020 2020 2020 2020  tails).         
+000149b0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+000149c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000149d0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+000149e0: 6d61 7463 685f 616c 6c3a 0a20 2020 2020  match_all:.     
+000149f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014a00: 2020 2020 2020 2069 6620 7461 6773 2026         if tags &
+00014a10: 2073 6f6e 675f 7461 6773 3a20 2023 2069   song_tags:  # i
+00014a20: 6e74 6572 7365 6374 696f 6e0a 2020 2020  ntersection.    
+00014a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014a40: 2020 2020 2020 2020 2020 2020 706c 6179              play
+00014a50: 6c69 7374 2e61 7070 656e 6428 6465 7461  list.append(deta
+00014a60: 696c 7329 0a20 2020 2020 2020 2020 2020  ils).           
+00014a70: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00014a80: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00014a90: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00014aa0: 6620 7461 6773 203c 3d20 736f 6e67 5f74  f tags <= song_t
+00014ab0: 6167 733a 2020 2320 7375 6273 6574 0a20  ags:  # subset. 
+00014ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ad0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00014ae0: 6c61 796c 6973 742e 6170 7065 6e64 2864  laylist.append(d
+00014af0: 6574 6169 6c73 290a 0a20 2020 2066 6f72  etails)..    for
+00014b00: 2064 6574 6169 6c73 2069 6e20 706c 6179   details in play
+00014b10: 6c69 7374 3a0a 2020 2020 2020 2020 736f  list:.        so
+00014b20: 6e67 5f64 6174 6120 3d20 6d75 7369 635f  ng_data = music_
+00014b30: 7461 672e 6c6f 6164 5f66 696c 6528 6f73  tag.load_file(os
+00014b40: 2e70 6174 682e 6a6f 696e 2853 4f4e 4753  .path.join(SONGS
+00014b50: 5f44 4952 2c20 6465 7461 696c 735b 315d  _DIR, details[1]
+00014b60: 2929 0a20 2020 2020 2020 2064 6574 6169  )).        detai
+00014b70: 6c73 202b 3d20 5b0a 2020 2020 2020 2020  ls += [.        
+00014b80: 2020 2020 2873 6f6e 675f 6461 7461 5b22      (song_data["
+00014b90: 6172 7469 7374 225d 2e76 616c 7565 206f  artist"].value o
+00014ba0: 7220 2255 6e6b 6e6f 776e 2041 7274 6973  r "Unknown Artis
+00014bb0: 7422 292c 0a20 2020 2020 2020 2020 2020  t"),.           
+00014bc0: 2028 736f 6e67 5f64 6174 615b 2261 6c62   (song_data["alb
+00014bd0: 756d 225d 2e76 616c 7565 206f 7220 2255  um"].value or "U
+00014be0: 6e6b 6e6f 776e 2041 6c62 756d 2229 2c0a  nknown Album"),.
+00014bf0: 2020 2020 2020 2020 2020 2020 2873 6f6e              (son
+00014c00: 675f 6461 7461 5b22 616c 6275 6d61 7274  g_data["albumart
+00014c10: 6973 7422 5d2e 7661 6c75 6520 6f72 2022  ist"].value or "
+00014c20: 556e 6b6e 6f77 6e20 416c 6275 6d20 4172  Unknown Album Ar
+00014c30: 7469 7374 2229 2c0a 2020 2020 2020 2020  tist"),.        
+00014c40: 5d0a 0a20 2020 2069 6620 7368 7566 666c  ]..    if shuffl
+00014c50: 655f 203d 3d20 303a 0a20 2020 2020 2020  e_ == 0:.       
+00014c60: 2073 6875 6666 6c65 5f20 3d20 5472 7565   shuffle_ = True
+00014c70: 0a20 2020 2020 2020 2072 6573 6875 6666  .        reshuff
+00014c80: 6c65 203d 2046 616c 7365 0a20 2020 2065  le = False.    e
+00014c90: 6c69 6620 7368 7566 666c 655f 203d 3d20  lif shuffle_ == 
+00014ca0: 313a 0a20 2020 2020 2020 2073 6875 6666  1:.        shuff
+00014cb0: 6c65 5f20 3d20 5472 7565 0a20 2020 2020  le_ = True.     
+00014cc0: 2020 2072 6573 6875 6666 6c65 203d 2054     reshuffle = T
+00014cd0: 7275 650a 2020 2020 656c 6966 2073 6875  rue.    elif shu
+00014ce0: 6666 6c65 5f20 3d3d 2032 3a0a 2020 2020  ffle_ == 2:.    
+00014cf0: 2020 2020 7368 7566 666c 655f 203d 2046      shuffle_ = F
+00014d00: 616c 7365 0a20 2020 2020 2020 2072 6573  alse.        res
+00014d10: 6875 6666 6c65 203d 2054 7275 650a 2020  huffle = True.  
+00014d20: 2020 656c 7365 3a20 2023 2073 6875 6666    else:  # shuff
+00014d30: 6c65 5f20 3d20 4e6f 6e65 0a20 2020 2020  le_ = None.     
+00014d40: 2020 2073 6875 6666 6c65 5f20 3d20 4661     shuffle_ = Fa
+00014d50: 6c73 650a 2020 2020 2020 2020 7265 7368  lse.        resh
+00014d60: 7566 666c 6520 3d20 4661 6c73 650a 0a20  uffle = False.. 
+00014d70: 2020 2069 6620 7368 7566 666c 655f 3a0a     if shuffle_:.
+00014d80: 2020 2020 2020 2020 7368 7566 666c 6528          shuffle(
+00014d90: 706c 6179 6c69 7374 290a 2020 2020 656c  playlist).    el
+00014da0: 6966 2072 6576 6572 7365 3a0a 2020 2020  if reverse:.    
+00014db0: 2020 2020 706c 6179 6c69 7374 2e72 6576      playlist.rev
+00014dc0: 6572 7365 2829 0a0a 2020 2020 6966 206e  erse()..    if n
+00014dd0: 6f74 2070 6c61 796c 6973 743a 0a20 2020  ot playlist:.   
+00014de0: 2020 2020 2063 6c69 636b 2e73 6563 686f       click.secho
+00014df0: 2822 4e6f 2073 6f6e 6773 2066 6f75 6e64  ("No songs found
+00014e00: 206d 6174 6368 696e 6720 7461 6720 6372   matching tag cr
+00014e10: 6974 6572 6961 2e22 2c20 6667 3d22 7265  iteria.", fg="re
+00014e20: 6422 290a 2020 2020 656c 7365 3a0a 2020  d").    else:.  
+00014e30: 2020 2020 2020 766f 6c75 6d65 202f 3d20        volume /= 
+00014e40: 3130 300a 2020 2020 2020 2020 6375 7273  100.        curs
+00014e50: 6573 2e77 7261 7070 6572 280a 2020 2020  es.wrapper(.    
+00014e60: 2020 2020 2020 2020 5f70 6c61 792c 0a20          _play,. 
+00014e70: 2020 2020 2020 2020 2020 2070 6c61 796c             playl
+00014e80: 6973 742c 0a20 2020 2020 2020 2020 2020  ist,.           
+00014e90: 2076 6f6c 756d 652c 0a20 2020 2020 2020   volume,.       
+00014ea0: 2020 2020 206c 6f6f 702c 0a20 2020 2020       loop,.     
+00014eb0: 2020 2020 2020 2063 6c69 7073 2c0a 2020         clips,.  
+00014ec0: 2020 2020 2020 2020 2020 7265 7368 7566            reshuf
+00014ed0: 666c 652c 0a20 2020 2020 2020 2020 2020  fle,.           
+00014ee0: 2064 6973 636f 7264 2061 6e64 2063 616e   discord and can
+00014ef0: 5f75 7064 6174 655f 6469 7363 6f72 642c  _update_discord,
+00014f00: 0a20 2020 2020 2020 2020 2020 2076 6973  .            vis
+00014f10: 7561 6c69 7a65 2c0a 2020 2020 2020 2020  ualize,.        
+00014f20: 290a 0a20 2020 2069 6620 736f 6e67 735f  )..    if songs_
+00014f30: 6e6f 745f 666f 756e 643a 0a20 2020 2020  not_found:.     
+00014f40: 2020 2063 6c69 636b 2e73 6563 686f 2822     click.secho("
+00014f50: 536f 6e67 2066 696c 6573 206e 6f74 2066  Song files not f
+00014f60: 6f75 6e64 3a22 2c20 6667 3d22 7265 6422  ound:", fg="red"
+00014f70: 290a 2020 2020 2020 2020 666f 7220 6465  ).        for de
+00014f80: 7461 696c 7320 696e 2073 6f6e 6773 5f6e  tails in songs_n
+00014f90: 6f74 5f66 6f75 6e64 3a0a 2020 2020 2020  ot_found:.      
+00014fa0: 2020 2020 2020 636c 6963 6b2e 7365 6368        click.sech
+00014fb0: 6f28 6622 5c74 7b64 6574 6169 6c73 5b31  o(f"\t{details[1
+00014fc0: 5d7d 2028 4944 207b 6465 7461 696c 735b  ]} (ID {details[
+00014fd0: 305d 7d29 222c 2066 673d 2272 6564 2229  0]})", fg="red")
+00014fe0: 0a0a 0a40 636c 692e 636f 6d6d 616e 6428  ...@cli.command(
+00014ff0: 290a 4063 6c69 636b 2e6f 7074 696f 6e28  ).@click.option(
+00015000: 0a20 2020 2022 2d54 2f2d 6e54 222c 0a20  .    "-T/-nT",. 
+00015010: 2020 2022 2d2d 7461 672f 2d2d 6e6f 2d74     "--tag/--no-t
+00015020: 6167 222c 0a20 2020 2022 7265 6e61 6d69  ag",.    "renami
+00015030: 6e67 5f74 6167 222c 0a20 2020 2064 6566  ng_tag",.    def
+00015040: 6175 6c74 3d46 616c 7365 2c0a 2020 2020  ault=False,.    
+00015050: 6865 6c70 3d22 4966 2070 6173 7365 642c  help="If passed,
+00015060: 2072 656e 616d 6520 7461 6720 696e 7374   rename tag inst
+00015070: 6561 6420 6f66 2073 6f6e 6720 2874 7265  ead of song (tre
+00015080: 6174 2074 6865 2061 7267 756d 656e 7473  at the arguments
+00015090: 2061 7320 7461 6773 292e 222c 0a29 0a40   as tags).",.).@
+000150a0: 636c 6963 6b2e 6172 6775 6d65 6e74 2822  click.argument("
+000150b0: 6f72 6967 696e 616c 2229 0a40 636c 6963  original").@clic
+000150c0: 6b2e 6172 6775 6d65 6e74 2822 6e65 775f  k.argument("new_
+000150d0: 6e61 6d65 2229 0a64 6566 2072 656e 616d  name").def renam
+000150e0: 6528 6f72 6967 696e 616c 2c20 6e65 775f  e(original, new_
+000150f0: 6e61 6d65 2c20 7265 6e61 6d69 6e67 5f74  name, renaming_t
+00015100: 6167 293a 0a20 2020 2022 2222 0a20 2020  ag):.    """.   
+00015110: 2052 656e 616d 6520 6120 736f 6e67 2e0a   Rename a song..
+00015120: 0a20 2020 2052 656e 616d 6573 2074 6865  .    Renames the
+00015130: 2073 6f6e 6720 7769 7468 2074 6865 2049   song with the I
+00015140: 4420 4f52 4947 494e 414c 2074 6f20 4e45  D ORIGINAL to NE
+00015150: 575f 4e41 4d45 2e20 5468 6520 6578 7465  W_NAME. The exte
+00015160: 6e73 696f 6e20 6f66 2074 6865 0a20 2020  nsion of the.   
+00015170: 2073 6f6e 6720 2865 2e67 2e20 272e 7761   song (e.g. '.wa
+00015180: 7627 2c20 272e 6d70 3327 2920 6973 2070  v', '.mp3') is p
+00015190: 7265 7365 7276 6564 e280 9464 6f20 6e6f  reserved...do no
+000151a0: 7420 696e 636c 7564 6520 6974 2069 6e20  t include it in 
+000151b0: 7468 6520 6e61 6d65 2e0a 0a20 2020 2049  the name...    I
+000151c0: 6620 7468 6520 272d 542f 2d2d 7461 6727  f the '-T/--tag'
+000151d0: 2066 6c61 6720 6973 2070 6173 7365 642c   flag is passed,
+000151e0: 2074 7265 6174 7320 4f52 4947 494e 414c   treats ORIGINAL
+000151f0: 2061 7320 6120 7461 672c 2072 656e 616d   as a tag, renam
+00015200: 696e 6720 616c 6c0a 2020 2020 6f63 7572  ing all.    ocur
+00015210: 7265 6e63 6573 206f 6620 6974 2074 6f20  rences of it to 
+00015220: 4e45 575f 4e41 4d45 e280 9464 6f65 736e  NEW_NAME...doesn
+00015230: 2774 2063 6865 636b 2069 6620 7468 6520  't check if the 
+00015240: 7461 6720 4e45 575f 4e41 4d45 2061 6c72  tag NEW_NAME alr
+00015250: 6561 6479 2c0a 2020 2020 6578 6973 7473  eady,.    exists
+00015260: 2c20 736f 2062 6520 6361 7265 6675 6c21  , so be careful!
+00015270: 0a20 2020 2022 2222 0a20 2020 2073 6f6e  .    """.    son
+00015280: 6773 5f66 696c 6520 3d20 6f70 656e 2853  gs_file = open(S
+00015290: 4f4e 4753 5f49 4e46 4f5f 5041 5448 2c20  ONGS_INFO_PATH, 
+000152a0: 2272 222c 2065 6e63 6f64 696e 673d 2275  "r", encoding="u
+000152b0: 7466 2d38 2229 0a20 2020 206c 696e 6573  tf-8").    lines
+000152c0: 203d 2073 6f6e 6773 5f66 696c 652e 7265   = songs_file.re
+000152d0: 6164 2829 2e73 706c 6974 6c69 6e65 7328  ad().splitlines(
+000152e0: 290a 2020 2020 6966 206e 6f74 2072 656e  ).    if not ren
+000152f0: 616d 696e 675f 7461 673a 0a20 2020 2020  aming_tag:.     
+00015300: 2020 2069 6620 6e6f 7420 6f72 6967 696e     if not origin
+00015310: 616c 2e69 736e 756d 6572 6963 2829 3a0a  al.isnumeric():.
+00015320: 2020 2020 2020 2020 2020 2020 636c 6963              clic
+00015330: 6b2e 7365 6368 6f28 0a20 2020 2020 2020  k.secho(.       
+00015340: 2020 2020 2020 2020 2022 536f 6e67 2049           "Song I
+00015350: 4420 6d75 7374 2062 6520 616e 2069 6e74  D must be an int
+00015360: 6567 6572 2e20 546f 2072 656e 616d 6520  eger. To rename 
+00015370: 6120 7461 672c 2070 6173 7320 7468 6520  a tag, pass the 
+00015380: 272d 542f 2d2d 7461 6727 2066 6c61 672e  '-T/--tag' flag.
+00015390: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+000153a0: 2020 2066 673d 2272 6564 222c 0a20 2020     fg="red",.   
+000153b0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+000153c0: 2020 2020 2020 2072 6574 7572 6e0a 0a20         return.. 
+000153d0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+000153e0: 7261 6e67 6528 6c65 6e28 6c69 6e65 7329  range(len(lines)
+000153f0: 293a 0a20 2020 2020 2020 2020 2020 2064  ):.            d
+00015400: 6574 6169 6c73 203d 206c 696e 6573 5b69  etails = lines[i
+00015410: 5d2e 7374 7269 7028 292e 7370 6c69 7428  ].strip().split(
+00015420: 227c 2229 0a20 2020 2020 2020 2020 2020  "|").           
+00015430: 2069 6620 6f73 2e70 6174 682e 7370 6c69   if os.path.spli
+00015440: 7465 7874 2864 6574 6169 6c73 5b31 5d29  text(details[1])
+00015450: 5b30 5d20 3d3d 206e 6577 5f6e 616d 653a  [0] == new_name:
+00015460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015470: 2063 6c69 636b 2e73 6563 686f 280a 2020   click.secho(.  
+00015480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015490: 2020 6622 4120 736f 6e67 2077 6974 6820    f"A song with 
+000154a0: 7468 6520 6e61 6d65 2027 7b6e 6577 5f6e  the name '{new_n
+000154b0: 616d 657d 2720 616c 7265 6164 7920 6578  ame}' already ex
+000154c0: 6973 7473 2e20 506c 6561 7365 2063 686f  ists. Please cho
+000154d0: 6f73 6520 616e 6f74 6865 7220 6e61 6d65  ose another name
+000154e0: 2e22 2c0a 2020 2020 2020 2020 2020 2020  .",.            
+000154f0: 2020 2020 2020 2020 6667 3d22 7265 6422          fg="red"
+00015500: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00015510: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00015520: 2020 2020 7265 7475 726e 0a0a 2020 2020      return..    
+00015530: 2020 2020 6f72 6967 696e 616c 203d 2069      original = i
+00015540: 6e74 286f 7269 6769 6e61 6c29 0a20 2020  nt(original).   
+00015550: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
+00015560: 6e67 6528 6c65 6e28 6c69 6e65 7329 293a  nge(len(lines)):
+00015570: 0a20 2020 2020 2020 2020 2020 2064 6574  .            det
+00015580: 6169 6c73 203d 206c 696e 6573 5b69 5d2e  ails = lines[i].
+00015590: 7374 7269 7028 292e 7370 6c69 7428 227c  strip().split("|
+000155a0: 2229 0a20 2020 2020 2020 2020 2020 2069  ").            i
+000155b0: 6620 696e 7428 6465 7461 696c 735b 305d  f int(details[0]
+000155c0: 2920 3d3d 206f 7269 6769 6e61 6c3a 0a20  ) == original:. 
+000155d0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+000155e0: 6c64 5f70 6174 6820 3d20 6465 7461 696c  ld_path = detail
+000155f0: 735b 315d 0a20 2020 2020 2020 2020 2020  s[1].           
+00015600: 2020 2020 2064 6574 6169 6c73 5b31 5d20       details[1] 
+00015610: 3d20 6e65 775f 6e61 6d65 202b 206f 732e  = new_name + os.
+00015620: 7061 7468 2e73 706c 6974 6578 7428 6f6c  path.splitext(ol
+00015630: 645f 7061 7468 295b 315d 0a0a 2020 2020  d_path)[1]..    
+00015640: 2020 2020 2020 2020 2020 2020 6c69 6e65              line
+00015650: 735b 695d 203d 2022 7c22 2e6a 6f69 6e28  s[i] = "|".join(
+00015660: 6465 7461 696c 7329 0a20 2020 2020 2020  details).       
+00015670: 2020 2020 2020 2020 2073 6f6e 6773 5f66           songs_f
+00015680: 696c 652e 636c 6f73 6528 290a 2020 2020  ile.close().    
+00015690: 2020 2020 2020 2020 2020 2020 736f 6e67              song
+000156a0: 735f 6669 6c65 203d 206f 7065 6e28 534f  s_file = open(SO
+000156b0: 4e47 535f 494e 464f 5f50 4154 482c 2022  NGS_INFO_PATH, "
+000156c0: 7722 2c20 656e 636f 6469 6e67 3d22 7574  w", encoding="ut
+000156d0: 662d 3822 290a 2020 2020 2020 2020 2020  f-8").          
+000156e0: 2020 2020 2020 736f 6e67 735f 6669 6c65        songs_file
+000156f0: 2e77 7269 7465 2822 5c6e 222e 6a6f 696e  .write("\n".join
+00015700: 286c 696e 6573 2929 0a0a 2020 2020 2020  (lines))..      
+00015710: 2020 2020 2020 2020 2020 6f73 2e72 656e            os.ren
+00015720: 616d 6528 0a20 2020 2020 2020 2020 2020  ame(.           
+00015730: 2020 2020 2020 2020 206f 732e 7061 7468           os.path
+00015740: 2e6a 6f69 6e28 534f 4e47 535f 4449 522c  .join(SONGS_DIR,
+00015750: 206f 6c64 5f70 6174 6829 2c0a 2020 2020   old_path),.    
+00015760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015770: 6f73 2e70 6174 682e 6a6f 696e 2853 4f4e  os.path.join(SON
+00015780: 4753 5f44 4952 2c20 6465 7461 696c 735b  GS_DIR, details[
+00015790: 315d 292c 0a20 2020 2020 2020 2020 2020  1]),.           
+000157a0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+000157b0: 2020 2020 2020 2020 636c 6963 6b2e 7365          click.se
+000157c0: 6368 6f28 0a20 2020 2020 2020 2020 2020  cho(.           
+000157d0: 2020 2020 2020 2020 2066 2252 656e 616d           f"Renam
+000157e0: 6564 2073 6f6e 6720 277b 6f6c 645f 7061  ed song '{old_pa
+000157f0: 7468 7d27 2077 6974 6820 4944 207b 6f72  th}' with ID {or
+00015800: 6967 696e 616c 7d20 746f 2027 7b64 6574  iginal} to '{det
+00015810: 6169 6c73 5b31 5d7d 272e 222c 0a20 2020  ails[1]}'.",.   
+00015820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015830: 2066 673d 2267 7265 656e 222c 0a20 2020   fg="green",.   
+00015840: 2020 2020 2020 2020 2020 2020 2029 0a0a               )..
+00015850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015860: 6272 6561 6b0a 2020 2020 2020 2020 656c  break.        el
+00015870: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00015880: 636c 6963 6b2e 7365 6368 6f28 6622 536f  click.secho(f"So
+00015890: 6e67 2077 6974 6820 4944 207b 6f72 6967  ng with ID {orig
+000158a0: 696e 616c 7d20 6e6f 7420 666f 756e 642e  inal} not found.
+000158b0: 222c 2066 673d 2272 6564 2229 0a20 2020  ", fg="red").   
+000158c0: 2020 2020 2020 2020 2073 6f6e 6773 5f66           songs_f
+000158d0: 696c 652e 636c 6f73 6528 290a 2020 2020  ile.close().    
+000158e0: 656c 7365 3a0a 2020 2020 2020 2020 666f  else:.        fo
+000158f0: 7220 6920 696e 2072 616e 6765 286c 656e  r i in range(len
+00015900: 286c 696e 6573 2929 3a0a 2020 2020 2020  (lines)):.      
+00015910: 2020 2020 2020 6465 7461 696c 7320 3d20        details = 
+00015920: 6c69 6e65 735b 695d 2e73 7472 6970 2829  lines[i].strip()
+00015930: 2e73 706c 6974 2822 7c22 290a 2020 2020  .split("|").    
+00015940: 2020 2020 2020 2020 7461 6773 203d 2064          tags = d
+00015950: 6574 6169 6c73 5b32 5d2e 7370 6c69 7428  etails[2].split(
+00015960: 222c 2229 0a20 2020 2020 2020 2020 2020  ",").           
+00015970: 2066 6f72 2074 2069 6e20 7261 6e67 6528   for t in range(
+00015980: 6c65 6e28 7461 6773 2929 3a0a 2020 2020  len(tags)):.    
+00015990: 2020 2020 2020 2020 2020 2020 6966 2074              if t
+000159a0: 6167 735b 745d 203d 3d20 6f72 6967 696e  ags[t] == origin
+000159b0: 616c 3a0a 2020 2020 2020 2020 2020 2020  al:.            
+000159c0: 2020 2020 2020 2020 7461 6773 5b74 5d20          tags[t] 
+000159d0: 3d20 6e65 775f 6e61 6d65 0a20 2020 2020  = new_name.     
+000159e0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+000159f0: 6574 6169 6c73 5b32 5d20 3d20 222c 222e  etails[2] = ",".
+00015a00: 6a6f 696e 2874 6167 7329 0a0a 2020 2020  join(tags)..    
+00015a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015a20: 6c69 6e65 735b 695d 203d 2022 7c22 2e6a  lines[i] = "|".j
+00015a30: 6f69 6e28 6465 7461 696c 7329 0a20 2020  oin(details).   
+00015a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015a50: 2062 7265 616b 0a0a 2020 2020 2020 2020   break..        
+00015a60: 736f 6e67 735f 6669 6c65 2e63 6c6f 7365  songs_file.close
+00015a70: 2829 0a20 2020 2020 2020 2073 6f6e 6773  ().        songs
+00015a80: 5f66 696c 6520 3d20 6f70 656e 2853 4f4e  _file = open(SON
+00015a90: 4753 5f49 4e46 4f5f 5041 5448 2c20 2277  GS_INFO_PATH, "w
+00015aa0: 222c 2065 6e63 6f64 696e 673d 2275 7466  ", encoding="utf
+00015ab0: 2d38 2229 0a20 2020 2020 2020 2073 6f6e  -8").        son
+00015ac0: 6773 5f66 696c 652e 7772 6974 6528 225c  gs_file.write("\
+00015ad0: 6e22 2e6a 6f69 6e28 6c69 6e65 7329 290a  n".join(lines)).
+00015ae0: 0a20 2020 2020 2020 2063 6c69 636b 2e73  .        click.s
+00015af0: 6563 686f 280a 2020 2020 2020 2020 2020  echo(.          
+00015b00: 2020 6622 5265 706c 6163 6564 2061 6c6c    f"Replaced all
+00015b10: 206f 6375 7272 656e 6365 7320 6f66 2074   ocurrences of t
+00015b20: 6167 2027 7b6f 7269 6769 6e61 6c7d 2720  ag '{original}' 
+00015b30: 746f 2027 7b6e 6577 5f6e 616d 657d 272e  to '{new_name}'.
+00015b40: 222c 0a20 2020 2020 2020 2020 2020 2066  ",.            f
+00015b50: 673d 2267 7265 656e 222c 0a20 2020 2020  g="green",.     
+00015b60: 2020 2029 0a0a 0a40 636c 692e 636f 6d6d     )...@cli.comm
+00015b70: 616e 6428 290a 4063 6c69 636b 2e61 7267  and().@click.arg
+00015b80: 756d 656e 7428 2270 6872 6173 6522 290a  ument("phrase").
+00015b90: 4063 6c69 636b 2e6f 7074 696f 6e28 0a20  @click.option(. 
+00015ba0: 2020 2022 2d54 2f2d 6e54 222c 0a20 2020     "-T/-nT",.   
+00015bb0: 2022 2d2d 7461 672f 2d2d 6e6f 2d74 6167   "--tag/--no-tag
+00015bc0: 222c 0a20 2020 2022 7365 6172 6368 696e  ",.    "searchin
+00015bd0: 675f 666f 725f 7461 6773 222c 0a20 2020  g_for_tags",.   
+00015be0: 2064 6566 6175 6c74 3d46 616c 7365 2c0a   default=False,.
+00015bf0: 2020 2020 6865 6c70 3d22 5365 6172 6368      help="Search
+00015c00: 6573 2066 6f72 206d 6174 6368 696e 6720  es for matching 
+00015c10: 7461 6773 2069 6e73 7465 6164 206f 6620  tags instead of 
+00015c20: 736f 6e67 206e 616d 6573 2e22 2c0a 290a  song names.",.).
+00015c30: 6465 6620 7365 6172 6368 2870 6872 6173  def search(phras
+00015c40: 652c 2073 6561 7263 6869 6e67 5f66 6f72  e, searching_for
+00015c50: 5f74 6167 7329 3a0a 2020 2020 2222 2253  _tags):.    """S
+00015c60: 6561 7263 6865 7320 666f 7220 736f 6e67  earches for song
+00015c70: 7320 7468 6174 2063 6f6e 7461 696e 2050  s that contain P
+00015c80: 4852 4153 452e 2041 6c6c 2073 6f6e 6773  HRASE. All songs
+00015c90: 2073 7461 7274 696e 6720 7769 7468 2050   starting with P
+00015ca0: 4852 4153 450a 2020 2020 7769 6c6c 2061  HRASE.    will a
+00015cb0: 7070 6561 7220 6265 666f 7265 2073 6f6e  ppear before son
+00015cc0: 6773 2063 6f6e 7461 696e 696e 6720 6275  gs containing bu
+00015cd0: 7420 6e6f 7420 7374 6172 7469 6e67 2077  t not starting w
+00015ce0: 6974 6820 5048 5241 5345 2e20 5468 6973  ith PHRASE. This
+00015cf0: 0a20 2020 2073 6561 7263 6820 6973 2063  .    search is c
+00015d00: 6173 652d 696e 7365 6e73 6974 6976 652e  ase-insensitive.
+00015d10: 0a0a 2020 2020 4966 2074 6865 2027 2d54  ..    If the '-T
+00015d20: 2720 666c 6167 2069 7320 7061 7373 6564  ' flag is passed
+00015d30: 2c20 7365 6172 6368 6573 2066 6f72 2074  , searches for t
+00015d40: 6167 7320 696e 7374 6561 6420 6f66 2073  ags instead of s
+00015d50: 6f6e 6720 6e61 6d65 732e 2222 220a 2020  ong names.""".  
+00015d60: 2020 7068 7261 7365 203d 2070 6872 6173    phrase = phras
+00015d70: 652e 6c6f 7765 7228 290a 2020 2020 7769  e.lower().    wi
+00015d80: 7468 206f 7065 6e28 534f 4e47 535f 494e  th open(SONGS_IN
+00015d90: 464f 5f50 4154 482c 2022 7222 2c20 656e  FO_PATH, "r", en
+00015da0: 636f 6469 6e67 3d22 7574 662d 3822 2920  coding="utf-8") 
+00015db0: 6173 2073 6f6e 6773 5f66 696c 653a 0a20  as songs_file:. 
+00015dc0: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
+00015dd0: 6172 6368 696e 675f 666f 725f 7461 6773  arching_for_tags
+00015de0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00015df0: 7375 6c74 7320 3d20 5b5d 2c20 5b5d 2020  sults = [], []  
+00015e00: 2320 7374 6172 7473 2c20 636f 6e74 6169  # starts, contai
+00015e10: 6e73 2062 7574 2064 6f65 7320 6e6f 7420  ns but does not 
+00015e20: 7374 6172 740a 2020 2020 2020 2020 2020  start.          
+00015e30: 2020 666f 7220 6c69 6e65 2069 6e20 736f    for line in so
+00015e40: 6e67 735f 6669 6c65 3a0a 2020 2020 2020  ngs_file:.      
+00015e50: 2020 2020 2020 2020 2020 736f 6e67 5f69            song_i
+00015e60: 642c 2073 6f6e 675f 6e61 6d65 2c20 7461  d, song_name, ta
+00015e70: 6773 2c20 2a5f 203d 206c 696e 652e 7374  gs, *_ = line.st
+00015e80: 7269 7028 292e 7370 6c69 7428 227c 2229  rip().split("|")
+00015e90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015ea0: 2073 6f6e 675f 6964 203d 2069 6e74 2873   song_id = int(s
+00015eb0: 6f6e 675f 6964 290a 2020 2020 2020 2020  ong_id).        
+00015ec0: 2020 2020 2020 2020 736f 6e67 5f6e 616d          song_nam
+00015ed0: 6520 3d20 736f 6e67 5f6e 616d 652e 6c6f  e = song_name.lo
+00015ee0: 7765 7228 290a 0a20 2020 2020 2020 2020  wer()..         
+00015ef0: 2020 2020 2020 2069 6620 736f 6e67 5f6e         if song_n
+00015f00: 616d 652e 7374 6172 7473 7769 7468 2870  ame.startswith(p
+00015f10: 6872 6173 6529 3a0a 2020 2020 2020 2020  hrase):.        
+00015f20: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00015f30: 6c74 735b 305d 2e61 7070 656e 6428 736f  lts[0].append(so
+00015f40: 6e67 5f69 6429 0a20 2020 2020 2020 2020  ng_id).         
+00015f50: 2020 2020 2020 2065 6c69 6620 7068 7261         elif phra
+00015f60: 7365 2069 6e20 736f 6e67 5f6e 616d 653a  se in song_name:
+00015f70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015f80: 2020 2020 2072 6573 756c 7473 5b31 5d2e       results[1].
+00015f90: 6170 7065 6e64 2873 6f6e 675f 6964 290a  append(song_id).
+00015fa0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00015fb0: 6e6f 7420 616e 7928 7265 7375 6c74 7329  not any(results)
+00015fc0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00015fd0: 2020 636c 6963 6b2e 7365 6368 6f28 224e    click.secho("N
+00015fe0: 6f20 7265 7375 6c74 7320 666f 756e 642e  o results found.
+00015ff0: 222c 2066 673d 2272 6564 2229 0a20 2020  ", fg="red").   
+00016000: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00016010: 7572 6e0a 0a20 2020 2020 2020 2020 2020  urn..           
+00016020: 2073 6f6e 6773 5f66 696c 652e 7365 656b   songs_file.seek
+00016030: 2830 290a 2020 2020 2020 2020 2020 2020  (0).            
+00016040: 666f 7220 6c69 6e65 2069 6e20 736f 6e67  for line in song
+00016050: 735f 6669 6c65 3a0a 2020 2020 2020 2020  s_file:.        
+00016060: 2020 2020 2020 2020 6465 7461 696c 7320          details 
+00016070: 3d20 6c69 6e65 2e73 7472 6970 2829 2e73  = line.strip().s
+00016080: 706c 6974 2822 7c22 290a 2020 2020 2020  plit("|").      
+00016090: 2020 2020 2020 2020 2020 6966 2069 6e74            if int
+000160a0: 2864 6574 6169 6c73 5b30 5d29 2069 6e20  (details[0]) in 
+000160b0: 7265 7375 6c74 735b 305d 3a0a 2020 2020  results[0]:.    
+000160c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000160d0: 7072 696e 745f 656e 7472 7928 6465 7461  print_entry(deta
+000160e0: 696c 732c 2070 6872 6173 6529 0a0a 2020  ils, phrase)..  
+000160f0: 2020 2020 2020 2020 2020 736f 6e67 735f            songs_
+00016100: 6669 6c65 2e73 6565 6b28 3029 0a20 2020  file.seek(0).   
+00016110: 2020 2020 2020 2020 2066 6f72 206c 696e           for lin
+00016120: 6520 696e 2073 6f6e 6773 5f66 696c 653a  e in songs_file:
+00016130: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016140: 2064 6574 6169 6c73 203d 206c 696e 652e   details = line.
+00016150: 7374 7269 7028 292e 7370 6c69 7428 227c  strip().split("|
+00016160: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+00016170: 2020 2069 6620 696e 7428 6465 7461 696c     if int(detail
+00016180: 735b 305d 2920 696e 2072 6573 756c 7473  s[0]) in results
+00016190: 5b31 5d3a 0a20 2020 2020 2020 2020 2020  [1]:.           
+000161a0: 2020 2020 2020 2020 2070 7269 6e74 5f65           print_e
+000161b0: 6e74 7279 2864 6574 6169 6c73 2c20 7068  ntry(details, ph
+000161c0: 7261 7365 290a 0a20 2020 2020 2020 2020  rase)..         
+000161d0: 2020 2063 6c69 636b 2e73 6563 686f 280a     click.secho(.
+000161e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000161f0: 6622 466f 756e 6420 7b6c 656e 2872 6573  f"Found {len(res
+00016200: 756c 7473 5b30 5d29 202b 206c 656e 2872  ults[0]) + len(r
+00016210: 6573 756c 7473 5b31 5d29 7d20 736f 6e67  esults[1])} song
+00016220: 2873 292e 222c 0a20 2020 2020 2020 2020  (s).",.         
+00016230: 2020 2020 2020 2066 673d 2267 7265 656e         fg="green
+00016240: 222c 0a20 2020 2020 2020 2020 2020 2029  ",.            )
+00016250: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00016260: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00016270: 7473 203d 2073 6574 2829 2c20 7365 7428  ts = set(), set(
+00016280: 2920 2023 2073 7461 7274 732c 2063 6f6e  )  # starts, con
+00016290: 7461 696e 7320 6275 7420 646f 6573 206e  tains but does n
+000162a0: 6f74 2073 7461 7274 0a20 2020 2020 2020  ot start.       
+000162b0: 2020 2020 2066 6f72 206c 696e 6520 696e       for line in
+000162c0: 2073 6f6e 6773 5f66 696c 653a 0a20 2020   songs_file:.   
+000162d0: 2020 2020 2020 2020 2020 2020 2073 6f6e               son
+000162e0: 675f 6964 2c20 736f 6e67 5f6e 616d 652c  g_id, song_name,
+000162f0: 2074 6167 732c 202a 5f20 3d20 6c69 6e65   tags, *_ = line
+00016300: 2e73 7472 6970 2829 2e73 706c 6974 2822  .strip().split("
+00016310: 7c22 290a 2020 2020 2020 2020 2020 2020  |").            
+00016320: 2020 2020 6966 2074 6167 733a 0a20 2020      if tags:.   
+00016330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016340: 2074 6167 7320 3d20 7461 6773 2e73 706c   tags = tags.spl
+00016350: 6974 2822 2c22 290a 0a20 2020 2020 2020  it(",")..       
+00016360: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00016370: 2074 6167 2069 6e20 7461 6773 3a0a 2020   tag in tags:.  
+00016380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016390: 2020 2020 2020 7461 675f 6c6f 7765 7220        tag_lower 
+000163a0: 3d20 7461 672e 6c6f 7765 7228 290a 2020  = tag.lower().  
+000163b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000163c0: 2020 2020 2020 6966 2074 6167 5f6c 6f77        if tag_low
+000163d0: 6572 2e73 7461 7274 7377 6974 6828 7068  er.startswith(ph
+000163e0: 7261 7365 293a 0a20 2020 2020 2020 2020  rase):.         
+000163f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016400: 2020 2072 6573 756c 7473 5b30 5d2e 6164     results[0].ad
+00016410: 6428 7461 6729 0a20 2020 2020 2020 2020  d(tag).         
+00016420: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00016430: 6c69 6620 7068 7261 7365 2069 6e20 7461  lif phrase in ta
+00016440: 675f 6c6f 7765 723a 0a20 2020 2020 2020  g_lower:.       
+00016450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016460: 2020 2020 2072 6573 756c 7473 5b31 5d2e       results[1].
+00016470: 6164 6428 7461 6729 0a0a 2020 2020 2020  add(tag)..      
+00016480: 2020 2020 2020 6966 206e 6f74 2061 6e79        if not any
+00016490: 2872 6573 756c 7473 293a 0a20 2020 2020  (results):.     
+000164a0: 2020 2020 2020 2020 2020 2063 6c69 636b             click
+000164b0: 2e73 6563 686f 2822 4e6f 2072 6573 756c  .secho("No resul
+000164c0: 7473 2066 6f75 6e64 2e22 2c20 6667 3d22  ts found.", fg="
+000164d0: 7265 6422 290a 2020 2020 2020 2020 2020  red").          
+000164e0: 2020 2020 2020 7265 7475 726e 0a0a 2020        return..  
+000164f0: 2020 2020 2020 2020 2020 666f 7220 7461            for ta
+00016500: 6720 696e 2072 6573 756c 7473 5b30 5d3a  g in results[0]:
+00016510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016520: 2070 7269 6e74 2874 6167 290a 0a20 2020   print(tag)..   
+00016530: 2020 2020 2020 2020 2066 6f72 2074 6167           for tag
+00016540: 2069 6e20 7265 7375 6c74 735b 315d 3a0a   in results[1]:.
+00016550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016560: 7072 696e 7428 7461 6729 0a0a 2020 2020  print(tag)..    
+00016570: 2020 2020 2020 2020 636c 6963 6b2e 7365          click.se
+00016580: 6368 6f28 0a20 2020 2020 2020 2020 2020  cho(.           
+00016590: 2020 2020 2066 2246 6f75 6e64 207b 6c65       f"Found {le
+000165a0: 6e28 7265 7375 6c74 735b 305d 2920 2b20  n(results[0]) + 
+000165b0: 6c65 6e28 7265 7375 6c74 735b 315d 297d  len(results[1])}
+000165c0: 2074 6167 2873 292e 222c 2066 673d 2267   tag(s).", fg="g
+000165d0: 7265 656e 220a 2020 2020 2020 2020 2020  reen".          
+000165e0: 2020 290a 0a0a 4063 6c69 2e63 6f6d 6d61    )...@cli.comma
+000165f0: 6e64 286e 616d 653d 226c 6973 7422 290a  nd(name="list").
+00016600: 4063 6c69 636b 2e61 7267 756d 656e 7428  @click.argument(
+00016610: 2273 6561 7263 685f 7461 6773 222c 206d  "search_tags", m
+00016620: 6574 6176 6172 3d22 5441 4753 222c 206e  etavar="TAGS", n
+00016630: 6172 6773 3d2d 3129 0a40 636c 6963 6b2e  args=-1).@click.
+00016640: 6f70 7469 6f6e 280a 2020 2020 222d 7322  option(.    "-s"
+00016650: 2c0a 2020 2020 222d 2d73 6f72 7422 2c0a  ,.    "--sort",.
+00016660: 2020 2020 2273 6f72 745f 222c 0a20 2020      "sort_",.   
+00016670: 2074 7970 653d 636c 6963 6b2e 4368 6f69   type=click.Choi
+00016680: 6365 280a 2020 2020 2020 2020 280a 2020  ce(.        (.  
+00016690: 2020 2020 2020 2020 2020 226e 6f6e 6522            "none"
+000166a0: 2c0a 2020 2020 2020 2020 2020 2020 226e  ,.            "n
+000166b0: 616d 6522 2c0a 2020 2020 2020 2020 2020  ame",.          
+000166c0: 2020 226e 222c 0a20 2020 2020 2020 2020    "n",.         
+000166d0: 2020 2022 7365 6373 2d6c 6973 7465 6e65     "secs-listene
+000166e0: 6422 2c0a 2020 2020 2020 2020 2020 2020  d",.            
+000166f0: 2273 222c 0a20 2020 2020 2020 2020 2020  "s",.           
+00016700: 2022 6475 7261 7469 6f6e 222c 0a20 2020   "duration",.   
+00016710: 2020 2020 2020 2020 2022 6422 2c0a 2020           "d",.  
+00016720: 2020 2020 2020 2020 2020 2274 696d 6573            "times
+00016730: 2d6c 6973 7465 6e65 6422 2c0a 2020 2020  -listened",.    
+00016740: 2020 2020 2020 2020 2274 222c 0a20 2020          "t",.   
+00016750: 2020 2020 2029 0a20 2020 2029 2c0a 2020       ).    ),.  
+00016760: 2020 6865 6c70 3d22 536f 7274 2062 7920    help="Sort by 
+00016770: 6e61 6d65 2c20 7365 636f 6e64 7320 6c69  name, seconds li
+00016780: 7374 656e 6564 2c20 6f72 2074 696d 6573  stened, or times
+00016790: 206c 6973 7465 6e65 6420 2873 6563 6f6e   listened (secon
+000167a0: 6473 2f73 6f6e 6720 6475 7261 7469 6f6e  ds/song duration
+000167b0: 292e 2047 7265 6174 6573 7420 6669 7273  ). Greatest firs
+000167c0: 742e 222c 0a20 2020 2064 6566 6175 6c74  t.",.    default
+000167d0: 3d22 6e6f 6e65 222c 0a20 2020 2073 686f  ="none",.    sho
+000167e0: 775f 6465 6661 756c 743d 5472 7565 2c0a  w_default=True,.
+000167f0: 290a 4063 6c69 636b 2e6f 7074 696f 6e28  ).@click.option(
+00016800: 0a20 2020 2022 2d52 2f2d 6e52 222c 0a20  .    "-R/-nR",. 
+00016810: 2020 2022 2d2d 7265 7665 7273 652f 2d2d     "--reverse/--
+00016820: 6e6f 2d72 6576 6572 7365 222c 0a20 2020  no-reverse",.   
+00016830: 2022 7265 7665 7273 655f 222c 0a20 2020   "reverse_",.   
+00016840: 2064 6566 6175 6c74 3d46 616c 7365 2c0a   default=False,.
+00016850: 2020 2020 6865 6c70 3d22 5265 7665 7273      help="Revers
+00016860: 6520 7468 6520 736f 7274 696e 6720 6f72  e the sorting or
+00016870: 6465 7220 2867 7265 6174 6573 7420 6669  der (greatest fi
+00016880: 7273 7429 2e22 2c0a 290a 4063 6c69 636b  rst).",.).@click
+00016890: 2e6f 7074 696f 6e28 0a20 2020 2022 2d54  .option(.    "-T
+000168a0: 2f2d 6e54 222c 0a20 2020 2022 2d2d 7461  /-nT",.    "--ta
+000168b0: 672f 2d2d 6e6f 2d74 6167 222c 0a20 2020  g/--no-tag",.   
+000168c0: 2022 6c69 7374 696e 675f 7461 6773 222c   "listing_tags",
+000168d0: 0a20 2020 2064 6566 6175 6c74 3d46 616c  .    default=Fal
+000168e0: 7365 2c0a 2020 2020 6865 6c70 3d22 4c69  se,.    help="Li
+000168f0: 7374 2074 6167 7320 6d61 7463 6869 6e67  st tags matching
+00016900: 2054 4147 5320 696e 7374 6561 6420 6f66   TAGS instead of
+00016910: 2073 6f6e 6773 2e22 2c0a 290a 4063 6c69   songs.",.).@cli
+00016920: 636b 2e6f 7074 696f 6e28 0a20 2020 2022  ck.option(.    "
+00016930: 2d79 222c 0a20 2020 2022 2d2d 7965 6172  -y",.    "--year
+00016940: 222c 0a20 2020 2022 7965 6172 222c 0a20  ",.    "year",. 
+00016950: 2020 2068 656c 703d 2253 686f 7720 7469     help="Show ti
+00016960: 6d65 206c 6973 7465 6e65 6420 666f 7220  me listened for 
+00016970: 6120 7370 6563 6966 6963 2079 6561 722c  a specific year,
+00016980: 2069 6e73 7465 6164 206f 6620 7468 6520   instead of the 
+00016990: 746f 7461 6c2e 2050 6173 7369 6e67 2027  total. Passing '
+000169a0: 6375 7227 2077 696c 6c20 7368 6f77 2074  cur' will show t
+000169b0: 6865 2074 696d 6520 6c69 7374 656e 6564  he time listened
+000169c0: 2066 6f72 2074 6865 2063 7572 7265 6e74   for the current
+000169d0: 2079 6561 722e 222c 0a29 0a40 636c 6963   year.",.).@clic
+000169e0: 6b2e 6f70 7469 6f6e 2822 2d74 222c 2022  k.option("-t", "
+000169f0: 2d2d 746f 7022 2c20 2274 6f70 222c 2074  --top", "top", t
+00016a00: 7970 653d 696e 742c 2068 656c 703d 2253  ype=int, help="S
+00016a10: 686f 7720 7468 6520 746f 7020 6e20 736f  how the top n so
+00016a20: 6e67 732f 7461 6773 2e22 290a 4063 6c69  ngs/tags.").@cli
+00016a30: 636b 2e6f 7074 696f 6e28 0a20 2020 2022  ck.option(.    "
+00016a40: 2d4d 2f2d 6e4d 222c 0a20 2020 2022 2d2d  -M/-nM",.    "--
+00016a50: 6d61 7463 682d 616c 6c2f 2d2d 6e6f 2d6d  match-all/--no-m
+00016a60: 6174 6368 2d61 6c6c 222c 0a20 2020 2022  atch-all",.    "
+00016a70: 6d61 7463 685f 616c 6c22 2c0a 2020 2020  match_all",.    
+00016a80: 6465 6661 756c 743d 4661 6c73 652c 0a20  default=False,. 
+00016a90: 2020 2068 656c 703d 2253 686f 7773 2073     help="Shows s
+00016aa0: 6f6e 6773 2074 6861 7420 6d61 7463 6820  ongs that match 
+00016ab0: 616c 6c20 7461 6773 2069 6e73 7465 6164  all tags instead
+00016ac0: 206f 6620 616e 7920 7461 672e 2049 676e   of any tag. Ign
+00016ad0: 6f72 6564 2069 6620 272d 742f 2d2d 7461  ored if '-t/--ta
+00016ae0: 6727 2069 7320 7061 7373 6564 2e22 2c0a  g' is passed.",.
+00016af0: 290a 6465 6620 6c69 7374 5f28 7365 6172  ).def list_(sear
+00016b00: 6368 5f74 6167 732c 206c 6973 7469 6e67  ch_tags, listing
+00016b10: 5f74 6167 732c 2079 6561 722c 2073 6f72  _tags, year, sor
+00016b20: 745f 2c20 746f 702c 2072 6576 6572 7365  t_, top, reverse
+00016b30: 5f2c 206d 6174 6368 5f61 6c6c 293a 0a20  _, match_all):. 
+00016b40: 2020 2022 2222 4c69 7374 2074 6865 2065     """List the e
+00016b50: 6e74 7269 6573 2066 6f72 2061 6c6c 2073  ntries for all s
+00016b60: 6f6e 6773 2e0a 0a20 2020 204f 7574 7075  ongs...    Outpu
+00016b70: 7420 666f 726d 6174 3a20 4944 2c20 6e61  t format: ID, na
+00016b80: 6d65 2c20 6475 7261 7469 6f6e 2c20 6c69  me, duration, li
+00016b90: 7374 656e 2074 696d 652c 2074 696d 6573  sten time, times
+00016ba0: 206c 6973 7465 6e65 642c 205b 636c 6970   listened, [clip
+00016bb0: 2d73 7461 7274 2c20 636c 6970 2d65 6e64  -start, clip-end
+00016bc0: 5d20 6966 2063 6c69 7020 6578 6973 7473  ] if clip exists
+00016bd0: 2c20 636f 6d6d 612d 7365 7061 7261 7465  , comma-separate
+00016be0: 6420 7461 6773 2069 6620 616e 790a 0a20  d tags if any.. 
+00016bf0: 2020 2049 6620 7468 6520 272d 5427 2066     If the '-T' f
+00016c00: 6c61 6720 6973 2070 6173 7365 642c 2074  lag is passed, t
+00016c10: 6167 7320 7769 6c6c 2062 6520 6c69 7374  ags will be list
+00016c20: 6564 2069 6e73 7465 6164 206f 6620 736f  ed instead of so
+00016c30: 6e67 732e 0a0a 2020 2020 4f75 7470 7574  ngs...    Output
+00016c40: 2066 6f72 6d61 743a 2074 6167 2c20 6475   format: tag, du
+00016c50: 7261 7469 6f6e 2c20 6c69 7374 656e 2074  ration, listen t
+00016c60: 696d 652c 2074 696d 6573 206c 6973 7465  ime, times liste
+00016c70: 6e65 640a 0a20 2020 2049 6620 5441 4753  ned..    If TAGS
+00016c80: 2061 7265 2070 6173 7365 642c 2061 6e79   are passed, any
+00016c90: 2074 6167 2f73 6f6e 6720 6d61 7463 6869   tag/song matchi
+00016ca0: 6e67 2061 6e79 2074 6167 2069 6e20 5441  ng any tag in TA
+00016cb0: 4753 2077 696c 6c20 6265 206c 6973 7465  GS will be liste
+00016cc0: 642c 0a20 2020 2075 6e6c 6573 7320 7468  d,.    unless th
+00016cd0: 6520 272d 4d2f 2d2d 6d61 7463 682d 616c  e '-M/--match-al
+00016ce0: 6c27 2066 6c61 6720 6973 2070 6173 7365  l' flag is passe
+00016cf0: 642c 2069 6e20 7768 6963 6820 6361 7365  d, in which case
+00016d00: 2065 7665 7279 2074 6167 206d 7573 740a   every tag must.
+00016d10: 2020 2020 6265 206d 6174 6368 6564 2028      be matched (
+00016d20: 6967 6e6f 7265 6420 6966 206c 6973 7469  ignored if listi
+00016d30: 6e67 2074 6167 7329 2e0a 2020 2020 2222  ng tags)..    ""
+00016d40: 220a 2020 2020 6966 2074 6f70 2069 7320  ".    if top is 
+00016d50: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00016d60: 2020 6966 2074 6f70 203c 2031 3a0a 2020    if top < 1:.  
+00016d70: 2020 2020 2020 2020 2020 636c 6963 6b2e            click.
+00016d80: 7365 6368 6f28 0a20 2020 2020 2020 2020  secho(.         
+00016d90: 2020 2020 2020 2022 5468 6520 6f70 7469         "The opti
+00016da0: 6f6e 2027 2d74 2f2d 2d74 6f70 2720 6d75  on '-t/--top' mu
+00016db0: 7374 2062 6520 6120 706f 7369 7469 7665  st be a positive
+00016dc0: 206e 756d 6265 722e 222c 2066 673d 2272   number.", fg="r
+00016dd0: 6564 220a 2020 2020 2020 2020 2020 2020  ed".            
+00016de0: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+00016df0: 7475 726e 0a0a 2020 2020 6966 2079 6561  turn..    if yea
+00016e00: 7220 6973 204e 6f6e 653a 0a20 2020 2020  r is None:.     
+00016e10: 2020 2073 7461 7473 5f70 6174 6820 3d20     stats_path = 
+00016e20: 544f 5441 4c5f 5354 4154 535f 5041 5448  TOTAL_STATS_PATH
+00016e30: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+00016e40: 2020 2069 6620 7965 6172 203d 3d20 2263     if year == "c
+00016e50: 7572 223a 0a20 2020 2020 2020 2020 2020  ur":.           
+00016e60: 2079 6561 7220 3d20 4355 525f 5945 4152   year = CUR_YEAR
+00016e70: 0a20 2020 2020 2020 2020 2020 2073 7461  .            sta
+00016e80: 7473 5f70 6174 6820 3d20 4355 525f 5945  ts_path = CUR_YE
+00016e90: 4152 5f53 5441 5453 5f50 4154 480a 2020  AR_STATS_PATH.  
+00016ea0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00016eb0: 2020 2020 2020 2020 6966 206e 6f74 2079          if not y
+00016ec0: 6561 722e 6973 6469 6769 7428 293a 0a20  ear.isdigit():. 
+00016ed0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00016ee0: 6c69 636b 2e73 6563 686f 2822 5965 6172  lick.secho("Year
+00016ef0: 206d 7573 7420 6265 2061 206e 756d 6265   must be a numbe
+00016f00: 7220 6f72 2027 6375 7227 2e22 2c20 6667  r or 'cur'.", fg
+00016f10: 3d22 7265 6422 290a 2020 2020 2020 2020  ="red").        
+00016f20: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+00016f30: 2020 2020 2020 2020 2020 2073 7461 7473             stats
+00016f40: 5f70 6174 6820 3d20 6f73 2e70 6174 682e  _path = os.path.
+00016f50: 6a6f 696e 2853 5441 5453 5f44 4952 2c20  join(STATS_DIR, 
+00016f60: 6622 7b79 6561 727d 2e74 7874 2229 0a20  f"{year}.txt"). 
+00016f70: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+00016f80: 7420 6f73 2e70 6174 682e 6578 6973 7473  t os.path.exists
+00016f90: 2873 7461 7473 5f70 6174 6829 3a0a 2020  (stats_path):.  
+00016fa0: 2020 2020 2020 2020 2020 2020 2020 636c                cl
+00016fb0: 6963 6b2e 7365 6368 6f28 6622 4e6f 2073  ick.secho(f"No s
+00016fc0: 7461 7473 2066 6f75 6e64 2066 6f72 2079  tats found for y
+00016fd0: 6561 7220 7b79 6561 727d 2e22 2c20 6667  ear {year}.", fg
+00016fe0: 3d22 7265 6422 290a 2020 2020 2020 2020  ="red").        
+00016ff0: 2020 2020 2020 2020 7265 7475 726e 0a0a          return..
+00017000: 2020 2020 6966 2073 6561 7263 685f 7461      if search_ta
+00017010: 6773 3a0a 2020 2020 2020 2020 7365 6172  gs:.        sear
+00017020: 6368 5f74 6167 7320 3d20 7365 7428 7365  ch_tags = set(se
+00017030: 6172 6368 5f74 6167 7329 0a0a 2020 2020  arch_tags)..    
+00017040: 6e75 6d5f 6c69 6e65 7320 3d20 300a 2020  num_lines = 0.  
+00017050: 2020 736f 6e67 735f 6e6f 745f 666f 756e    songs_not_foun
+00017060: 6420 3d20 5b5d 0a0a 2020 2020 6966 206c  d = []..    if l
+00017070: 6973 7469 6e67 5f74 6167 733a 0a20 2020  isting_tags:.   
+00017080: 2020 2020 2077 6974 6820 280a 2020 2020       with (.    
+00017090: 2020 2020 2020 2020 6f70 656e 2853 4f4e          open(SON
+000170a0: 4753 5f49 4e46 4f5f 5041 5448 2c20 2272  GS_INFO_PATH, "r
+000170b0: 222c 2065 6e63 6f64 696e 673d 2275 7466  ", encoding="utf
+000170c0: 2d38 2229 2061 7320 736f 6e67 735f 6669  -8") as songs_fi
+000170d0: 6c65 2c0a 2020 2020 2020 2020 2020 2020  le,.            
+000170e0: 6f70 656e 2873 7461 7473 5f70 6174 682c  open(stats_path,
+000170f0: 2022 7222 2c20 656e 636f 6469 6e67 3d22   "r", encoding="
+00017100: 7574 662d 3822 2920 6173 2073 7461 7473  utf-8") as stats
+00017110: 5f66 696c 652c 0a20 2020 2020 2020 2029  _file,.        )
+00017120: 3a0a 2020 2020 2020 2020 2020 2020 736f  :.            so
+00017130: 6e67 735f 6c69 6e65 7320 3d20 736f 6e67  ngs_lines = song
+00017140: 735f 6669 6c65 2e72 6561 646c 696e 6573  s_file.readlines
+00017150: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
+00017160: 7461 7473 203d 2064 6963 7428 0a20 2020  tats = dict(.   
+00017170: 2020 2020 2020 2020 2020 2020 206d 6170               map
+00017180: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00017190: 2020 2020 2020 6c61 6d62 6461 2074 3a20        lambda t: 
+000171a0: 2869 6e74 2874 5b30 5d29 2c29 202b 2074  (int(t[0]),) + t
+000171b0: 5b31 3a5d 2c0a 2020 2020 2020 2020 2020  [1:],.          
+000171c0: 2020 2020 2020 2020 2020 6d61 7028 0a20            map(. 
+000171d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000171e0: 2020 2020 2020 206c 616d 6264 6120 783a         lambda x:
+000171f0: 2074 7570 6c65 286d 6170 2866 6c6f 6174   tuple(map(float
+00017200: 2c20 782e 7374 7269 7028 292e 7370 6c69  , x.strip().spli
+00017210: 7428 227c 2229 2929 2c0a 2020 2020 2020  t("|"))),.      
+00017220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017230: 2020 7374 6174 735f 6669 6c65 2e72 6561    stats_file.rea
+00017240: 646c 696e 6573 2829 2c0a 2020 2020 2020  dlines(),.      
+00017250: 2020 2020 2020 2020 2020 2020 2020 292c                ),
+00017260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017270: 2029 0a20 2020 2020 2020 2020 2020 2029   ).            )
+00017280: 0a0a 2020 2020 2020 2020 2020 2020 7461  ..            ta
+00017290: 6773 203d 2064 6566 6175 6c74 6469 6374  gs = defaultdict
+000172a0: 286c 616d 6264 613a 2028 302e 302c 2030  (lambda: (0.0, 0
+000172b0: 2e30 2929 0a20 2020 2020 2020 2020 2020  .0)).           
+000172c0: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+000172d0: 6c65 6e28 736f 6e67 735f 6c69 6e65 7329  len(songs_lines)
+000172e0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000172f0: 2020 2073 6f6e 675f 6964 2c20 736f 6e67     song_id, song
+00017300: 5f6e 616d 652c 2074 6167 5f73 7472 696e  _name, tag_strin
+00017310: 6720 3d20 280a 2020 2020 2020 2020 2020  g = (.          
+00017320: 2020 2020 2020 2020 2020 736f 6e67 735f            songs_
+00017330: 6c69 6e65 735b 695d 2e73 7472 6970 2829  lines[i].strip()
+00017340: 2e73 706c 6974 2822 7c22 295b 303a 335d  .split("|")[0:3]
+00017350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017360: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+00017370: 2020 2069 6620 6e6f 7420 6f73 2e70 6174     if not os.pat
+00017380: 682e 6578 6973 7473 286f 732e 7061 7468  h.exists(os.path
+00017390: 2e6a 6f69 6e28 534f 4e47 535f 4449 522c  .join(SONGS_DIR,
+000173a0: 2073 6f6e 675f 6e61 6d65 2929 3a0a 2020   song_name)):.  
+000173b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000173c0: 2020 736f 6e67 735f 6e6f 745f 666f 756e    songs_not_foun
+000173d0: 642e 6170 7065 6e64 2828 736f 6e67 5f69  d.append((song_i
+000173e0: 642c 2073 6f6e 675f 6e61 6d65 2929 0a20  d, song_name)). 
+000173f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017400: 2020 2063 6f6e 7469 6e75 650a 2020 2020     continue.    
+00017410: 2020 2020 2020 2020 2020 2020 736f 6e67              song
+00017420: 5f69 6420 3d20 696e 7428 736f 6e67 5f69  _id = int(song_i
+00017430: 6429 0a20 2020 2020 2020 2020 2020 2020  d).             
+00017440: 2020 2069 6620 7461 675f 7374 7269 6e67     if tag_string
+00017450: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00017460: 2020 2020 2020 666f 7220 7461 6720 696e        for tag in
+00017470: 2074 6167 5f73 7472 696e 672e 7370 6c69   tag_string.spli
+00017480: 7428 222c 2229 3a0a 2020 2020 2020 2020  t(","):.        
+00017490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000174a0: 6966 206e 6f74 2073 6561 7263 685f 7461  if not search_ta
+000174b0: 6773 206f 7220 7461 6720 696e 2073 6561  gs or tag in sea
+000174c0: 7263 685f 7461 6773 3a0a 2020 2020 2020  rch_tags:.      
+000174d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000174e0: 2020 2020 2020 7461 6773 5b74 6167 5d20        tags[tag] 
+000174f0: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+00017500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017510: 2020 2020 7461 6773 5b74 6167 5d5b 305d      tags[tag][0]
+00017520: 202b 2073 7461 7473 5b73 6f6e 675f 6964   + stats[song_id
+00017530: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00017540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017550: 2020 2074 6167 735b 7461 675d 5b31 5d0a     tags[tag][1].
+00017560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017580: 2b20 6d75 7369 635f 7461 672e 6c6f 6164  + music_tag.load
+00017590: 5f66 696c 6528 0a20 2020 2020 2020 2020  _file(.         
+000175a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000175b0: 2020 2020 2020 2020 2020 206f 732e 7061             os.pa
+000175c0: 7468 2e6a 6f69 6e28 534f 4e47 535f 4449  th.join(SONGS_DI
+000175d0: 522c 2073 6f6e 675f 6e61 6d65 290a 2020  R, song_name).  
+000175e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000175f0: 2020 2020 2020 2020 2020 2020 2020 295b                )[
+00017600: 2223 6c65 6e67 7468 225d 2e76 616c 7565  "#length"].value
+00017610: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00017620: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00017630: 0a20 2020 2020 2020 2020 2020 2074 6167  .            tag
+00017640: 5f69 7465 6d73 203d 206c 6973 7428 7461  _items = list(ta
+00017650: 6773 2e69 7465 6d73 2829 290a 0a20 2020  gs.items())..   
+00017660: 2020 2020 2020 2020 2069 6620 736f 7274           if sort
+00017670: 5f20 213d 2022 6e6f 6e65 223a 0a20 2020  _ != "none":.   
+00017680: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00017690: 736f 7274 5f20 696e 2028 226e 616d 6522  sort_ in ("name"
+000176a0: 2c20 226e 2229 3a0a 2020 2020 2020 2020  , "n"):.        
+000176b0: 2020 2020 2020 2020 2020 2020 736f 7274              sort
+000176c0: 5f6b 6579 203d 206c 616d 6264 6120 743a  _key = lambda t:
+000176d0: 2074 5b30 5d0a 2020 2020 2020 2020 2020   t[0].          
+000176e0: 2020 2020 2020 656c 6966 2073 6f72 745f        elif sort_
+000176f0: 2069 6e20 2822 7365 6373 2d6c 6973 7465   in ("secs-liste
+00017700: 6e65 6422 2c20 2273 2229 3a0a 2020 2020  ned", "s"):.    
+00017710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017720: 736f 7274 5f6b 6579 203d 206c 616d 6264  sort_key = lambd
+00017730: 6120 743a 2074 5b31 5d5b 305d 0a20 2020  a t: t[1][0].   
+00017740: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
+00017750: 6620 736f 7274 5f20 696e 2028 2264 7572  f sort_ in ("dur
+00017760: 6174 696f 6e22 2c20 2264 2229 3a0a 2020  ation", "d"):.  
+00017770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017780: 2020 736f 7274 5f6b 6579 203d 206c 616d    sort_key = lam
+00017790: 6264 6120 743a 2074 5b31 5d5b 315d 0a20  bda t: t[1][1]. 
+000177a0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+000177b0: 6c69 6620 736f 7274 5f20 696e 2028 2274  lif sort_ in ("t
+000177c0: 696d 6573 2d6c 6973 7465 6e65 6422 2c20  imes-listened", 
+000177d0: 2274 2229 3a0a 2020 2020 2020 2020 2020  "t"):.          
+000177e0: 2020 2020 2020 2020 2020 736f 7274 5f6b            sort_k
+000177f0: 6579 203d 206c 616d 6264 6120 743a 2074  ey = lambda t: t
+00017800: 5b31 5d5b 305d 202f 2074 5b31 5d5b 315d  [1][0] / t[1][1]
+00017810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017820: 2074 6167 5f69 7465 6d73 2e73 6f72 7428   tag_items.sort(
+00017830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017840: 2020 2020 206b 6579 3d73 6f72 745f 6b65       key=sort_ke
+00017850: 792c 0a20 2020 2020 2020 2020 2020 2020  y,.             
+00017860: 2020 2020 2020 2072 6576 6572 7365 3d6e         reverse=n
+00017870: 6f74 2072 6576 6572 7365 5f2c 0a20 2020  ot reverse_,.   
+00017880: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+00017890: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+000178a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000178b0: 2069 6620 6e6f 7420 7265 7665 7273 655f   if not reverse_
+000178c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000178d0: 2020 2020 2020 7461 675f 6974 656d 732e        tag_items.
+000178e0: 7265 7665 7273 6528 290a 0a20 2020 2020  reverse()..     
+000178f0: 2020 2020 2020 2066 6f72 2074 6167 2c20         for tag, 
+00017900: 286c 6973 7465 6e5f 7469 6d65 2c20 746f  (listen_time, to
+00017910: 7461 6c5f 6475 7261 7469 6f6e 2920 696e  tal_duration) in
+00017920: 2074 6167 5f69 7465 6d73 3a0a 2020 2020   tag_items:.    
+00017930: 2020 2020 2020 2020 2020 2020 636c 6963              clic
+00017940: 6b2e 6563 686f 280a 2020 2020 2020 2020  k.echo(.        
+00017950: 2020 2020 2020 2020 2020 2020 6622 7b74              f"{t
+00017960: 6167 7d20 7b63 6c69 636b 2e73 7479 6c65  ag} {click.style
+00017970: 2866 6f72 6d61 745f 7365 636f 6e64 7328  (format_seconds(
+00017980: 746f 7461 6c5f 6475 7261 7469 6f6e 2c20  total_duration, 
+00017990: 7368 6f77 5f64 6563 696d 616c 3d54 7275  show_decimal=Tru
+000179a0: 6529 2c20 6667 3d27 6272 6967 6874 5f62  e), fg='bright_b
+000179b0: 6c61 636b 2729 7d20 7b63 6c69 636b 2e73  lack')} {click.s
+000179c0: 7479 6c65 2866 6f72 6d61 745f 7365 636f  tyle(format_seco
+000179d0: 6e64 7328 6c69 7374 656e 5f74 696d 652c  nds(listen_time,
+000179e0: 2073 686f 775f 6465 6369 6d61 6c3d 5472   show_decimal=Tr
+000179f0: 7565 292c 2066 673d 2779 656c 6c6f 7727  ue), fg='yellow'
+00017a00: 297d 207b 636c 6963 6b2e 7374 796c 6528  )} {click.style(
+00017a10: 2725 2e32 6627 2528 6c69 7374 656e 5f74  '%.2f'%(listen_t
+00017a20: 696d 652f 746f 7461 6c5f 6475 7261 7469  ime/total_durati
+00017a30: 6f6e 292c 2066 673d 2767 7265 656e 2729  on), fg='green')
+00017a40: 7d22 0a20 2020 2020 2020 2020 2020 2020  }".             
+00017a50: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00017a60: 2020 2020 206e 756d 5f6c 696e 6573 202b       num_lines +
+00017a70: 3d20 310a 2020 2020 2020 2020 2020 2020  = 1.            
+00017a80: 2020 2020 6966 2074 6f70 2069 7320 6e6f      if top is no
+00017a90: 7420 4e6f 6e65 2061 6e64 206e 756d 5f6c  t None and num_l
+00017aa0: 696e 6573 203d 3d20 746f 703a 0a20 2020  ines == top:.   
+00017ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017ac0: 2062 7265 616b 0a20 2020 2020 2020 2020   break.         
+00017ad0: 2020 2069 6620 736f 6e67 735f 6e6f 745f     if songs_not_
+00017ae0: 666f 756e 643a 0a20 2020 2020 2020 2020  found:.         
+00017af0: 2020 2020 2020 2063 6c69 636b 2e73 6563         click.sec
+00017b00: 686f 2822 536f 6e67 2066 696c 6573 206e  ho("Song files n
+00017b10: 6f74 2066 6f75 6e64 3a22 2c20 6667 3d22  ot found:", fg="
+00017b20: 7265 6422 290a 2020 2020 2020 2020 2020  red").          
+00017b30: 2020 2020 2020 666f 7220 736f 6e67 5f69        for song_i
+00017b40: 642c 2073 6f6e 675f 6e61 6d65 2069 6e20  d, song_name in 
+00017b50: 736f 6e67 735f 6e6f 745f 666f 756e 643a  songs_not_found:
+00017b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017b70: 2020 2020 2063 6c69 636b 2e73 6563 686f       click.secho
+00017b80: 2866 225c 747b 736f 6e67 5f6e 616d 657d  (f"\t{song_name}
+00017b90: 2028 4944 207b 736f 6e67 5f69 647d 2922   (ID {song_id})"
+00017ba0: 2c20 6667 3d22 7265 6422 290a 2020 2020  , fg="red").    
+00017bb0: 2020 2020 7265 7475 726e 0a0a 2020 2020      return..    
+00017bc0: 6e6f 5f72 6573 756c 7473 203d 2054 7275  no_results = Tru
+00017bd0: 650a 2020 2020 7769 7468 2028 0a20 2020  e.    with (.   
+00017be0: 2020 2020 206f 7065 6e28 534f 4e47 535f       open(SONGS_
+00017bf0: 494e 464f 5f50 4154 482c 2022 7222 2c20  INFO_PATH, "r", 
+00017c00: 656e 636f 6469 6e67 3d22 7574 662d 3822  encoding="utf-8"
+00017c10: 2920 6173 2073 6f6e 6773 5f66 696c 652c  ) as songs_file,
+00017c20: 0a20 2020 2020 2020 206f 7065 6e28 7374  .        open(st
+00017c30: 6174 735f 7061 7468 2c20 2272 222c 2065  ats_path, "r", e
+00017c40: 6e63 6f64 696e 673d 2275 7466 2d38 2229  ncoding="utf-8")
+00017c50: 2061 7320 7374 6174 735f 6669 6c65 2c0a   as stats_file,.
+00017c60: 2020 2020 293a 0a0a 2020 2020 2020 2020      ):..        
+00017c70: 6465 6620 6368 6563 6b5f 6966 5f66 696c  def check_if_fil
+00017c80: 655f 6578 6973 7473 2864 6574 6169 6c5f  e_exists(detail_
+00017c90: 7374 7269 6e67 293a 0a20 2020 2020 2020  string):.       
+00017ca0: 2020 2020 2064 6574 6169 6c73 203d 2064       details = d
+00017cb0: 6574 6169 6c5f 7374 7269 6e67 2e73 7472  etail_string.str
+00017cc0: 6970 2829 2e73 706c 6974 2822 7c22 290a  ip().split("|").
+00017cd0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+00017ce0: 6f74 206f 732e 7061 7468 2e65 7869 7374  ot os.path.exist
+00017cf0: 7328 6f73 2e70 6174 682e 6a6f 696e 2853  s(os.path.join(S
+00017d00: 4f4e 4753 5f44 4952 2c20 6465 7461 696c  ONGS_DIR, detail
+00017d10: 735b 315d 2929 3a0a 2020 2020 2020 2020  s[1])):.        
+00017d20: 2020 2020 2020 2020 736f 6e67 735f 6e6f          songs_no
+00017d30: 745f 666f 756e 642e 6170 7065 6e64 2864  t_found.append(d
+00017d40: 6574 6169 6c73 290a 2020 2020 2020 2020  etails).        
+00017d50: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+00017d60: 616c 7365 0a20 2020 2020 2020 2020 2020  alse.           
+00017d70: 2072 6574 7572 6e20 5472 7565 0a0a 2020   return True..  
+00017d80: 2020 2020 2020 6c69 6e65 7320 3d20 6c69        lines = li
+00017d90: 7374 2866 696c 7465 7228 6368 6563 6b5f  st(filter(check_
+00017da0: 6966 5f66 696c 655f 6578 6973 7473 2c20  if_file_exists, 
+00017db0: 736f 6e67 735f 6669 6c65 2e72 6561 646c  songs_file.readl
+00017dc0: 696e 6573 2829 2929 0a0a 2020 2020 2020  ines()))..      
+00017dd0: 2020 7374 6174 7320 3d20 6469 6374 280a    stats = dict(.
+00017de0: 2020 2020 2020 2020 2020 2020 6d61 7028              map(
+00017df0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017e00: 206c 616d 6264 6120 743a 2028 696e 7428   lambda t: (int(
+00017e10: 745b 305d 292c 2920 2b20 745b 313a 5d2c  t[0]),) + t[1:],
+00017e20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017e30: 206d 6170 280a 2020 2020 2020 2020 2020   map(.          
+00017e40: 2020 2020 2020 2020 2020 6c61 6d62 6461            lambda
+00017e50: 2078 3a20 7475 706c 6528 6d61 7028 666c   x: tuple(map(fl
+00017e60: 6f61 742c 2078 2e73 7472 6970 2829 2e73  oat, x.strip().s
+00017e70: 706c 6974 2822 7c22 2929 292c 0a20 2020  plit("|"))),.   
+00017e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017e90: 2073 7461 7473 5f66 696c 652e 7265 6164   stats_file.read
+00017ea0: 6c69 6e65 7328 292c 0a20 2020 2020 2020  lines(),.       
+00017eb0: 2020 2020 2020 2020 2029 2c0a 2020 2020           ),.    
+00017ec0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00017ed0: 2020 290a 0a20 2020 2020 2020 2066 6f72    )..        for
+00017ee0: 2069 2069 6e20 7261 6e67 6528 6c65 6e28   i in range(len(
+00017ef0: 6c69 6e65 7329 293a 0a20 2020 2020 2020  lines)):.       
+00017f00: 2020 2020 2064 6574 6169 6c73 203d 206c       details = l
+00017f10: 696e 6573 5b69 5d2e 7374 7269 7028 292e  ines[i].strip().
+00017f20: 7370 6c69 7428 227c 2229 0a20 2020 2020  split("|").     
+00017f30: 2020 2020 2020 2073 6f6e 675f 6964 203d         song_id =
+00017f40: 2069 6e74 2864 6574 6169 6c73 5b30 5d29   int(details[0])
+00017f50: 0a0a 2020 2020 2020 2020 2020 2020 7461  ..            ta
+00017f60: 6773 203d 2073 6574 2864 6574 6169 6c73  gs = set(details
+00017f70: 5b32 5d2e 7370 6c69 7428 222c 2229 290a  [2].split(",")).
+00017f80: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00017f90: 6561 7263 685f 7461 6773 3a0a 2020 2020  earch_tags:.    
+00017fa0: 2020 2020 2020 2020 2020 2020 6966 206d              if m
+00017fb0: 6174 6368 5f61 6c6c 3a0a 2020 2020 2020  atch_all:.      
+00017fc0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00017fd0: 206e 6f74 2073 6561 7263 685f 7461 6773   not search_tags
+00017fe0: 203c 3d20 7461 6773 3a20 2023 2073 7562   <= tags:  # sub
+00017ff0: 7365 740a 2020 2020 2020 2020 2020 2020  set.            
+00018000: 2020 2020 2020 2020 2020 2020 6c69 6e65              line
+00018010: 735b 695d 203d 2022 220a 2020 2020 2020  s[i] = "".      
+00018020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018030: 2020 636f 6e74 696e 7565 0a20 2020 2020    continue.     
+00018040: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00018050: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018060: 2020 2020 2069 6620 6e6f 7420 7365 6172       if not sear
+00018070: 6368 5f74 6167 7320 2620 7461 6773 3a20  ch_tags & tags: 
+00018080: 2023 2069 6e74 6572 7365 6374 696f 6e0a   # intersection.
+00018090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000180a0: 2020 2020 2020 2020 6c69 6e65 735b 695d          lines[i]
+000180b0: 203d 2022 220a 2020 2020 2020 2020 2020   = "".          
+000180c0: 2020 2020 2020 2020 2020 2020 2020 636f                co
+000180d0: 6e74 696e 7565 0a0a 2020 2020 2020 2020  ntinue..        
+000180e0: 2020 2020 7469 6d65 5f6c 6973 7465 6e65      time_listene
+000180f0: 6420 3d20 7374 6174 735b 736f 6e67 5f69  d = stats[song_i
+00018100: 645d 0a20 2020 2020 2020 2020 2020 206c  d].            l
+00018110: 696e 6573 5b69 5d20 3d20 7475 706c 6528  ines[i] = tuple(
+00018120: 6465 7461 696c 7329 202b 2028 0a20 2020  details) + (.   
+00018130: 2020 2020 2020 2020 2020 2020 2074 696d               tim
+00018140: 655f 6c69 7374 656e 6564 2c0a 2020 2020  e_listened,.    
+00018150: 2020 2020 2020 2020 2020 2020 6d75 7369              musi
+00018160: 635f 7461 672e 6c6f 6164 5f66 696c 6528  c_tag.load_file(
+00018170: 6f73 2e70 6174 682e 6a6f 696e 2853 4f4e  os.path.join(SON
+00018180: 4753 5f44 4952 2c20 6465 7461 696c 735b  GS_DIR, details[
+00018190: 315d 2929 5b0a 2020 2020 2020 2020 2020  1]))[.          
+000181a0: 2020 2020 2020 2020 2020 2223 6c65 6e67            "#leng
+000181b0: 7468 220a 2020 2020 2020 2020 2020 2020  th".            
+000181c0: 2020 2020 5d2e 7661 6c75 652c 0a20 2020      ].value,.   
+000181d0: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+000181e0: 2020 2020 6c69 6e65 7320 3d20 5b6c 696e      lines = [lin
+000181f0: 6520 666f 7220 6c69 6e65 2069 6e20 6c69  e for line in li
+00018200: 6e65 7320 6966 206c 696e 655d 0a0a 2020  nes if line]..  
+00018210: 2020 2020 2020 6966 2073 6f72 745f 2021        if sort_ !
+00018220: 3d20 226e 6f6e 6522 3a0a 2020 2020 2020  = "none":.      
+00018230: 2020 2020 2020 6966 2073 6f72 745f 2069        if sort_ i
+00018240: 6e20 2822 6e61 6d65 222c 2022 6e22 293a  n ("name", "n"):
+00018250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018260: 2073 6f72 745f 6b65 7920 3d20 6c61 6d62   sort_key = lamb
+00018270: 6461 2074 3a20 745b 315d 0a20 2020 2020  da t: t[1].     
+00018280: 2020 2020 2020 2065 6c69 6620 736f 7274         elif sort
+00018290: 5f20 696e 2028 2273 6563 732d 6c69 7374  _ in ("secs-list
+000182a0: 656e 6564 222c 2022 7322 293a 0a20 2020  ened", "s"):.   
+000182b0: 2020 2020 2020 2020 2020 2020 2073 6f72               sor
+000182c0: 745f 6b65 7920 3d20 6c61 6d62 6461 2074  t_key = lambda t
+000182d0: 3a20 666c 6f61 7428 745b 2d32 5d29 0a20  : float(t[-2]). 
+000182e0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+000182f0: 736f 7274 5f20 696e 2028 2264 7572 6174  sort_ in ("durat
+00018300: 696f 6e22 2c20 2264 2229 3a0a 2020 2020  ion", "d"):.    
+00018310: 2020 2020 2020 2020 2020 2020 736f 7274              sort
+00018320: 5f6b 6579 203d 206c 616d 6264 6120 743a  _key = lambda t:
+00018330: 2066 6c6f 6174 2874 5b2d 315d 290a 2020   float(t[-1]).  
+00018340: 2020 2020 2020 2020 2020 656c 6966 2073            elif s
+00018350: 6f72 745f 2069 6e20 2822 7469 6d65 732d  ort_ in ("times-
+00018360: 6c69 7374 656e 6564 222c 2022 7422 293a  listened", "t"):
+00018370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018380: 2073 6f72 745f 6b65 7920 3d20 6c61 6d62   sort_key = lamb
+00018390: 6461 2074 3a20 666c 6f61 7428 745b 2d32  da t: float(t[-2
+000183a0: 5d29 202f 2066 6c6f 6174 2874 5b2d 315d  ]) / float(t[-1]
+000183b0: 290a 2020 2020 2020 2020 2020 2020 6c69  ).            li
+000183c0: 6e65 732e 736f 7274 280a 2020 2020 2020  nes.sort(.      
+000183d0: 2020 2020 2020 2020 2020 6b65 793d 736f            key=so
+000183e0: 7274 5f6b 6579 2c0a 2020 2020 2020 2020  rt_key,.        
+000183f0: 2020 2020 2020 2020 7265 7665 7273 653d          reverse=
+00018400: 6e6f 7420 7265 7665 7273 655f 2c0a 2020  not reverse_,.  
+00018410: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00018420: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00018430: 2020 2020 2020 6966 206e 6f74 2072 6576        if not rev
+00018440: 6572 7365 5f3a 0a20 2020 2020 2020 2020  erse_:.         
+00018450: 2020 2020 2020 206c 696e 6573 2e72 6576         lines.rev
+00018460: 6572 7365 2829 0a0a 2020 2020 2020 2020  erse()..        
+00018470: 666f 7220 6465 7461 696c 7320 696e 206c  for details in l
+00018480: 696e 6573 3a0a 2020 2020 2020 2020 2020  ines:.          
+00018490: 2020 7072 696e 745f 656e 7472 7928 6465    print_entry(de
+000184a0: 7461 696c 7329 0a20 2020 2020 2020 2020  tails).         
+000184b0: 2020 206e 756d 5f6c 696e 6573 202b 3d20     num_lines += 
+000184c0: 310a 2020 2020 2020 2020 2020 2020 6e6f  1.            no
+000184d0: 5f72 6573 756c 7473 203d 2046 616c 7365  _results = False
+000184e0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000184f0: 746f 7020 6973 206e 6f74 204e 6f6e 6520  top is not None 
+00018500: 616e 6420 6e75 6d5f 6c69 6e65 7320 3d3d  and num_lines ==
+00018510: 2074 6f70 3a0a 2020 2020 2020 2020 2020   top:.          
+00018520: 2020 2020 2020 6272 6561 6b0a 0a20 2020        break..   
+00018530: 2069 6620 6e6f 5f72 6573 756c 7473 2061   if no_results a
+00018540: 6e64 2073 6561 7263 685f 7461 6773 3a0a  nd search_tags:.
+00018550: 2020 2020 2020 2020 636c 6963 6b2e 7365          click.se
+00018560: 6368 6f28 224e 6f20 736f 6e67 7320 666f  cho("No songs fo
+00018570: 756e 6420 6d61 7463 6869 6e67 2074 6167  und matching tag
+00018580: 732e 222c 2066 673d 2272 6564 2229 0a20  s.", fg="red"). 
+00018590: 2020 2065 6c69 6620 6e6f 5f72 6573 756c     elif no_resul
+000185a0: 7473 3a0a 2020 2020 2020 2020 636c 6963  ts:.        clic
+000185b0: 6b2e 7365 6368 6f28 0a20 2020 2020 2020  k.secho(.       
+000185c0: 2020 2020 2022 4e6f 2073 6f6e 6773 2066       "No songs f
+000185d0: 6f75 6e64 2e20 5573 6520 276d 6165 7374  ound. Use 'maest
+000185e0: 726f 2061 6464 2720 746f 2061 6464 2061  ro add' to add a
+000185f0: 2073 6f6e 672e 222c 2066 673d 2272 6564   song.", fg="red
+00018600: 220a 2020 2020 2020 2020 290a 2020 2020  ".        ).    
+00018610: 656c 6966 2073 6f6e 6773 5f6e 6f74 5f66  elif songs_not_f
+00018620: 6f75 6e64 3a0a 2020 2020 2020 2020 636c  ound:.        cl
+00018630: 6963 6b2e 7365 6368 6f28 2253 6f6e 6720  ick.secho("Song 
+00018640: 6669 6c65 7320 6e6f 7420 666f 756e 643a  files not found:
+00018650: 222c 2066 673d 2272 6564 2229 0a20 2020  ", fg="red").   
+00018660: 2020 2020 2066 6f72 2064 6574 6169 6c73       for details
+00018670: 2069 6e20 736f 6e67 735f 6e6f 745f 666f   in songs_not_fo
+00018680: 756e 643a 0a20 2020 2020 2020 2020 2020  und:.           
+00018690: 2063 6c69 636b 2e73 6563 686f 2866 225c   click.secho(f"\
+000186a0: 747b 6465 7461 696c 735b 315d 7d20 2849  t{details[1]} (I
+000186b0: 4420 7b64 6574 6169 6c73 5b30 5d7d 2922  D {details[0]})"
+000186c0: 2c20 6667 3d22 7265 6422 290a 0a0a 4063  , fg="red")...@c
+000186d0: 6c69 2e63 6f6d 6d61 6e64 2829 0a40 636c  li.command().@cl
+000186e0: 6963 6b2e 6f70 7469 6f6e 280a 2020 2020  ick.option(.    
+000186f0: 222d 7922 2c0a 2020 2020 222d 2d79 6561  "-y",.    "--yea
+00018700: 7222 2c0a 2020 2020 2279 6561 7222 2c0a  r",.    "year",.
+00018710: 2020 2020 6865 6c70 3d22 5368 6f77 2074      help="Show t
+00018720: 696d 6520 6c69 7374 656e 6564 2066 6f72  ime listened for
+00018730: 2061 2073 7065 6369 6669 6320 7965 6172   a specific year
+00018740: 2c20 696e 7374 6561 6420 6f66 2074 6865  , instead of the
+00018750: 2074 6f74 616c 2e20 5061 7373 696e 6720   total. Passing 
+00018760: 2763 7572 2720 7769 6c6c 2073 686f 7720  'cur' will show 
+00018770: 7468 6520 7469 6d65 206c 6973 7465 6e65  the time listene
+00018780: 6420 666f 7220 7468 6520 6375 7272 656e  d for the curren
+00018790: 7420 7965 6172 2e22 2c0a 290a 4063 6c69  t year.",.).@cli
+000187a0: 636b 2e6f 7074 696f 6e28 0a20 2020 2022  ck.option(.    "
+000187b0: 2d49 2f2d 6e49 222c 0a20 2020 2022 2d2d  -I/-nI",.    "--
+000187c0: 736f 6e67 2d69 6e66 6f2f 2d2d 6e6f 2d73  song-info/--no-s
+000187d0: 6f6e 672d 696e 666f 222c 0a20 2020 2022  ong-info",.    "
+000187e0: 736f 6e67 5f69 6e66 6f22 2c0a 2020 2020  song_info",.    
+000187f0: 6465 6661 756c 743d 4661 6c73 652c 0a20  default=False,. 
+00018800: 2020 2068 656c 703d 2253 686f 7720 7468     help="Show th
+00018810: 6520 6172 7469 7374 2c20 616c 6275 6d2c  e artist, album,
+00018820: 2061 6e64 2061 6c62 756d 2061 7274 6973   and album artis
+00018830: 7420 666f 7220 6561 6368 2073 6f6e 672e  t for each song.
+00018840: 222c 0a29 0a40 636c 6963 6b2e 6172 6775  ",.).@click.argu
+00018850: 6d65 6e74 2822 736f 6e67 5f69 6473 222c  ment("song_ids",
+00018860: 2074 7970 653d 636c 6963 6b2e 494e 542c   type=click.INT,
+00018870: 206e 6172 6773 3d2d 312c 2072 6571 7569   nargs=-1, requi
+00018880: 7265 643d 5472 7565 290a 6465 6620 656e  red=True).def en
+00018890: 7472 7928 736f 6e67 5f69 6473 2c20 7965  try(song_ids, ye
+000188a0: 6172 2c20 736f 6e67 5f69 6e66 6f29 3a0a  ar, song_info):.
+000188b0: 2020 2020 2222 220a 2020 2020 5669 6577      """.    View
+000188c0: 2074 6865 2064 6574 6169 6c73 2066 6f72   the details for
+000188d0: 2073 7065 6369 6669 6320 736f 6e67 2873   specific song(s
+000188e0: 292e 0a0a 2020 2020 5072 696e 7473 2074  )...    Prints t
+000188f0: 6865 2064 6574 6169 6c73 206f 6620 7468  he details of th
+00018900: 6520 736f 6e67 2873 2920 7769 7468 2074  e song(s) with t
+00018910: 6865 2049 4428 7329 2053 4f4e 475f 4944  he ID(s) SONG_ID
+00018920: 532e 0a0a 2020 2020 5c62 0a20 2020 204f  S...    \b.    O
+00018930: 7574 7075 7420 666f 726d 6174 3a0a 2020  utput format:.  
+00018940: 2020 2020 2020 4944 2c20 6e61 6d65 2c20        ID, name, 
+00018950: 6475 7261 7469 6f6e 2c20 6c69 7374 656e  duration, listen
+00018960: 2074 696d 652c 2074 696d 6573 206c 6973   time, times lis
+00018970: 7465 6e65 642c 205b 636c 6970 2d73 7461  tened, [clip-sta
+00018980: 7274 2c20 636c 6970 2d65 6e64 5d20 6966  rt, clip-end] if
+00018990: 2063 6c69 7020 6578 6973 7473 2c20 636f   clip exists, co
+000189a0: 6d6d 612d 7365 7061 7261 7465 6420 7461  mma-separated ta
+000189b0: 6773 2069 6620 616e 790a 2020 2020 2020  gs if any.      
+000189c0: 2020 6172 7469 7374 202d 2061 6c62 756d    artist - album
+000189d0: 2028 616c 6275 6d20 6172 7469 7374 2920   (album artist) 
+000189e0: 6966 202d 492f 2d2d 736f 6e67 2d69 6e66  if -I/--song-inf
+000189f0: 6f20 6973 2070 6173 7365 640a 2020 2020  o is passed.    
+00018a00: 2222 220a 2020 2020 736f 6e67 5f69 6473  """.    song_ids
+00018a10: 203d 2073 6574 2873 6f6e 675f 6964 7329   = set(song_ids)
+00018a20: 0a0a 2020 2020 6966 2079 6561 7220 6973  ..    if year is
+00018a30: 204e 6f6e 653a 0a20 2020 2020 2020 2073   None:.        s
+00018a40: 7461 7473 5f70 6174 6820 3d20 544f 5441  tats_path = TOTA
+00018a50: 4c5f 5354 4154 535f 5041 5448 0a20 2020  L_STATS_PATH.   
+00018a60: 2065 6c73 653a 0a20 2020 2020 2020 2069   else:.        i
+00018a70: 6620 7965 6172 203d 3d20 2263 7572 223a  f year == "cur":
+00018a80: 0a20 2020 2020 2020 2020 2020 2079 6561  .            yea
+00018a90: 7220 3d20 4355 525f 5945 4152 0a20 2020  r = CUR_YEAR.   
+00018aa0: 2020 2020 2020 2020 2073 7461 7473 5f70           stats_p
+00018ab0: 6174 6820 3d20 4355 525f 5945 4152 5f53  ath = CUR_YEAR_S
+00018ac0: 5441 5453 5f50 4154 480a 2020 2020 2020  TATS_PATH.      
+00018ad0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00018ae0: 2020 2020 6966 206e 6f74 2079 6561 722e      if not year.
+00018af0: 6973 6469 6769 7428 293a 0a20 2020 2020  isdigit():.     
+00018b00: 2020 2020 2020 2020 2020 2063 6c69 636b             click
+00018b10: 2e73 6563 686f 2822 5965 6172 206d 7573  .secho("Year mus
+00018b20: 7420 6265 2061 206e 756d 6265 722e 222c  t be a number.",
+00018b30: 2066 673d 2272 6564 2229 0a20 2020 2020   fg="red").     
+00018b40: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00018b50: 6e0a 2020 2020 2020 2020 2020 2020 7374  n.            st
+00018b60: 6174 735f 7061 7468 203d 206f 732e 7061  ats_path = os.pa
+00018b70: 7468 2e6a 6f69 6e28 5354 4154 535f 4449  th.join(STATS_DI
+00018b80: 522c 2066 227b 7965 6172 7d2e 7478 7422  R, f"{year}.txt"
+00018b90: 290a 0a20 2020 2074 7279 3a0a 2020 2020  )..    try:.    
+00018ba0: 2020 2020 7769 7468 2028 0a20 2020 2020      with (.     
+00018bb0: 2020 2020 2020 206f 7065 6e28 534f 4e47         open(SONG
+00018bc0: 535f 494e 464f 5f50 4154 482c 2022 7222  S_INFO_PATH, "r"
+00018bd0: 2c20 656e 636f 6469 6e67 3d22 7574 662d  , encoding="utf-
+00018be0: 3822 2920 6173 2073 6f6e 6773 5f66 696c  8") as songs_fil
+00018bf0: 652c 0a20 2020 2020 2020 2020 2020 206f  e,.            o
+00018c00: 7065 6e28 7374 6174 735f 7061 7468 2c20  pen(stats_path, 
+00018c10: 2272 222c 2065 6e63 6f64 696e 673d 2275  "r", encoding="u
+00018c20: 7466 2d38 2229 2061 7320 7374 6174 735f  tf-8") as stats_
+00018c30: 6669 6c65 2c0a 2020 2020 2020 2020 293a  file,.        ):
+00018c40: 0a20 2020 2020 2020 2020 2020 206c 696e  .            lin
+00018c50: 6573 203d 2073 6f6e 6773 5f66 696c 652e  es = songs_file.
+00018c60: 7265 6164 6c69 6e65 7328 290a 2020 2020  readlines().    
+00018c70: 2020 2020 2020 2020 7374 6174 7320 3d20          stats = 
+00018c80: 6469 6374 280a 2020 2020 2020 2020 2020  dict(.          
+00018c90: 2020 2020 2020 6d61 7028 0a20 2020 2020        map(.     
+00018ca0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00018cb0: 616d 6264 6120 743a 2028 696e 7428 745b  ambda t: (int(t[
+00018cc0: 305d 292c 2920 2b20 745b 313a 5d2c 2020  0]),) + t[1:],  
+00018cd0: 2320 636f 6e76 6572 7420 6b65 7920 746f  # convert key to
+00018ce0: 2069 6e74 0a20 2020 2020 2020 2020 2020   int.           
+00018cf0: 2020 2020 2020 2020 206d 6170 280a 2020           map(.  
+00018d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018d10: 2020 2020 2020 6c61 6d62 6461 2078 3a20        lambda x: 
+00018d20: 7475 706c 6528 6d61 7028 666c 6f61 742c  tuple(map(float,
+00018d30: 2078 2e73 7472 6970 2829 2e73 706c 6974   x.strip().split
+00018d40: 2822 7c22 2929 292c 0a20 2020 2020 2020  ("|"))),.       
 00018d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018d60: 2020 2072 6573 756c 7473 203d 2079 746d     results = ytm
-00018d70: 7573 6963 2e73 6561 7263 6828 0a20 2020  usic.search(.   
-00018d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018d90: 2020 2020 206f 732e 7061 7468 2e73 706c       os.path.spl
-00018da0: 6974 6578 7428 6465 7461 696c 735b 315d  itext(details[1]
-00018db0: 295b 305d 2c20 6669 6c74 6572 3d22 736f  )[0], filter="so
-00018dc0: 6e67 7322 0a20 2020 2020 2020 2020 2020  ngs".           
-00018dd0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00018de0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-00018df0: 7265 616b 0a20 2020 2020 2020 2020 2020  reak.           
-00018e00: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00018e10: 2020 2020 2020 2063 6c69 636b 2e73 6563         click.sec
-00018e20: 686f 2866 224e 6f20 736f 6e67 2066 6f75  ho(f"No song fou
-00018e30: 6e64 2077 6974 6820 4944 207b 736f 6e67  nd with ID {song
-00018e40: 7d2e 222c 2066 673d 2272 6564 2229 0a20  }.", fg="red"). 
-00018e50: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00018e60: 6574 7572 6e0a 0a20 2020 2079 745f 6d75  eturn..    yt_mu
-00018e70: 7369 635f 706c 6179 6c69 7374 203d 2079  sic_playlist = y
-00018e80: 746d 7573 6963 2e67 6574 5f77 6174 6368  tmusic.get_watch
-00018e90: 5f70 6c61 796c 6973 7428 7265 7375 6c74  _playlist(result
-00018ea0: 735b 305d 5b22 7669 6465 6f49 6422 5d29  s[0]["videoId"])
-00018eb0: 0a0a 2020 2020 636c 6963 6b2e 6563 686f  ..    click.echo
-00018ec0: 2822 5265 636f 6d6d 656e 6461 7469 6f6e  ("Recommendation
-00018ed0: 7320 666f 7220 222c 206e 6c3d 4661 6c73  s for ", nl=Fals
-00018ee0: 6529 0a20 2020 2063 6c69 636b 2e73 6563  e).    click.sec
-00018ef0: 686f 280a 2020 2020 2020 2020 7974 5f6d  ho(.        yt_m
-00018f00: 7573 6963 5f70 6c61 796c 6973 745b 2274  usic_playlist["t
-00018f10: 7261 636b 7322 5d5b 305d 5b22 7469 746c  racks"][0]["titl
-00018f20: 6522 5d20 2b20 2220 222c 0a20 2020 2020  e"] + " ",.     
-00018f30: 2020 2066 673d 2262 6c75 6522 2c0a 2020     fg="blue",.  
-00018f40: 2020 2020 2020 6e6c 3d46 616c 7365 2c0a        nl=False,.
-00018f50: 2020 2020 290a 2020 2020 636c 6963 6b2e      ).    click.
-00018f60: 7365 6368 6f28 0a20 2020 2020 2020 2066  secho(.        f
-00018f70: 2228 6874 7470 733a 2f2f 6d75 7369 632e  "(https://music.
-00018f80: 796f 7574 7562 652e 636f 6d2f 7761 7463  youtube.com/watc
-00018f90: 683f 763d 7b79 745f 6d75 7369 635f 706c  h?v={yt_music_pl
-00018fa0: 6179 6c69 7374 5b27 7472 6163 6b73 275d  aylist['tracks']
-00018fb0: 5b30 5d5b 2776 6964 656f 4964 275d 7d29  [0]['videoId']})
-00018fc0: 222c 0a20 2020 2020 2020 2066 673d 2262  ",.        fg="b
-00018fd0: 7269 6768 745f 626c 6163 6b22 2c0a 2020  right_black",.  
-00018fe0: 2020 2020 2020 6e6c 3d46 616c 7365 2c0a        nl=False,.
-00018ff0: 2020 2020 290a 2020 2020 636c 6963 6b2e      ).    click.
-00019000: 6563 686f 2822 3a22 290a 2020 2020 666f  echo(":").    fo
-00019010: 7220 7472 6163 6b20 696e 2079 745f 6d75  r track in yt_mu
-00019020: 7369 635f 706c 6179 6c69 7374 5b22 7472  sic_playlist["tr
-00019030: 6163 6b73 225d 5b31 3a5d 3a0a 2020 2020  acks"][1:]:.    
-00019040: 2020 2020 636c 6963 6b2e 7365 6368 6f28      click.secho(
-00019050: 7472 6163 6b5b 2274 6974 6c65 225d 202b  track["title"] +
-00019060: 2022 2022 2c20 6667 3d22 626c 7565 222c   " ", fg="blue",
-00019070: 2062 6f6c 643d 5472 7565 2c20 6e6c 3d46   bold=True, nl=F
-00019080: 616c 7365 290a 2020 2020 2020 2020 636c  alse).        cl
-00019090: 6963 6b2e 7365 6368 6f28 0a20 2020 2020  ick.secho(.     
-000190a0: 2020 2020 2020 2066 2268 7474 7073 3a2f         f"https:/
-000190b0: 2f6d 7573 6963 2e79 6f75 7475 6265 2e63  /music.youtube.c
-000190c0: 6f6d 2f77 6174 6368 3f76 3d7b 7472 6163  om/watch?v={trac
-000190d0: 6b5b 2776 6964 656f 4964 275d 7d22 2c0a  k['videoId']}",.
-000190e0: 2020 2020 2020 2020 2020 2020 6667 3d22              fg="
-000190f0: 6272 6967 6874 5f62 6c61 636b 222c 0a20  bright_black",. 
-00019100: 2020 2020 2020 2029 0a0a 0a40 636c 692e         )...@cli.
-00019110: 636f 6d6d 616e 6428 290a 4063 6c69 636b  command().@click
-00019120: 2e61 7267 756d 656e 7428 2273 6f6e 675f  .argument("song_
-00019130: 6964 7322 2c20 7265 7175 6972 6564 3d54  ids", required=T
-00019140: 7275 652c 2074 7970 653d 696e 742c 206e  rue, type=int, n
-00019150: 6172 6773 3d2d 3129 0a40 636c 6963 6b2e  args=-1).@click.
-00019160: 6f70 7469 6f6e 2822 2d42 2f2d 6e42 222c  option("-B/-nB",
-00019170: 2022 2d2d 626f 7474 6f6d 2f2d 2d6e 6f2d   "--bottom/--no-
-00019180: 626f 7474 6f6d 222c 2022 626f 7474 6f6d  bottom", "bottom
-00019190: 222c 2064 6566 6175 6c74 3d46 616c 7365  ", default=False
-000191a0: 290a 6465 6620 7075 7368 2873 6f6e 675f  ).def push(song_
-000191b0: 6964 732c 2062 6f74 746f 6d29 3a0a 2020  ids, bottom):.  
-000191c0: 2020 2222 220a 2020 2020 4d6f 7665 2073    """.    Move s
-000191d0: 6f6e 6773 2061 726f 756e 6420 746f 2074  ongs around to t
-000191e0: 6865 2062 6f74 746f 6d20 6f72 2074 6f70  he bottom or top
-000191f0: 206f 6620 7468 6520 6461 7461 6261 7365   of the database
-00019200: 2e0a 0a20 2020 2050 7573 6820 7468 6520  ...    Push the 
-00019210: 736f 6e67 2873 2920 7769 7468 2049 4428  song(s) with ID(
-00019220: 7329 2053 4f4e 475f 4944 5320 746f 2074  s) SONG_IDS to t
-00019230: 6865 2074 6f70 206f 6620 7468 6520 6461  he top of the da
-00019240: 7461 6261 7365 2028 6173 2069 6620 7468  tabase (as if th
-00019250: 6579 0a20 2020 2077 6572 6520 7468 6520  ey.    were the 
-00019260: 736f 6e67 7320 6d6f 7374 2072 6563 656e  songs most recen
-00019270: 746c 7920 6164 6465 6429 2069 6e20 7468  tly added) in th
-00019280: 6520 6f72 6465 7220 7468 6579 2061 7265  e order they are
-00019290: 2070 6173 7365 6420 2865 2e67 2e0a 2020   passed (e.g..  
-000192a0: 2020 276d 6165 7374 726f 2070 7573 6820    'maestro push 
-000192b0: 3120 3220 3327 2077 696c 6c20 6d61 6b65  1 2 3' will make
-000192c0: 2074 6865 206d 6f73 7420 7265 6365 6e74   the most recent
-000192d0: 2073 6f6e 6720 6265 2033 292e 0a0a 2020   song be 3)...  
-000192e0: 2020 4966 2074 6865 2027 2d42 2720 666c    If the '-B' fl
-000192f0: 6167 2069 7320 7061 7373 6564 2c20 7468  ag is passed, th
-00019300: 6520 736f 6e67 2873 2920 7769 6c6c 2062  e song(s) will b
-00019310: 6520 7075 7368 6564 2074 6f20 7468 6520  e pushed to the 
-00019320: 626f 7474 6f6d 206f 6620 7468 650a 2020  bottom of the.  
-00019330: 2020 6c69 7374 2069 6e73 7465 6164 2e0a    list instead..
-00019340: 2020 2020 2222 220a 2020 2020 7769 7468      """.    with
-00019350: 206f 7065 6e28 534f 4e47 535f 494e 464f   open(SONGS_INFO
-00019360: 5f50 4154 482c 2022 722b 222c 2065 6e63  _PATH, "r+", enc
-00019370: 6f64 696e 673d 2275 7466 2d38 2229 2061  oding="utf-8") a
-00019380: 7320 736f 6e67 735f 6669 6c65 3a0a 2020  s songs_file:.  
-00019390: 2020 2020 2020 6c69 6e65 7320 3d20 736f        lines = so
-000193a0: 6e67 735f 6669 6c65 2e72 6561 646c 696e  ngs_file.readlin
-000193b0: 6573 2829 0a0a 2020 2020 2020 2020 6c69  es()..        li
-000193c0: 6e65 735f 746f 5f6d 6f76 6520 3d20 5b5d  nes_to_move = []
-000193d0: 0a20 2020 2020 2020 2066 6f72 2069 2069  .        for i i
-000193e0: 6e20 7261 6e67 6528 6c65 6e28 6c69 6e65  n range(len(line
-000193f0: 7329 293a 0a20 2020 2020 2020 2020 2020  s)):.           
-00019400: 2069 6620 696e 7428 6c69 6e65 735b 695d   if int(lines[i]
-00019410: 2e73 706c 6974 2822 7c22 295b 305d 2920  .split("|")[0]) 
-00019420: 696e 2073 6f6e 675f 6964 733a 0a20 2020  in song_ids:.   
-00019430: 2020 2020 2020 2020 2020 2020 206c 696e               lin
-00019440: 6573 5f74 6f5f 6d6f 7665 2e61 7070 656e  es_to_move.appen
-00019450: 6428 2869 2c20 6c69 6e65 735b 695d 2929  d((i, lines[i]))
-00019460: 0a0a 2020 2020 2020 2020 666f 7220 692c  ..        for i,
-00019470: 205f 2069 6e20 7265 7665 7273 6564 286c   _ in reversed(l
-00019480: 696e 6573 5f74 6f5f 6d6f 7665 293a 0a20  ines_to_move):. 
-00019490: 2020 2020 2020 2020 2020 206c 696e 6573             lines
-000194a0: 2e70 6f70 2869 290a 0a20 2020 2020 2020  .pop(i)..       
-000194b0: 2073 6f6e 675f 6964 735f 7769 7468 5f6f   song_ids_with_o
-000194c0: 7264 6572 203d 2064 6963 7428 0a20 2020  rder = dict(.   
-000194d0: 2020 2020 2020 2020 206d 6170 286c 616d           map(lam
-000194e0: 6264 6120 783a 2028 785b 315d 2c20 785b  bda x: (x[1], x[
-000194f0: 305d 292c 2065 6e75 6d65 7261 7465 2873  0]), enumerate(s
-00019500: 6f6e 675f 6964 7329 290a 2020 2020 2020  ong_ids)).      
-00019510: 2020 290a 0a20 2020 2020 2020 2066 6f72    )..        for
-00019520: 2069 2069 6e20 7261 6e67 6528 6c65 6e28   i in range(len(
-00019530: 6c69 6e65 735f 746f 5f6d 6f76 6529 293a  lines_to_move)):
-00019540: 0a20 2020 2020 2020 2020 2020 206c 696e  .            lin
-00019550: 6573 5f74 6f5f 6d6f 7665 5b69 5d20 3d20  es_to_move[i] = 
-00019560: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00019570: 2020 736f 6e67 5f69 6473 5f77 6974 685f    song_ids_with_
-00019580: 6f72 6465 725b 696e 7428 6c69 6e65 735f  order[int(lines_
-00019590: 746f 5f6d 6f76 655b 695d 5b31 5d2e 7370  to_move[i][1].sp
-000195a0: 6c69 7428 227c 2229 5b30 5d29 5d2c 0a20  lit("|")[0])],. 
-000195b0: 2020 2020 2020 2020 2020 2020 2020 202a                 *
-000195c0: 6c69 6e65 735f 746f 5f6d 6f76 655b 695d  lines_to_move[i]
-000195d0: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-000195e0: 0a20 2020 2020 2020 206c 696e 6573 5f74  .        lines_t
-000195f0: 6f5f 6d6f 7665 2e73 6f72 7428 6b65 793d  o_move.sort(key=
-00019600: 6c61 6d62 6461 2078 3a20 785b 305d 2c20  lambda x: x[0], 
-00019610: 7265 7665 7273 653d 626f 7474 6f6d 290a  reverse=bottom).
-00019620: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00019630: 626f 7474 6f6d 3a0a 2020 2020 2020 2020  bottom:.        
-00019640: 2020 2020 6c69 6e65 7320 2b3d 205b 745b      lines += [t[
-00019650: 325d 2066 6f72 2074 2069 6e20 6c69 6e65  2] for t in line
-00019660: 735f 746f 5f6d 6f76 655d 0a20 2020 2020  s_to_move].     
-00019670: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00019680: 2020 2020 206c 696e 6573 203d 205b 745b       lines = [t[
-00019690: 325d 2066 6f72 2074 2069 6e20 6c69 6e65  2] for t in line
-000196a0: 735f 746f 5f6d 6f76 655d 202b 206c 696e  s_to_move] + lin
-000196b0: 6573 0a0a 2020 2020 2020 2020 736f 6e67  es..        song
-000196c0: 735f 6669 6c65 2e73 6565 6b28 3029 0a20  s_file.seek(0). 
-000196d0: 2020 2020 2020 2073 6f6e 6773 5f66 696c         songs_fil
-000196e0: 652e 7772 6974 6528 2222 2e6a 6f69 6e28  e.write("".join(
-000196f0: 6c69 6e65 7329 290a 2020 2020 2020 2020  lines)).        
-00019700: 736f 6e67 735f 6669 6c65 2e74 7275 6e63  songs_file.trunc
-00019710: 6174 6528 290a 0a0a 4063 6c69 2e63 6f6d  ate()...@cli.com
-00019720: 6d61 6e64 286e 616d 653d 2263 6c69 7022  mand(name="clip"
-00019730: 290a 4063 6c69 636b 2e61 7267 756d 656e  ).@click.argumen
-00019740: 7428 2273 6f6e 675f 6964 222c 2072 6571  t("song_id", req
-00019750: 7569 7265 643d 5472 7565 2c20 7479 7065  uired=True, type
-00019760: 3d69 6e74 290a 4063 6c69 636b 2e61 7267  =int).@click.arg
-00019770: 756d 656e 7428 2273 7461 7274 222c 2072  ument("start", r
-00019780: 6571 7569 7265 643d 4661 6c73 652c 2074  equired=False, t
-00019790: 7970 653d 666c 6f61 742c 2064 6566 6175  ype=float, defau
-000197a0: 6c74 3d4e 6f6e 6529 0a40 636c 6963 6b2e  lt=None).@click.
-000197b0: 6172 6775 6d65 6e74 2822 656e 6422 2c20  argument("end", 
-000197c0: 7265 7175 6972 6564 3d46 616c 7365 2c20  required=False, 
-000197d0: 7479 7065 3d66 6c6f 6174 2c20 6465 6661  type=float, defa
-000197e0: 756c 743d 4e6f 6e65 290a 6465 6620 636c  ult=None).def cl
-000197f0: 6970 5f28 736f 6e67 5f69 642c 2073 7461  ip_(song_id, sta
-00019800: 7274 2c20 656e 6429 3a0a 2020 2020 2222  rt, end):.    ""
-00019810: 220a 2020 2020 4372 6561 7465 206f 7220  ".    Create or 
-00019820: 6564 6974 2074 6865 2063 6c69 7020 666f  edit the clip fo
-00019830: 7220 6120 736f 6e67 2e0a 0a20 2020 2053  r a song...    S
-00019840: 6574 7320 7468 6520 636c 6970 2066 6f72  ets the clip for
-00019850: 2074 6865 2073 6f6e 6720 7769 7468 2049   the song with I
-00019860: 4420 534f 4e47 5f49 4420 746f 2074 6865  D SONG_ID to the
-00019870: 2074 696d 6520 7261 6e67 6520 5354 4152   time range STAR
-00019880: 5420 746f 2045 4e44 0a20 2020 2028 696e  T to END.    (in
-00019890: 2073 6563 6f6e 6473 292e 0a0a 2020 2020   seconds)...    
-000198a0: 4966 2045 4e44 2069 7320 6e6f 7420 7061  If END is not pa
-000198b0: 7373 6564 2c20 7468 6520 636c 6970 2077  ssed, the clip w
-000198c0: 696c 6c20 6265 2066 726f 6d20 5354 4152  ill be from STAR
-000198d0: 5420 746f 2074 6865 2065 6e64 206f 6620  T to the end of 
-000198e0: 7468 6520 736f 6e67 2e0a 0a20 2020 2049  the song...    I
-000198f0: 6620 6e65 6974 6865 7220 5354 4152 5420  f neither START 
-00019900: 6e6f 7220 454e 4420 6172 6520 7061 7373  nor END are pass
-00019910: 6564 2c20 6120 636c 6970 2065 6469 746f  ed, a clip edito
-00019920: 7220 7769 6c6c 2062 6520 6f70 656e 6564  r will be opened
-00019930: 2c20 696e 2077 6869 6368 0a20 2020 2079  , in which.    y
-00019940: 6f75 2063 616e 206d 6f76 6520 7468 6520  ou can move the 
-00019950: 7374 6172 7420 616e 6420 656e 6420 6f66  start and end of
-00019960: 2074 6865 2063 6c69 7020 6172 6f75 6e64   the clip around
-00019970: 2075 7369 6e67 2074 6865 2061 7272 6f77   using the arrow
-00019980: 206b 6579 7320 7768 696c 650a 2020 2020   keys while.    
-00019990: 6c69 7374 656e 696e 6720 746f 2074 6865  listening to the
-000199a0: 2073 6f6e 6720 2861 6c73 6f20 7368 6f77   song (also show
-000199b0: 7320 7761 7665 666f 726d 292e 0a0a 2020  s waveform)...  
-000199c0: 2020 5c62 0a20 2020 2054 6865 2065 6469    \b.    The edi
-000199d0: 746f 7220 7374 6172 7473 206f 7574 2065  tor starts out e
-000199e0: 6469 7469 6e67 2074 6865 2073 7461 7274  diting the start
-000199f0: 206f 6620 7468 6520 636c 6970 2e0a 2020   of the clip..  
-00019a00: 2020 5c78 3162 5b31 6d74 5c78 3162 5b30    \x1b[1mt\x1b[0
-00019a10: 6d20 746f 2074 6f67 676c 6520 6265 7477  m to toggle betw
-00019a20: 6565 6e20 6564 6974 696e 6720 7468 6520  een editing the 
-00019a30: 7374 6172 7420 616e 6420 656e 6420 6f66  start and end of
-00019a40: 2074 6865 2063 6c69 702e 0a20 2020 205c   the clip..    \
-00019a50: 7831 625b 316d 5348 4946 542b 4c45 4654  x1b[1mSHIFT+LEFT
-00019a60: 2f52 4947 4854 5c78 3162 5b30 6d20 7769  /RIGHT\x1b[0m wi
-00019a70: 6c6c 206d 6f76 6520 7768 6963 6865 7665  ll move whicheve
-00019a80: 7220 636c 6970 2065 6e64 2079 6f75 2061  r clip end you a
-00019a90: 7265 2065 6469 7469 6e67 0a20 2020 2020  re editing.     
-00019aa0: 2020 2062 7920 302e 3120 7365 636f 6e64     by 0.1 second
-00019ab0: 732c 2073 6e61 7020 7468 6520 6375 7272  s, snap the curr
-00019ac0: 656e 7420 706c 6179 6261 636b 2074 6f20  ent playback to 
-00019ad0: 7468 6174 2063 6c69 7020 656e 6420 2874  that clip end (t
-00019ae0: 6f20 6578 6163 746c 790a 2020 2020 2020  o exactly.      
-00019af0: 2020 7468 6520 636c 6970 2073 7461 7274    the clip start
-00019b00: 2069 6620 6564 6974 696e 6720 7374 6172   if editing star
-00019b10: 742c 2065 6e64 2d31 2069 6620 6564 6974  t, end-1 if edit
-00019b20: 696e 6720 656e 6429 2c20 616e 6420 7061  ing end), and pa
-00019b30: 7573 652e 0a20 2020 205c 7831 625b 316d  use..    \x1b[1m
-00019b40: 4c45 4654 2f52 4947 4854 5c78 3162 5b30  LEFT/RIGHT\x1b[0
-00019b50: 6d20 7769 6c6c 206d 6f76 6520 7768 6963  m will move whic
-00019b60: 6865 7665 7220 636c 6970 2065 6e64 2079  hever clip end y
-00019b70: 6f75 2061 7265 2065 6469 7469 6e67 2062  ou are editing b
-00019b80: 7920 310a 2020 2020 2020 2020 7365 636f  y 1.        seco
-00019b90: 6e64 2c20 736e 6170 2074 6865 2063 7572  nd, snap the cur
-00019ba0: 7265 6e74 2070 6c61 7962 6163 6b20 746f  rent playback to
-00019bb0: 2074 6861 7420 636c 6970 2065 6e64 2c20   that clip end, 
-00019bc0: 616e 6420 7061 7573 652e 0a20 2020 205c  and pause..    \
-00019bd0: 7831 625b 316d 454e 5445 525c 7831 625b  x1b[1mENTER\x1b[
-00019be0: 306d 2077 696c 6c20 6578 6974 2074 6865  0m will exit the
-00019bf0: 2065 6469 746f 7220 616e 6420 7361 7665   editor and save
-00019c00: 2074 6865 2063 6c69 702e 0a20 2020 205c   the clip..    \
-00019c10: 7831 625b 316d 715c 7831 625b 306d 2077  x1b[1mq\x1b[0m w
-00019c20: 696c 6c20 6578 6974 2074 6865 2065 6469  ill exit the edi
-00019c30: 746f 7220 7769 7468 6f75 7420 7361 7669  tor without savi
-00019c40: 6e67 2074 6865 2063 6c69 702e 0a20 2020  ng the clip..   
-00019c50: 2022 2222 0a20 2020 2069 6620 7374 6172   """.    if star
-00019c60: 7420 6973 206e 6f74 204e 6f6e 653a 0a20  t is not None:. 
-00019c70: 2020 2020 2020 2069 6620 7374 6172 7420         if start 
-00019c80: 3c20 303a 0a20 2020 2020 2020 2020 2020  < 0:.           
-00019c90: 2063 6c69 636b 2e73 6563 686f 2822 5354   click.secho("ST
-00019ca0: 4152 5420 6d75 7374 2062 6520 6120 706f  ART must be a po
-00019cb0: 7369 7469 7665 206e 756d 6265 722e 222c  sitive number.",
-00019cc0: 2066 673d 2272 6564 2229 0a20 2020 2020   fg="red").     
-00019cd0: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
-00019ce0: 2020 2020 2020 6966 2065 6e64 2069 7320        if end is 
-00019cf0: 6e6f 7420 4e6f 6e65 2061 6e64 2065 6e64  not None and end
-00019d00: 203c 2030 3a0a 2020 2020 2020 2020 2020   < 0:.          
-00019d10: 2020 636c 6963 6b2e 7365 6368 6f28 2245    click.secho("E
-00019d20: 4e44 206d 7573 7420 6265 2061 2070 6f73  ND must be a pos
-00019d30: 6974 6976 6520 6e75 6d62 6572 2e22 2c20  itive number.", 
-00019d40: 6667 3d22 7265 6422 290a 2020 2020 2020  fg="red").      
-00019d50: 2020 2020 2020 7265 7475 726e 0a0a 2020        return..  
-00019d60: 2020 7769 7468 206f 7065 6e28 534f 4e47    with open(SONG
-00019d70: 535f 494e 464f 5f50 4154 482c 2022 722b  S_INFO_PATH, "r+
-00019d80: 222c 2065 6e63 6f64 696e 673d 2275 7466  ", encoding="utf
-00019d90: 2d38 2229 2061 7320 736f 6e67 735f 6669  -8") as songs_fi
-00019da0: 6c65 3a0a 2020 2020 2020 2020 6c69 6e65  le:.        line
-00019db0: 7320 3d20 736f 6e67 735f 6669 6c65 2e72  s = songs_file.r
-00019dc0: 6561 646c 696e 6573 2829 0a0a 2020 2020  eadlines()..    
-00019dd0: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-00019de0: 6765 286c 656e 286c 696e 6573 2929 3a0a  ge(len(lines)):.
-00019df0: 2020 2020 2020 2020 2020 2020 6465 7461              deta
-00019e00: 696c 7320 3d20 6c69 6e65 735b 695d 2e73  ils = lines[i].s
-00019e10: 7472 6970 2829 2e73 706c 6974 2822 7c22  trip().split("|"
-00019e20: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-00019e30: 2069 6e74 2864 6574 6169 6c73 5b30 5d29   int(details[0])
-00019e40: 203d 3d20 736f 6e67 5f69 643a 0a20 2020   == song_id:.   
-00019e50: 2020 2020 2020 2020 2020 2020 2062 7265               bre
-00019e60: 616b 0a20 2020 2020 2020 2065 6c73 653a  ak.        else:
-00019e70: 0a20 2020 2020 2020 2020 2020 2063 6c69  .            cli
-00019e80: 636b 2e73 6563 686f 2866 224e 6f20 736f  ck.secho(f"No so
-00019e90: 6e67 2066 6f75 6e64 2077 6974 6820 4944  ng found with ID
-00019ea0: 207b 736f 6e67 5f69 647d 2e22 2c20 6667   {song_id}.", fg
-00019eb0: 3d22 7265 6422 290a 2020 2020 2020 2020  ="red").        
-00019ec0: 2020 2020 7265 7475 726e 0a0a 2020 2020      return..    
-00019ed0: 2020 2020 736f 6e67 5f6e 616d 6520 3d20      song_name = 
-00019ee0: 6465 7461 696c 735b 315d 0a0a 2020 2020  details[1]..    
-00019ef0: 2020 2020 6966 2073 7461 7274 2069 7320      if start is 
-00019f00: 4e6f 6e65 3a20 2023 2063 6c69 7020 6564  None:  # clip ed
-00019f10: 6974 6f72 0a20 2020 2020 2020 2020 2020  itor.           
-00019f20: 2073 7461 7274 2c20 656e 6420 3d20 6375   start, end = cu
-00019f30: 7273 6573 2e77 7261 7070 6572 2863 6c69  rses.wrapper(cli
-00019f40: 705f 6564 6974 6f72 2c20 6465 7461 696c  p_editor, detail
-00019f50: 7329 0a20 2020 2020 2020 2020 2020 2069  s).            i
-00019f60: 6620 7374 6172 7420 6973 204e 6f6e 653a  f start is None:
-00019f70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019f80: 2063 6c69 636b 2e73 6563 686f 2866 224e   click.secho(f"N
-00019f90: 6f20 6368 616e 6765 2069 6e20 636c 6970  o change in clip
-00019fa0: 2066 6f72 207b 736f 6e67 5f6e 616d 657d   for {song_name}
-00019fb0: 2e22 2c20 6667 3d22 6772 6565 6e22 290a  .", fg="green").
-00019fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019fd0: 7265 7475 726e 0a0a 2020 2020 2020 2020  return..        
-00019fe0: 736f 6e67 5f70 6174 6820 3d20 6f73 2e70  song_path = os.p
-00019ff0: 6174 682e 6a6f 696e 2853 4f4e 4753 5f44  ath.join(SONGS_D
-0001a000: 4952 2c20 736f 6e67 5f6e 616d 6529 0a20  IR, song_name). 
-0001a010: 2020 2020 2020 2064 7572 6174 696f 6e20         duration 
-0001a020: 3d20 6d75 7369 635f 7461 672e 6c6f 6164  = music_tag.load
-0001a030: 5f66 696c 6528 736f 6e67 5f70 6174 6829  _file(song_path)
-0001a040: 5b22 236c 656e 6774 6822 5d2e 7661 6c75  ["#length"].valu
-0001a050: 650a 0a20 2020 2020 2020 2069 6620 656e  e..        if en
-0001a060: 6420 6973 204e 6f6e 653a 0a20 2020 2020  d is None:.     
-0001a070: 2020 2020 2020 2065 6e64 203d 2064 7572         end = dur
-0001a080: 6174 696f 6e0a 0a20 2020 2020 2020 2069  ation..        i
-0001a090: 6620 7374 6172 7420 3e20 6475 7261 7469  f start > durati
-0001a0a0: 6f6e 3a0a 2020 2020 2020 2020 2020 2020  on:.            
-0001a0b0: 636c 6963 6b2e 7365 6368 6f28 0a20 2020  click.secho(.   
-0001a0c0: 2020 2020 2020 2020 2020 2020 2022 5354               "ST
-0001a0d0: 4152 5420 6d75 7374 206e 6f74 2062 6520  ART must not be 
-0001a0e0: 6d6f 7265 2074 6861 6e20 7468 6520 736f  more than the so
-0001a0f0: 6e67 2064 7572 6174 696f 6e2e 222c 2066  ng duration.", f
-0001a100: 673d 2272 6564 220a 2020 2020 2020 2020  g="red".        
-0001a110: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-0001a120: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
-0001a130: 2069 6620 656e 6420 3e20 6475 7261 7469   if end > durati
-0001a140: 6f6e 3a0a 2020 2020 2020 2020 2020 2020  on:.            
-0001a150: 636c 6963 6b2e 7365 6368 6f28 0a20 2020  click.secho(.   
-0001a160: 2020 2020 2020 2020 2020 2020 2022 454e               "EN
-0001a170: 4420 6d75 7374 206e 6f74 2062 6520 6d6f  D must not be mo
-0001a180: 7265 2074 6861 6e20 7468 6520 736f 6e67  re than the song
-0001a190: 2064 7572 6174 696f 6e2e 222c 2066 673d   duration.", fg=
-0001a1a0: 2272 6564 220a 2020 2020 2020 2020 2020  "red".          
-0001a1b0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-0001a1c0: 7265 7475 726e 0a20 2020 2020 2020 2069  return.        i
-0001a1d0: 6620 7374 6172 7420 3e20 656e 643a 0a20  f start > end:. 
-0001a1e0: 2020 2020 2020 2020 2020 2063 6c69 636b             click
-0001a1f0: 2e73 6563 686f 2822 5354 4152 5420 6d75  .secho("START mu
-0001a200: 7374 206e 6f74 2062 6520 6d6f 7265 2074  st not be more t
-0001a210: 6861 6e20 454e 442e 222c 2066 673d 2272  han END.", fg="r
-0001a220: 6564 2229 0a20 2020 2020 2020 2020 2020  ed").           
-0001a230: 2072 6574 7572 6e0a 0a20 2020 2020 2020   return..       
-0001a240: 206c 696e 6573 5b69 5d20 3d20 280a 2020   lines[i] = (.  
-0001a250: 2020 2020 2020 2020 2020 227c 222e 6a6f            "|".jo
-0001a260: 696e 2864 6574 6169 6c73 5b3a 335d 202b  in(details[:3] +
-0001a270: 205b 7374 7228 7374 6172 7429 202b 2022   [str(start) + "
-0001a280: 2022 202b 2073 7472 2865 6e64 295d 202b   " + str(end)] +
-0001a290: 2064 6574 6169 6c73 5b35 3a5d 290a 2020   details[5:]).  
-0001a2a0: 2020 2020 2020 2020 2020 2b20 225c 6e22            + "\n"
-0001a2b0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-0001a2c0: 2020 2020 736f 6e67 735f 6669 6c65 2e73      songs_file.s
-0001a2d0: 6565 6b28 3029 0a20 2020 2020 2020 2073  eek(0).        s
-0001a2e0: 6f6e 6773 5f66 696c 652e 7772 6974 6528  ongs_file.write(
-0001a2f0: 2222 2e6a 6f69 6e28 6c69 6e65 7329 290a  "".join(lines)).
-0001a300: 2020 2020 2020 2020 736f 6e67 735f 6669          songs_fi
-0001a310: 6c65 2e74 7275 6e63 6174 6528 290a 0a20  le.truncate().. 
-0001a320: 2020 2020 2020 2063 6c69 636b 2e73 6563         click.sec
-0001a330: 686f 2866 2243 6c69 7070 6564 207b 736f  ho(f"Clipped {so
-0001a340: 6e67 5f6e 616d 657d 2066 726f 6d20 7b73  ng_name} from {s
-0001a350: 7461 7274 7d20 746f 207b 656e 647d 2e22  tart} to {end}."
-0001a360: 2c20 6667 3d22 6772 6565 6e22 290a 0a0a  , fg="green")...
-0001a370: 4063 6c69 2e63 6f6d 6d61 6e64 2829 0a40  @cli.command().@
-0001a380: 636c 6963 6b2e 6172 6775 6d65 6e74 2822  click.argument("
-0001a390: 736f 6e67 5f69 6473 222c 2074 7970 653d  song_ids", type=
-0001a3a0: 696e 742c 206e 6172 6773 3d2d 312c 2072  int, nargs=-1, r
-0001a3b0: 6571 7569 7265 643d 4661 6c73 6529 0a40  equired=False).@
-0001a3c0: 636c 6963 6b2e 6f70 7469 6f6e 280a 2020  click.option(.  
-0001a3d0: 2020 222d 412f 2d6e 4122 2c0a 2020 2020    "-A/-nA",.    
-0001a3e0: 222d 2d61 6c6c 2f2d 2d6e 6f2d 616c 6c22  "--all/--no-all"
-0001a3f0: 2c0a 2020 2020 2261 6c6c 5f22 2c0a 2020  ,.    "all_",.  
-0001a400: 2020 6465 6661 756c 743d 4661 6c73 652c    default=False,
-0001a410: 0a20 2020 2068 656c 703d 2252 656d 6f76  .    help="Remov
-0001a420: 6520 636c 6970 7320 666f 7220 616c 6c20  e clips for all 
-0001a430: 736f 6e67 732e 2049 676e 6f72 6573 2053  songs. Ignores S
-0001a440: 4f4e 475f 4944 532e 222c 0a29 0a40 636c  ONG_IDS.",.).@cl
-0001a450: 6963 6b2e 6f70 7469 6f6e 2822 2d46 2f2d  ick.option("-F/-
-0001a460: 6e46 222c 2022 2d2d 666f 7263 652f 2d2d  nF", "--force/--
-0001a470: 6e6f 2d66 6f72 6365 222c 2022 666f 7263  no-force", "forc
-0001a480: 6522 2c20 6465 6661 756c 743d 4661 6c73  e", default=Fals
-0001a490: 6529 0a64 6566 2075 6e63 6c69 7028 736f  e).def unclip(so
-0001a4a0: 6e67 5f69 6473 2c20 616c 6c5f 2c20 666f  ng_ids, all_, fo
-0001a4b0: 7263 6529 3a0a 2020 2020 2222 220a 2020  rce):.    """.  
-0001a4c0: 2020 5265 6d6f 7665 2063 6c69 7073 2066    Remove clips f
-0001a4d0: 6f72 2073 7065 6369 6669 6320 736f 6e67  or specific song
-0001a4e0: 2873 292e 0a0a 2020 2020 5265 6d6f 7665  (s)...    Remove
-0001a4f0: 7320 636c 6970 2066 6f72 2074 6865 2073  s clip for the s
-0001a500: 6f6e 6728 7329 2077 6974 6820 4944 2873  ong(s) with ID(s
-0001a510: 2920 534f 4e47 5f49 4453 2e0a 0a20 2020  ) SONG_IDS...   
-0001a520: 2049 6620 7468 6520 272d 412f 2d2d 616c   If the '-A/--al
-0001a530: 6c27 2066 6c61 6720 6973 2070 6173 7365  l' flag is passe
-0001a540: 642c 2074 6865 2063 6c69 7073 2066 6f72  d, the clips for
-0001a550: 2061 6c6c 2073 6f6e 6773 2077 696c 6c20   all songs will 
-0001a560: 6265 2072 656d 6f76 6564 2c0a 2020 2020  be removed,.    
-0001a570: 6967 6e6f 7269 6e67 2053 4f4e 475f 4944  ignoring SONG_ID
-0001a580: 532e 2054 6869 7320 7072 6f6d 7074 7320  S. This prompts 
-0001a590: 666f 7220 636f 6e66 6972 6d61 7469 6f6e  for confirmation
-0001a5a0: 2075 6e6c 6573 7320 7468 6520 272d 462f   unless the '-F/
-0001a5b0: 2d2d 666f 7263 6527 0a20 2020 2066 6c61  --force'.    fla
-0001a5c0: 6720 6973 2070 6173 7365 642e 0a20 2020  g is passed..   
-0001a5d0: 2022 2222 0a20 2020 2069 6620 6e6f 7420   """.    if not 
-0001a5e0: 616c 6c5f 3a0a 2020 2020 2020 2020 6966  all_:.        if
-0001a5f0: 2073 6f6e 675f 6964 733a 0a20 2020 2020   song_ids:.     
-0001a600: 2020 2020 2020 2073 6f6e 675f 6964 7320         song_ids 
-0001a610: 3d20 7365 7428 736f 6e67 5f69 6473 290a  = set(song_ids).
-0001a620: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0001a630: 2020 2020 2020 2020 2020 636c 6963 6b2e            click.
-0001a640: 7365 6368 6f28 0a20 2020 2020 2020 2020  secho(.         
-0001a650: 2020 2020 2020 2022 4e6f 2073 6f6e 6720         "No song 
-0001a660: 4944 7320 7061 7373 6564 2e20 546f 2072  IDs passed. To r
-0001a670: 656d 6f76 6520 636c 6970 7320 666f 7220  emove clips for 
-0001a680: 616c 6c20 736f 6e67 732c 2070 6173 7320  all songs, pass 
-0001a690: 7468 6520 272d 412f 2d2d 616c 6c27 2066  the '-A/--all' f
-0001a6a0: 6c61 672e 222c 0a20 2020 2020 2020 2020  lag.",.         
-0001a6b0: 2020 2020 2020 2066 673d 2272 6564 222c         fg="red",
-0001a6c0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-0001a6d0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0001a6e0: 6e0a 0a20 2020 2069 6620 616c 6c5f 2061  n..    if all_ a
-0001a6f0: 6e64 206e 6f74 2066 6f72 6365 3a0a 2020  nd not force:.  
-0001a700: 2020 2020 2020 636c 6963 6b2e 6563 686f        click.echo
-0001a710: 280a 2020 2020 2020 2020 2020 2020 2241  (.            "A
-0001a720: 7265 2079 6f75 2073 7572 6520 796f 7520  re you sure you 
-0001a730: 7761 6e74 2074 6f20 7265 6d6f 7665 2063  want to remove c
-0001a740: 6c69 7073 2066 6f72 2061 6c6c 2073 6f6e  lips for all son
-0001a750: 6773 3f20 5468 6973 2063 616e 6e6f 7420  gs? This cannot 
-0001a760: 6265 2075 6e64 6f6e 652e 205b 792f 6e5d  be undone. [y/n]
-0001a770: 2022 2c0a 2020 2020 2020 2020 290a 2020   ",.        ).  
-0001a780: 2020 2020 2020 6966 2069 6e70 7574 2829        if input()
-0001a790: 2e6c 6f77 6572 2829 2021 3d20 2279 223a  .lower() != "y":
-0001a7a0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0001a7b0: 7572 6e0a 0a20 2020 2077 6974 6820 6f70  urn..    with op
-0001a7c0: 656e 2853 4f4e 4753 5f49 4e46 4f5f 5041  en(SONGS_INFO_PA
-0001a7d0: 5448 2c20 2272 2b22 2c20 656e 636f 6469  TH, "r+", encodi
-0001a7e0: 6e67 3d22 7574 662d 3822 2920 6173 2073  ng="utf-8") as s
-0001a7f0: 6f6e 6773 5f66 696c 653a 0a20 2020 2020  ongs_file:.     
-0001a800: 2020 206c 696e 6573 203d 2073 6f6e 6773     lines = songs
-0001a810: 5f66 696c 652e 7265 6164 6c69 6e65 7328  _file.readlines(
-0001a820: 290a 0a20 2020 2020 2020 2066 6f72 2069  )..        for i
-0001a830: 2069 6e20 7261 6e67 6528 6c65 6e28 6c69   in range(len(li
-0001a840: 6e65 7329 293a 0a20 2020 2020 2020 2020  nes)):.         
-0001a850: 2020 2064 6574 6169 6c73 203d 206c 696e     details = lin
-0001a860: 6573 5b69 5d2e 7374 7269 7028 292e 7370  es[i].strip().sp
-0001a870: 6c69 7428 227c 2229 0a20 2020 2020 2020  lit("|").       
-0001a880: 2020 2020 2069 6620 616c 6c5f 206f 7220       if all_ or 
-0001a890: 696e 7428 6465 7461 696c 735b 305d 2920  int(details[0]) 
-0001a8a0: 696e 2073 6f6e 675f 6964 733a 0a20 2020  in song_ids:.   
-0001a8b0: 2020 2020 2020 2020 2020 2020 206c 696e               lin
-0001a8c0: 6573 5b69 5d20 3d20 227c 222e 6a6f 696e  es[i] = "|".join
-0001a8d0: 2864 6574 6169 6c73 5b3a 335d 202b 205b  (details[:3] + [
-0001a8e0: 2222 5d20 2b20 6465 7461 696c 735b 353a  ""] + details[5:
-0001a8f0: 5d29 202b 2022 5c6e 220a 0a20 2020 2020  ]) + "\n"..     
-0001a900: 2020 2073 6f6e 6773 5f66 696c 652e 7365     songs_file.se
-0001a910: 656b 2830 290a 2020 2020 2020 2020 736f  ek(0).        so
-0001a920: 6e67 735f 6669 6c65 2e77 7269 7465 2822  ngs_file.write("
-0001a930: 222e 6a6f 696e 286c 696e 6573 2929 0a20  ".join(lines)). 
-0001a940: 2020 2020 2020 2073 6f6e 6773 5f66 696c         songs_fil
-0001a950: 652e 7472 756e 6361 7465 2829 0a0a 2020  e.truncate()..  
-0001a960: 2020 6966 2061 6c6c 5f3a 0a20 2020 2020    if all_:.     
-0001a970: 2020 2063 6c69 636b 2e73 6563 686f 2822     click.secho("
-0001a980: 5265 6d6f 7665 6420 636c 6970 7320 666f  Removed clips fo
-0001a990: 7220 616c 6c20 736f 6e67 732e 222c 2066  r all songs.", f
-0001a9a0: 673d 2267 7265 656e 2229 0a20 2020 2065  g="green").    e
-0001a9b0: 6c73 653a 0a20 2020 2020 2020 2063 6c69  lse:.        cli
-0001a9c0: 636b 2e73 6563 686f 280a 2020 2020 2020  ck.secho(.      
-0001a9d0: 2020 2020 2020 6622 5265 6d6f 7665 6420        f"Removed 
-0001a9e0: 636c 6970 2873 2920 666f 7220 736f 6e67  clip(s) for song
-0001a9f0: 2873 2920 7769 7468 2049 4428 7329 207b  (s) with ID(s) {
-0001aa00: 272c 2027 2e6a 6f69 6e28 6d61 7028 7374  ', '.join(map(st
-0001aa10: 722c 2073 6f6e 675f 6964 7329 297d 2e22  r, song_ids))}."
-0001aa20: 2c0a 2020 2020 2020 2020 2020 2020 6667  ,.            fg
-0001aa30: 3d22 6772 6565 6e22 2c0a 2020 2020 2020  ="green",.      
-0001aa40: 2020 290a 0a0a 4063 6c69 2e63 6f6d 6d61    )...@cli.comma
-0001aa50: 6e64 2829 0a40 636c 6963 6b2e 6172 6775  nd().@click.argu
-0001aa60: 6d65 6e74 2822 736f 6e67 5f69 6422 2c20  ment("song_id", 
-0001aa70: 7479 7065 3d69 6e74 2c20 7265 7175 6972  type=int, requir
-0001aa80: 6564 3d54 7275 6529 0a40 636c 6963 6b2e  ed=True).@click.
-0001aa90: 6172 6775 6d65 6e74 2822 7061 6972 7322  argument("pairs"
-0001aaa0: 2c20 7479 7065 3d73 7472 2c20 7265 7175  , type=str, requ
-0001aab0: 6972 6564 3d46 616c 7365 290a 6465 6620  ired=False).def 
-0001aac0: 6d65 7461 6461 7461 2873 6f6e 675f 6964  metadata(song_id
-0001aad0: 2c20 7061 6972 7329 3a0a 2020 2020 2222  , pairs):.    ""
-0001aae0: 220a 2020 2020 5669 6577 206f 7220 6564  ".    View or ed
-0001aaf0: 6974 2074 6865 206d 6574 6164 6174 6120  it the metadata 
-0001ab00: 666f 7220 6120 736f 6e67 2e0a 0a20 2020  for a song...   
-0001ab10: 2049 6620 6e6f 2050 4149 5253 2061 7265   If no PAIRS are
-0001ab20: 2070 6173 7365 642c 2070 7269 6e74 7320   passed, prints 
-0001ab30: 7468 6520 6d65 7461 6461 7461 2066 6f72  the metadata for
-0001ab40: 2074 6865 2073 6f6e 6720 7769 7468 2049   the song with I
-0001ab50: 4420 534f 4e47 5f49 442e 0a0a 2020 2020  D SONG_ID...    
-0001ab60: 4966 2050 4149 5253 2061 7265 2070 6173  If PAIRS are pas
-0001ab70: 7365 642c 2073 6574 7320 7468 6520 6d65  sed, sets the me
-0001ab80: 7461 6461 7461 2066 6f72 2074 6865 2073  tadata for the s
-0001ab90: 6f6e 6720 7769 7468 2049 4420 534f 4e47  ong with ID SONG
-0001aba0: 5f49 4420 746f 2074 6865 0a20 2020 206b  _ID to the.    k
-0001abb0: 6579 2d76 616c 7565 2070 6169 7273 2069  ey-value pairs i
-0001abc0: 6e20 5041 4952 532e 2050 4149 5253 2073  n PAIRS. PAIRS s
-0001abd0: 686f 756c 6420 6265 2061 2073 7472 696e  hould be a strin
-0001abe0: 6720 6f66 2074 6865 2066 6f72 6d0a 2020  g of the form.  
-0001abf0: 2020 276b 6579 313a 7661 6c75 6531 7c6b    'key1:value1|k
-0001ac00: 6579 323a 7661 6c75 6532 7c2e 2e2e 272e  ey2:value2|...'.
-0001ac10: 0a0a 2020 2020 506f 7373 6962 6c65 2065  ..    Possible e
-0001ac20: 6469 7461 626c 6520 6d65 7461 6461 7461  ditable metadata
-0001ac30: 206b 6579 7320 6172 653a 2061 6c62 756d   keys are: album
-0001ac40: 2c20 616c 6275 6d61 7274 6973 742c 2061  , albumartist, a
-0001ac50: 7274 6973 742c 2061 7274 776f 726b 2c0a  rtist, artwork,.
-0001ac60: 2020 2020 636f 6d6d 656e 742c 2063 6f6d      comment, com
-0001ac70: 7069 6c61 7469 6f6e 2c20 636f 6d70 6f73  pilation, compos
-0001ac80: 6572 2c20 6469 7363 6e75 6d62 6572 2c20  er, discnumber, 
-0001ac90: 6765 6e72 652c 206c 7972 6963 732c 2074  genre, lyrics, t
-0001aca0: 6f74 616c 6469 7363 732c 0a20 2020 2074  otaldiscs,.    t
-0001acb0: 6f74 616c 7472 6163 6b73 2c20 7472 6163  otaltracks, trac
-0001acc0: 6b6e 756d 6265 722c 2074 7261 636b 7469  knumber, trackti
-0001acd0: 746c 652c 2079 6561 722c 2069 7372 630a  tle, year, isrc.
-0001ace0: 0a20 2020 204b 6579 7320 6172 6520 6e6f  .    Keys are no
-0001acf0: 7420 6361 7365 2073 656e 7369 7469 7665  t case sensitive
-0001ad00: 2061 6e64 2063 616e 2063 6f6e 7461 696e   and can contain
-0001ad10: 2061 7262 6974 7261 7279 2077 6869 7465   arbitrary white
-0001ad20: 7370 6163 652c 2027 2d27 2c20 616e 640a  space, '-', and.
-0001ad30: 2020 2020 275f 2720 6368 6172 6163 7465      '_' characte
-0001ad40: 7273 2e20 496e 206f 7468 6572 2077 6f72  rs. In other wor
-0001ad50: 6473 2c20 2741 6c62 756d 2041 7274 6973  ds, 'Album Artis
-0001ad60: 7427 2c20 2761 6c62 756d 2d61 7274 6973  t', 'album-artis
-0001ad70: 7427 2c20 616e 640a 2020 2020 2761 6c62  t', and.    'alb
-0001ad80: 756d 5f61 7274 6973 7427 2061 7265 2061  um_artist' are a
-0001ad90: 6c6c 2073 796e 6f6e 796d 7320 666f 7220  ll synonyms for 
-0001ada0: 2761 6c62 756d 6172 7469 7374 272e 2041  'albumartist'. A
-0001adb0: 6c73 6f2c 2027 6469 736b 2720 6973 0a20  lso, 'disk' is. 
-0001adc0: 2020 2073 796e 6f6e 796d 6f75 7320 7769     synonymous wi
-0001add0: 7468 2027 6469 7363 272e 0a20 2020 2022  th 'disc'..    "
-0001ade0: 2222 0a0a 2020 2020 7769 7468 206f 7065  ""..    with ope
-0001adf0: 6e28 534f 4e47 535f 494e 464f 5f50 4154  n(SONGS_INFO_PAT
-0001ae00: 482c 2022 7222 2c20 656e 636f 6469 6e67  H, "r", encoding
-0001ae10: 3d22 7574 662d 3822 2920 6173 2073 6f6e  ="utf-8") as son
-0001ae20: 6773 5f66 696c 653a 0a20 2020 2020 2020  gs_file:.       
-0001ae30: 206c 696e 6573 203d 2073 6f6e 6773 5f66   lines = songs_f
-0001ae40: 696c 652e 7265 6164 6c69 6e65 7328 290a  ile.readlines().
-0001ae50: 0a20 2020 2020 2020 2066 6f72 2069 2069  .        for i i
-0001ae60: 6e20 7261 6e67 6528 6c65 6e28 6c69 6e65  n range(len(line
-0001ae70: 7329 293a 0a20 2020 2020 2020 2020 2020  s)):.           
-0001ae80: 2064 6574 6169 6c73 203d 206c 696e 6573   details = lines
-0001ae90: 5b69 5d2e 7374 7269 7028 292e 7370 6c69  [i].strip().spli
-0001aea0: 7428 227c 2229 0a20 2020 2020 2020 2020  t("|").         
-0001aeb0: 2020 2069 6620 696e 7428 6465 7461 696c     if int(detail
-0001aec0: 735b 305d 2920 3d3d 2073 6f6e 675f 6964  s[0]) == song_id
-0001aed0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001aee0: 2020 736f 6e67 5f70 6174 6820 3d20 6f73    song_path = os
-0001aef0: 2e70 6174 682e 6a6f 696e 2853 4f4e 4753  .path.join(SONGS
-0001af00: 5f44 4952 2c20 6465 7461 696c 735b 315d  _DIR, details[1]
-0001af10: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001af20: 2020 736f 6e67 5f6e 616d 6520 3d20 6465    song_name = de
-0001af30: 7461 696c 735b 315d 0a20 2020 2020 2020  tails[1].       
-0001af40: 2020 2020 2020 2020 2062 7265 616b 0a20           break. 
-0001af50: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0001af60: 2020 2020 2020 2020 2063 6c69 636b 2e73           click.s
-0001af70: 6563 686f 280a 2020 2020 2020 2020 2020  echo(.          
-0001af80: 2020 2020 2020 6622 4e6f 2073 6f6e 6720        f"No song 
-0001af90: 7769 7468 2049 4420 7b73 6f6e 675f 6964  with ID {song_id
-0001afa0: 7d20 666f 756e 642e 222c 0a20 2020 2020  } found.",.     
-0001afb0: 2020 2020 2020 2020 2020 2066 673d 2272             fg="r
-0001afc0: 6564 222c 0a20 2020 2020 2020 2020 2020  ed",.           
-0001afd0: 2029 0a20 2020 2020 2020 2020 2020 2072   ).            r
-0001afe0: 6574 7572 6e0a 0a20 2020 2069 6620 7061  eturn..    if pa
-0001aff0: 6972 733a 0a20 2020 2020 2020 2070 6169  irs:.        pai
-0001b000: 7273 203d 205b 7475 706c 6528 7061 6972  rs = [tuple(pair
-0001b010: 2e73 7472 6970 2829 2e73 706c 6974 2822  .strip().split("
-0001b020: 3a22 2929 2066 6f72 2070 6169 7220 696e  :")) for pair in
-0001b030: 2070 6169 7273 2e73 706c 6974 2822 7c22   pairs.split("|"
-0001b040: 295d 0a0a 2020 2020 2020 2020 736f 6e67  )]..        song
-0001b050: 5f64 6174 6120 3d20 6d75 7369 635f 7461  _data = music_ta
-0001b060: 672e 6c6f 6164 5f66 696c 6528 736f 6e67  g.load_file(song
-0001b070: 5f70 6174 6829 0a20 2020 2020 2020 2076  _path).        v
-0001b080: 616c 6964 5f70 6169 7273 203d 2070 6169  alid_pairs = pai
-0001b090: 7273 5b3a 5d0a 2020 2020 2020 2020 666f  rs[:].        fo
-0001b0a0: 7220 6b65 792c 2076 616c 7565 2069 6e20  r key, value in 
-0001b0b0: 7061 6972 733a 0a20 2020 2020 2020 2020  pairs:.         
-0001b0c0: 2020 2069 6620 6b65 7920 6e6f 7420 696e     if key not in
-0001b0d0: 204d 4554 4144 4154 415f 4b45 5953 206f   METADATA_KEYS o
-0001b0e0: 7220 6b65 792e 7374 6172 7473 7769 7468  r key.startswith
-0001b0f0: 2822 2322 293a 0a20 2020 2020 2020 2020  ("#"):.         
-0001b100: 2020 2020 2020 2063 6c69 636b 2e73 6563         click.sec
-0001b110: 686f 280a 2020 2020 2020 2020 2020 2020  ho(.            
-0001b120: 2020 2020 2020 2020 6622 277b 6b65 797d          f"'{key}
-0001b130: 2720 6973 206e 6f74 2061 2076 616c 6964  ' is not a valid
-0001b140: 2065 6469 7461 626c 6520 6d65 7461 6461   editable metada
-0001b150: 7461 206b 6579 2e22 2c20 6667 3d22 7265  ta key.", fg="re
-0001b160: 6422 0a20 2020 2020 2020 2020 2020 2020  d".             
-0001b170: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-0001b180: 2020 2020 2076 616c 6964 5f70 6169 7273       valid_pairs
-0001b190: 2e72 656d 6f76 6528 286b 6579 2c20 7661  .remove((key, va
-0001b1a0: 6c75 6529 290a 2020 2020 2020 2020 2020  lue)).          
-0001b1b0: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
-0001b1c0: 2020 2020 2020 2020 2020 2073 6f6e 675f             song_
-0001b1d0: 6461 7461 5b6b 6579 5d20 3d20 7661 6c75  data[key] = valu
-0001b1e0: 650a 0a20 2020 2020 2020 2073 6f6e 675f  e..        song_
-0001b1f0: 6461 7461 2e73 6176 6528 290a 0a20 2020  data.save()..   
-0001b200: 2020 2020 2063 6c69 636b 2e73 6563 686f       click.secho
-0001b210: 280a 2020 2020 2020 2020 2020 2020 6622  (.            f"
-0001b220: 5365 7420 6d65 7461 6461 7461 2066 6f72  Set metadata for
-0001b230: 2027 7b73 6f6e 675f 6e61 6d65 7d27 2077   '{song_name}' w
-0001b240: 6974 6820 4944 207b 736f 6e67 5f69 647d  ith ID {song_id}
-0001b250: 2074 6f20 7b76 616c 6964 5f70 6169 7273   to {valid_pairs
-0001b260: 7d2e 222c 0a20 2020 2020 2020 2020 2020  }.",.           
-0001b270: 2066 673d 2267 7265 656e 222c 0a20 2020   fg="green",.   
-0001b280: 2020 2020 2029 0a20 2020 2065 6c73 653a       ).    else:
-0001b290: 0a20 2020 2020 2020 2073 6f6e 675f 6461  .        song_da
-0001b2a0: 7461 203d 206d 7573 6963 5f74 6167 2e6c  ta = music_tag.l
-0001b2b0: 6f61 645f 6669 6c65 2873 6f6e 675f 7061  oad_file(song_pa
-0001b2c0: 7468 290a 2020 2020 2020 2020 636c 6963  th).        clic
-0001b2d0: 6b2e 6563 686f 2822 4d65 7461 6461 7461  k.echo("Metadata
-0001b2e0: 2066 6f72 2022 2c20 6e6c 3d46 616c 7365   for ", nl=False
-0001b2f0: 290a 2020 2020 2020 2020 636c 6963 6b2e  ).        click.
-0001b300: 7365 6368 6f28 736f 6e67 5f6e 616d 652c  secho(song_name,
-0001b310: 2066 673d 2262 6c75 6522 2c20 626f 6c64   fg="blue", bold
-0001b320: 3d54 7275 652c 206e 6c3d 4661 6c73 6529  =True, nl=False)
-0001b330: 0a20 2020 2020 2020 2063 6c69 636b 2e65  .        click.e
-0001b340: 6368 6f28 6622 2077 6974 6820 4944 207b  cho(f" with ID {
-0001b350: 736f 6e67 5f69 647d 3a22 290a 0a20 2020  song_id}:")..   
-0001b360: 2020 2020 2066 6f72 206b 6579 2069 6e20       for key in 
-0001b370: 4d45 5441 4441 5441 5f4b 4559 533a 0a20  METADATA_KEYS:. 
-0001b380: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
-0001b390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b3a0: 636c 6963 6b2e 6563 686f 280a 2020 2020  click.echo(.    
-0001b3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b3c0: 6622 5c74 7b6b 6579 2069 6620 6e6f 7420  f"\t{key if not 
-0001b3d0: 6b65 792e 7374 6172 7473 7769 7468 2827  key.startswith('
-0001b3e0: 2327 2920 656c 7365 206b 6579 5b31 3a5d  #') else key[1:]
-0001b3f0: 7d3a 207b 736f 6e67 5f64 6174 615b 6b65  }: {song_data[ke
-0001b400: 795d 2e76 616c 7565 7d22 0a20 2020 2020  y].value}".     
-0001b410: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0001b420: 2020 2020 2020 2020 2065 7863 6570 743a           except:
-0001b430: 2020 2320 7079 6c69 6e74 3a20 6469 7361    # pylint: disa
-0001b440: 626c 653d 6261 7265 2d65 7863 6570 740a  ble=bare-except.
-0001b450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b460: 7061 7373 0a                             pass.
+00018d60: 2073 7461 7473 5f66 696c 652e 7265 6164   stats_file.read
+00018d70: 6c69 6e65 7328 292c 0a20 2020 2020 2020  lines(),.       
+00018d80: 2020 2020 2020 2020 2020 2020 2029 2c0a               ),.
+00018d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018da0: 290a 2020 2020 2020 2020 2020 2020 290a  ).            ).
+00018db0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00018dc0: 6920 696e 2072 616e 6765 286c 656e 286c  i in range(len(l
+00018dd0: 696e 6573 2929 3a0a 2020 2020 2020 2020  ines)):.        
+00018de0: 2020 2020 2020 2020 6465 7461 696c 7320          details 
+00018df0: 3d20 6c69 6e65 735b 695d 2e73 7472 6970  = lines[i].strip
+00018e00: 2829 2e73 706c 6974 2822 7c22 290a 2020  ().split("|").  
+00018e10: 2020 2020 2020 2020 2020 2020 2020 736f                so
+00018e20: 6e67 5f69 6420 3d20 696e 7428 6465 7461  ng_id = int(deta
+00018e30: 696c 735b 305d 290a 2020 2020 2020 2020  ils[0]).        
+00018e40: 2020 2020 2020 2020 6966 2073 6f6e 675f          if song_
+00018e50: 6964 2069 6e20 736f 6e67 5f69 6473 3a0a  id in song_ids:.
+00018e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018e70: 2020 2020 6966 206e 6f74 206f 732e 7061      if not os.pa
+00018e80: 7468 2e65 7869 7374 7328 6f73 2e70 6174  th.exists(os.pat
+00018e90: 682e 6a6f 696e 2853 4f4e 4753 5f44 4952  h.join(SONGS_DIR
+00018ea0: 2c20 6465 7461 696c 735b 315d 2929 3a0a  , details[1])):.
+00018eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018ec0: 2020 2020 2020 2020 636c 6963 6b2e 7365          click.se
+00018ed0: 6368 6f28 0a20 2020 2020 2020 2020 2020  cho(.           
+00018ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018ef0: 2066 2253 6f6e 6720 6669 6c65 2077 6974   f"Song file wit
+00018f00: 6820 4944 207b 736f 6e67 5f69 647d 206e  h ID {song_id} n
+00018f10: 6f74 2066 6f75 6e64 2e22 2c20 6667 3d22  ot found.", fg="
+00018f20: 7265 6422 0a20 2020 2020 2020 2020 2020  red".           
+00018f30: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+00018f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018f50: 2020 2020 2020 2073 6f6e 675f 6964 732e         song_ids.
+00018f60: 7265 6d6f 7665 2873 6f6e 675f 6964 290a  remove(song_id).
+00018f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018f80: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
+00018f90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018fa0: 2020 2020 2070 7269 6e74 5f65 6e74 7279       print_entry
+00018fb0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00018fc0: 2020 2020 2020 2020 2020 6465 7461 696c            detail
+00018fd0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+00018fe0: 2020 2020 2020 2020 2020 2b20 5b0a 2020            + [.  
+00018ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019000: 2020 2020 2020 2020 2020 7374 6174 735b            stats[
+00019010: 736f 6e67 5f69 645d 2c0a 2020 2020 2020  song_id],.      
+00019020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019030: 2020 2020 2020 6d75 7369 635f 7461 672e        music_tag.
+00019040: 6c6f 6164 5f66 696c 6528 0a20 2020 2020  load_file(.     
+00019050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019060: 2020 2020 2020 2020 2020 206f 732e 7061             os.pa
+00019070: 7468 2e6a 6f69 6e28 534f 4e47 535f 4449  th.join(SONGS_DI
+00019080: 522c 2064 6574 6169 6c73 5b31 5d29 0a20  R, details[1]). 
+00019090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000190a0: 2020 2020 2020 2020 2020 2029 5b22 236c             )["#l
+000190b0: 656e 6774 6822 5d2e 7661 6c75 652c 0a20  ength"].value,. 
+000190c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000190d0: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
+000190e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000190f0: 2020 7368 6f77 5f73 6f6e 675f 696e 666f    show_song_info
+00019100: 3d73 6f6e 675f 696e 666f 2c0a 2020 2020  =song_info,.    
+00019110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019120: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00019130: 2020 2020 2020 736f 6e67 5f69 6473 2e72        song_ids.r
+00019140: 656d 6f76 6528 736f 6e67 5f69 6429 0a20  emove(song_id). 
+00019150: 2020 2065 7863 6570 7420 4669 6c65 4e6f     except FileNo
+00019160: 7446 6f75 6e64 4572 726f 723a 0a20 2020  tFoundError:.   
+00019170: 2020 2020 2063 6c69 636b 2e73 6563 686f       click.secho
+00019180: 2866 224e 6f20 7374 6174 7320 666f 756e  (f"No stats foun
+00019190: 6420 666f 7220 7965 6172 207b 7965 6172  d for year {year
+000191a0: 7d2e 222c 2066 673d 2272 6564 2229 0a0a  }.", fg="red")..
+000191b0: 2020 2020 6966 2073 6f6e 675f 6964 733a      if song_ids:
+000191c0: 0a20 2020 2020 2020 2073 6f6e 675f 6964  .        song_id
+000191d0: 7320 3d20 5b73 7472 2869 645f 2920 666f  s = [str(id_) fo
+000191e0: 7220 6964 5f20 696e 2073 6f6e 675f 6964  r id_ in song_id
+000191f0: 735d 0a20 2020 2020 2020 2063 6c69 636b  s].        click
+00019200: 2e73 6563 686f 280a 2020 2020 2020 2020  .secho(.        
+00019210: 2020 2020 6622 4e6f 2073 6f6e 6773 2066      f"No songs f
+00019220: 6f75 6e64 2077 6974 6820 4944 733a 207b  ound with IDs: {
+00019230: 272c 2027 2e6a 6f69 6e28 736f 6e67 5f69  ', '.join(song_i
+00019240: 6473 297d 2e22 2c20 6667 3d22 7265 6422  ds)}.", fg="red"
+00019250: 0a20 2020 2020 2020 2029 0a0a 0a40 636c  .        )...@cl
+00019260: 692e 636f 6d6d 616e 6428 290a 4063 6c69  i.command().@cli
+00019270: 636b 2e61 7267 756d 656e 7428 2273 6f6e  ck.argument("son
+00019280: 6722 2c20 7265 7175 6972 6564 3d54 7275  g", required=Tru
+00019290: 6529 0a40 636c 6963 6b2e 6f70 7469 6f6e  e).@click.option
+000192a0: 280a 2020 2020 222d 4e2f 2d6e 4e22 2c0a  (.    "-N/-nN",.
+000192b0: 2020 2020 222d 2d6e 616d 652f 2d2d 6e6f      "--name/--no
+000192c0: 2d6e 616d 6522 2c0a 2020 2020 2274 6974  -name",.    "tit
+000192d0: 6c65 222c 0a20 2020 2064 6566 6175 6c74  le",.    default
+000192e0: 3d46 616c 7365 2c0a 2020 2020 6865 6c70  =False,.    help
+000192f0: 3d22 5472 6561 7420 534f 4e47 2061 7320  ="Treat SONG as 
+00019300: 6120 736f 6e67 206e 616d 6520 696e 7374  a song name inst
+00019310: 6561 6420 6f66 2061 6e20 4944 2e22 2c0a  ead of an ID.",.
+00019320: 290a 6465 6620 7265 636f 6d6d 656e 6428  ).def recommend(
+00019330: 736f 6e67 2c20 7469 746c 6529 3a0a 2020  song, title):.  
+00019340: 2020 2222 220a 2020 2020 4765 7420 7265    """.    Get re
+00019350: 636f 6d6d 656e 6461 7469 6f6e 7320 6672  commendations fr
+00019360: 6f6d 2059 5420 4d75 7369 6320 6261 7365  om YT Music base
+00019370: 6420 6f6e 2073 6f6e 6720 7469 746c 6573  d on song titles
+00019380: 2e20 4e6f 7465 3a20 7468 6973 2066 6561  . Note: this fea
+00019390: 7475 7265 0a20 2020 2069 7320 6578 7065  ture.    is expe
+000193a0: 7269 6d65 6e74 616c 2e0a 0a20 2020 2052  rimental...    R
+000193b0: 6563 6f6d 6d65 6e64 7320 736f 6e67 7320  ecommends songs 
+000193c0: 2870 6f73 7369 626c 7920 6578 706c 6963  (possibly explic
+000193d0: 6974 2920 7573 696e 6720 7468 6520 596f  it) using the Yo
+000193e0: 7554 7562 6520 4d75 7369 6320 4150 4920  uTube Music API 
+000193f0: 7369 6d69 6c61 720a 2020 2020 746f 2074  similar.    to t
+00019400: 6865 2073 6f6e 6720 7769 7468 2049 4420  he song with ID 
+00019410: 534f 4e47 2074 6f20 6c69 7374 656e 2074  SONG to listen t
+00019420: 6f2e 0a0a 2020 2020 4966 2074 6865 2027  o...    If the '
+00019430: 2d4e 2720 666c 6167 2069 7320 7061 7373  -N' flag is pass
+00019440: 6564 2c20 534f 4e47 2069 7320 7472 6561  ed, SONG is trea
+00019450: 7465 6420 6173 2061 2073 6f6e 6720 6e61  ted as a song na
+00019460: 6d65 2074 6f20 7365 6172 6368 2066 6f72  me to search for
+00019470: 0a20 2020 206f 6e20 596f 7554 7562 6520  .    on YouTube 
+00019480: 4d75 7369 632e 2222 220a 2020 2020 7472  Music.""".    tr
+00019490: 793a 0a20 2020 2020 2020 2066 726f 6d20  y:.        from 
+000194a0: 7974 6d75 7369 6361 7069 2069 6d70 6f72  ytmusicapi impor
+000194b0: 7420 5954 4d75 7369 630a 2020 2020 6578  t YTMusic.    ex
+000194c0: 6365 7074 2049 6d70 6f72 7445 7272 6f72  cept ImportError
+000194d0: 3a0a 2020 2020 2020 2020 636c 6963 6b2e  :.        click.
+000194e0: 7365 6368 6f28 0a20 2020 2020 2020 2020  secho(.         
+000194f0: 2020 2022 5468 6520 2772 6563 6f6d 6d65     "The 'recomme
+00019500: 6e64 2720 636f 6d6d 616e 6420 7265 7175  nd' command requ
+00019510: 6972 6573 2074 6865 2027 7974 6d75 7369  ires the 'ytmusi
+00019520: 6361 7069 2720 7061 636b 6167 6520 746f  capi' package to
+00019530: 2062 6520 696e 7374 616c 6c65 642e 2052   be installed. R
+00019540: 756e 2027 7069 7020 696e 7374 616c 6c20  un 'pip install 
+00019550: 7974 6d75 7369 6361 7069 2720 746f 2069  ytmusicapi' to i
+00019560: 6e73 7461 6c6c 2069 742e 222c 0a20 2020  nstall it.",.   
+00019570: 2020 2020 2020 2020 2066 673d 2272 6564           fg="red
+00019580: 222c 0a20 2020 2020 2020 2029 0a20 2020  ",.        ).   
+00019590: 2020 2020 2072 6574 7572 6e0a 0a20 2020       return..   
+000195a0: 2079 746d 7573 6963 203d 2059 544d 7573   ytmusic = YTMus
+000195b0: 6963 2829 0a0a 2020 2020 6966 2074 6974  ic()..    if tit
+000195c0: 6c65 3a0a 2020 2020 2020 2020 7265 7375  le:.        resu
+000195d0: 6c74 7320 3d20 7974 6d75 7369 632e 7365  lts = ytmusic.se
+000195e0: 6172 6368 2873 6f6e 672c 2066 696c 7465  arch(song, filte
+000195f0: 723d 2273 6f6e 6773 2229 0a20 2020 2065  r="songs").    e
+00019600: 6c73 653a 0a20 2020 2020 2020 2069 6620  lse:.        if 
+00019610: 6e6f 7420 736f 6e67 2e69 7364 6967 6974  not song.isdigit
+00019620: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00019630: 636c 6963 6b2e 7365 6368 6f28 0a20 2020  click.secho(.   
+00019640: 2020 2020 2020 2020 2020 2020 2022 536f               "So
+00019650: 6e67 2049 4420 6d75 7374 2062 6520 6120  ng ID must be a 
+00019660: 6e75 6d62 6572 2e20 546f 2067 6574 2072  number. To get r
+00019670: 6563 6f6d 6d65 6e64 6174 696f 6e73 2062  ecommendations b
+00019680: 7920 6e61 6d65 2c20 7061 7373 2074 6865  y name, pass the
+00019690: 2027 2d4e 2f2d 2d6e 616d 6527 2066 6c61   '-N/--name' fla
+000196a0: 672e 222c 0a20 2020 2020 2020 2020 2020  g.",.           
+000196b0: 2020 2020 2066 673d 2272 6564 222c 0a20       fg="red",. 
+000196c0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+000196d0: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+000196e0: 0a20 2020 2020 2020 2077 6974 6820 6f70  .        with op
+000196f0: 656e 2853 4f4e 4753 5f49 4e46 4f5f 5041  en(SONGS_INFO_PA
+00019700: 5448 2c20 2272 222c 2065 6e63 6f64 696e  TH, "r", encodin
+00019710: 673d 2275 7466 2d38 2229 2061 7320 736f  g="utf-8") as so
+00019720: 6e67 735f 6669 6c65 3a0a 2020 2020 2020  ngs_file:.      
+00019730: 2020 2020 2020 666f 7220 6c69 6e65 2069        for line i
+00019740: 6e20 736f 6e67 735f 6669 6c65 3a0a 2020  n songs_file:.  
+00019750: 2020 2020 2020 2020 2020 2020 2020 6465                de
+00019760: 7461 696c 7320 3d20 6c69 6e65 2e73 7472  tails = line.str
+00019770: 6970 2829 2e73 706c 6974 2822 7c22 290a  ip().split("|").
+00019780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019790: 6966 2064 6574 6169 6c73 5b30 5d20 3d3d  if details[0] ==
+000197a0: 2073 6f6e 673a 0a20 2020 2020 2020 2020   song:.         
+000197b0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+000197c0: 7473 203d 2079 746d 7573 6963 2e73 6561  ts = ytmusic.sea
+000197d0: 7263 6828 0a20 2020 2020 2020 2020 2020  rch(.           
+000197e0: 2020 2020 2020 2020 2020 2020 206f 732e               os.
+000197f0: 7061 7468 2e73 706c 6974 6578 7428 6465  path.splitext(de
+00019800: 7461 696c 735b 315d 295b 305d 2c20 6669  tails[1])[0], fi
+00019810: 6c74 6572 3d22 736f 6e67 7322 0a20 2020  lter="songs".   
+00019820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019830: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+00019840: 2020 2020 2020 2062 7265 616b 0a20 2020         break.   
+00019850: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+00019860: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00019870: 6c69 636b 2e73 6563 686f 2866 224e 6f20  lick.secho(f"No 
+00019880: 736f 6e67 2066 6f75 6e64 2077 6974 6820  song found with 
+00019890: 4944 207b 736f 6e67 7d2e 222c 2066 673d  ID {song}.", fg=
+000198a0: 2272 6564 2229 0a20 2020 2020 2020 2020  "red").         
+000198b0: 2020 2020 2020 2072 6574 7572 6e0a 0a20         return.. 
+000198c0: 2020 2079 745f 6d75 7369 635f 706c 6179     yt_music_play
+000198d0: 6c69 7374 203d 2079 746d 7573 6963 2e67  list = ytmusic.g
+000198e0: 6574 5f77 6174 6368 5f70 6c61 796c 6973  et_watch_playlis
+000198f0: 7428 7265 7375 6c74 735b 305d 5b22 7669  t(results[0]["vi
+00019900: 6465 6f49 6422 5d29 0a0a 2020 2020 636c  deoId"])..    cl
+00019910: 6963 6b2e 6563 686f 2822 5265 636f 6d6d  ick.echo("Recomm
+00019920: 656e 6461 7469 6f6e 7320 666f 7220 222c  endations for ",
+00019930: 206e 6c3d 4661 6c73 6529 0a20 2020 2063   nl=False).    c
+00019940: 6c69 636b 2e73 6563 686f 280a 2020 2020  lick.secho(.    
+00019950: 2020 2020 7974 5f6d 7573 6963 5f70 6c61      yt_music_pla
+00019960: 796c 6973 745b 2274 7261 636b 7322 5d5b  ylist["tracks"][
+00019970: 305d 5b22 7469 746c 6522 5d20 2b20 2220  0]["title"] + " 
+00019980: 222c 0a20 2020 2020 2020 2066 673d 2262  ",.        fg="b
+00019990: 6c75 6522 2c0a 2020 2020 2020 2020 6e6c  lue",.        nl
+000199a0: 3d46 616c 7365 2c0a 2020 2020 290a 2020  =False,.    ).  
+000199b0: 2020 636c 6963 6b2e 7365 6368 6f28 0a20    click.secho(. 
+000199c0: 2020 2020 2020 2066 2228 6874 7470 733a         f"(https:
+000199d0: 2f2f 6d75 7369 632e 796f 7574 7562 652e  //music.youtube.
+000199e0: 636f 6d2f 7761 7463 683f 763d 7b79 745f  com/watch?v={yt_
+000199f0: 6d75 7369 635f 706c 6179 6c69 7374 5b27  music_playlist['
+00019a00: 7472 6163 6b73 275d 5b30 5d5b 2776 6964  tracks'][0]['vid
+00019a10: 656f 4964 275d 7d29 222c 0a20 2020 2020  eoId']})",.     
+00019a20: 2020 2066 673d 2262 7269 6768 745f 626c     fg="bright_bl
+00019a30: 6163 6b22 2c0a 2020 2020 2020 2020 6e6c  ack",.        nl
+00019a40: 3d46 616c 7365 2c0a 2020 2020 290a 2020  =False,.    ).  
+00019a50: 2020 636c 6963 6b2e 6563 686f 2822 3a22    click.echo(":"
+00019a60: 290a 2020 2020 666f 7220 7472 6163 6b20  ).    for track 
+00019a70: 696e 2079 745f 6d75 7369 635f 706c 6179  in yt_music_play
+00019a80: 6c69 7374 5b22 7472 6163 6b73 225d 5b31  list["tracks"][1
+00019a90: 3a5d 3a0a 2020 2020 2020 2020 636c 6963  :]:.        clic
+00019aa0: 6b2e 7365 6368 6f28 7472 6163 6b5b 2274  k.secho(track["t
+00019ab0: 6974 6c65 225d 202b 2022 2022 2c20 6667  itle"] + " ", fg
+00019ac0: 3d22 626c 7565 222c 2062 6f6c 643d 5472  ="blue", bold=Tr
+00019ad0: 7565 2c20 6e6c 3d46 616c 7365 290a 2020  ue, nl=False).  
+00019ae0: 2020 2020 2020 636c 6963 6b2e 7365 6368        click.sech
+00019af0: 6f28 0a20 2020 2020 2020 2020 2020 2066  o(.            f
+00019b00: 2268 7474 7073 3a2f 2f6d 7573 6963 2e79  "https://music.y
+00019b10: 6f75 7475 6265 2e63 6f6d 2f77 6174 6368  outube.com/watch
+00019b20: 3f76 3d7b 7472 6163 6b5b 2776 6964 656f  ?v={track['video
+00019b30: 4964 275d 7d22 2c0a 2020 2020 2020 2020  Id']}",.        
+00019b40: 2020 2020 6667 3d22 6272 6967 6874 5f62      fg="bright_b
+00019b50: 6c61 636b 222c 0a20 2020 2020 2020 2029  lack",.        )
+00019b60: 0a0a 0a40 636c 692e 636f 6d6d 616e 6428  ...@cli.command(
+00019b70: 290a 4063 6c69 636b 2e61 7267 756d 656e  ).@click.argumen
+00019b80: 7428 2273 6f6e 675f 6964 7322 2c20 7265  t("song_ids", re
+00019b90: 7175 6972 6564 3d54 7275 652c 2074 7970  quired=True, typ
+00019ba0: 653d 696e 742c 206e 6172 6773 3d2d 3129  e=int, nargs=-1)
+00019bb0: 0a40 636c 6963 6b2e 6f70 7469 6f6e 2822  .@click.option("
+00019bc0: 2d42 2f2d 6e42 222c 2022 2d2d 626f 7474  -B/-nB", "--bott
+00019bd0: 6f6d 2f2d 2d6e 6f2d 626f 7474 6f6d 222c  om/--no-bottom",
+00019be0: 2022 626f 7474 6f6d 222c 2064 6566 6175   "bottom", defau
+00019bf0: 6c74 3d46 616c 7365 290a 6465 6620 7075  lt=False).def pu
+00019c00: 7368 2873 6f6e 675f 6964 732c 2062 6f74  sh(song_ids, bot
+00019c10: 746f 6d29 3a0a 2020 2020 2222 220a 2020  tom):.    """.  
+00019c20: 2020 4d6f 7665 2073 6f6e 6773 2061 726f    Move songs aro
+00019c30: 756e 6420 746f 2074 6865 2062 6f74 746f  und to the botto
+00019c40: 6d20 6f72 2074 6f70 206f 6620 7468 6520  m or top of the 
+00019c50: 6461 7461 6261 7365 2e0a 0a20 2020 2050  database...    P
+00019c60: 7573 6820 7468 6520 736f 6e67 2873 2920  ush the song(s) 
+00019c70: 7769 7468 2049 4428 7329 2053 4f4e 475f  with ID(s) SONG_
+00019c80: 4944 5320 746f 2074 6865 2074 6f70 206f  IDS to the top o
+00019c90: 6620 7468 6520 6461 7461 6261 7365 2028  f the database (
+00019ca0: 6173 2069 6620 7468 6579 0a20 2020 2077  as if they.    w
+00019cb0: 6572 6520 7468 6520 736f 6e67 7320 6d6f  ere the songs mo
+00019cc0: 7374 2072 6563 656e 746c 7920 6164 6465  st recently adde
+00019cd0: 6429 2069 6e20 7468 6520 6f72 6465 7220  d) in the order 
+00019ce0: 7468 6579 2061 7265 2070 6173 7365 6420  they are passed 
+00019cf0: 2865 2e67 2e0a 2020 2020 276d 6165 7374  (e.g..    'maest
+00019d00: 726f 2070 7573 6820 3120 3220 3327 2077  ro push 1 2 3' w
+00019d10: 696c 6c20 6d61 6b65 2074 6865 206d 6f73  ill make the mos
+00019d20: 7420 7265 6365 6e74 2073 6f6e 6720 6265  t recent song be
+00019d30: 2033 292e 0a0a 2020 2020 4966 2074 6865   3)...    If the
+00019d40: 2027 2d42 2720 666c 6167 2069 7320 7061   '-B' flag is pa
+00019d50: 7373 6564 2c20 7468 6520 736f 6e67 2873  ssed, the song(s
+00019d60: 2920 7769 6c6c 2062 6520 7075 7368 6564  ) will be pushed
+00019d70: 2074 6f20 7468 6520 626f 7474 6f6d 206f   to the bottom o
+00019d80: 6620 7468 650a 2020 2020 6c69 7374 2069  f the.    list i
+00019d90: 6e73 7465 6164 2e0a 2020 2020 2222 220a  nstead..    """.
+00019da0: 2020 2020 7769 7468 206f 7065 6e28 534f      with open(SO
+00019db0: 4e47 535f 494e 464f 5f50 4154 482c 2022  NGS_INFO_PATH, "
+00019dc0: 722b 222c 2065 6e63 6f64 696e 673d 2275  r+", encoding="u
+00019dd0: 7466 2d38 2229 2061 7320 736f 6e67 735f  tf-8") as songs_
+00019de0: 6669 6c65 3a0a 2020 2020 2020 2020 6c69  file:.        li
+00019df0: 6e65 7320 3d20 736f 6e67 735f 6669 6c65  nes = songs_file
+00019e00: 2e72 6561 646c 696e 6573 2829 0a0a 2020  .readlines()..  
+00019e10: 2020 2020 2020 6c69 6e65 735f 746f 5f6d        lines_to_m
+00019e20: 6f76 6520 3d20 5b5d 0a20 2020 2020 2020  ove = [].       
+00019e30: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+00019e40: 6c65 6e28 6c69 6e65 7329 293a 0a20 2020  len(lines)):.   
+00019e50: 2020 2020 2020 2020 2069 6620 696e 7428           if int(
+00019e60: 6c69 6e65 735b 695d 2e73 706c 6974 2822  lines[i].split("
+00019e70: 7c22 295b 305d 2920 696e 2073 6f6e 675f  |")[0]) in song_
+00019e80: 6964 733a 0a20 2020 2020 2020 2020 2020  ids:.           
+00019e90: 2020 2020 206c 696e 6573 5f74 6f5f 6d6f       lines_to_mo
+00019ea0: 7665 2e61 7070 656e 6428 2869 2c20 6c69  ve.append((i, li
+00019eb0: 6e65 735b 695d 2929 0a0a 2020 2020 2020  nes[i]))..      
+00019ec0: 2020 666f 7220 692c 205f 2069 6e20 7265    for i, _ in re
+00019ed0: 7665 7273 6564 286c 696e 6573 5f74 6f5f  versed(lines_to_
+00019ee0: 6d6f 7665 293a 0a20 2020 2020 2020 2020  move):.         
+00019ef0: 2020 206c 696e 6573 2e70 6f70 2869 290a     lines.pop(i).
+00019f00: 0a20 2020 2020 2020 2073 6f6e 675f 6964  .        song_id
+00019f10: 735f 7769 7468 5f6f 7264 6572 203d 2064  s_with_order = d
+00019f20: 6963 7428 0a20 2020 2020 2020 2020 2020  ict(.           
+00019f30: 206d 6170 286c 616d 6264 6120 783a 2028   map(lambda x: (
+00019f40: 785b 315d 2c20 785b 305d 292c 2065 6e75  x[1], x[0]), enu
+00019f50: 6d65 7261 7465 2873 6f6e 675f 6964 7329  merate(song_ids)
+00019f60: 290a 2020 2020 2020 2020 290a 0a20 2020  ).        )..   
+00019f70: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
+00019f80: 6e67 6528 6c65 6e28 6c69 6e65 735f 746f  nge(len(lines_to
+00019f90: 5f6d 6f76 6529 293a 0a20 2020 2020 2020  _move)):.       
+00019fa0: 2020 2020 206c 696e 6573 5f74 6f5f 6d6f       lines_to_mo
+00019fb0: 7665 5b69 5d20 3d20 280a 2020 2020 2020  ve[i] = (.      
+00019fc0: 2020 2020 2020 2020 2020 736f 6e67 5f69            song_i
+00019fd0: 6473 5f77 6974 685f 6f72 6465 725b 696e  ds_with_order[in
+00019fe0: 7428 6c69 6e65 735f 746f 5f6d 6f76 655b  t(lines_to_move[
+00019ff0: 695d 5b31 5d2e 7370 6c69 7428 227c 2229  i][1].split("|")
+0001a000: 5b30 5d29 5d2c 0a20 2020 2020 2020 2020  [0])],.         
+0001a010: 2020 2020 2020 202a 6c69 6e65 735f 746f         *lines_to
+0001a020: 5f6d 6f76 655b 695d 2c0a 2020 2020 2020  _move[i],.      
+0001a030: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+0001a040: 206c 696e 6573 5f74 6f5f 6d6f 7665 2e73   lines_to_move.s
+0001a050: 6f72 7428 6b65 793d 6c61 6d62 6461 2078  ort(key=lambda x
+0001a060: 3a20 785b 305d 2c20 7265 7665 7273 653d  : x[0], reverse=
+0001a070: 626f 7474 6f6d 290a 0a20 2020 2020 2020  bottom)..       
+0001a080: 2069 6620 6e6f 7420 626f 7474 6f6d 3a0a   if not bottom:.
+0001a090: 2020 2020 2020 2020 2020 2020 6c69 6e65              line
+0001a0a0: 7320 2b3d 205b 745b 325d 2066 6f72 2074  s += [t[2] for t
+0001a0b0: 2069 6e20 6c69 6e65 735f 746f 5f6d 6f76   in lines_to_mov
+0001a0c0: 655d 0a20 2020 2020 2020 2065 6c73 653a  e].        else:
+0001a0d0: 0a20 2020 2020 2020 2020 2020 206c 696e  .            lin
+0001a0e0: 6573 203d 205b 745b 325d 2066 6f72 2074  es = [t[2] for t
+0001a0f0: 2069 6e20 6c69 6e65 735f 746f 5f6d 6f76   in lines_to_mov
+0001a100: 655d 202b 206c 696e 6573 0a0a 2020 2020  e] + lines..    
+0001a110: 2020 2020 736f 6e67 735f 6669 6c65 2e73      songs_file.s
+0001a120: 6565 6b28 3029 0a20 2020 2020 2020 2073  eek(0).        s
+0001a130: 6f6e 6773 5f66 696c 652e 7772 6974 6528  ongs_file.write(
+0001a140: 2222 2e6a 6f69 6e28 6c69 6e65 7329 290a  "".join(lines)).
+0001a150: 2020 2020 2020 2020 736f 6e67 735f 6669          songs_fi
+0001a160: 6c65 2e74 7275 6e63 6174 6528 290a 0a0a  le.truncate()...
+0001a170: 4063 6c69 2e63 6f6d 6d61 6e64 286e 616d  @cli.command(nam
+0001a180: 653d 2263 6c69 7022 290a 4063 6c69 636b  e="clip").@click
+0001a190: 2e61 7267 756d 656e 7428 2273 6f6e 675f  .argument("song_
+0001a1a0: 6964 222c 2072 6571 7569 7265 643d 5472  id", required=Tr
+0001a1b0: 7565 2c20 7479 7065 3d69 6e74 290a 4063  ue, type=int).@c
+0001a1c0: 6c69 636b 2e61 7267 756d 656e 7428 2273  lick.argument("s
+0001a1d0: 7461 7274 222c 2072 6571 7569 7265 643d  tart", required=
+0001a1e0: 4661 6c73 652c 2074 7970 653d 666c 6f61  False, type=floa
+0001a1f0: 742c 2064 6566 6175 6c74 3d4e 6f6e 6529  t, default=None)
+0001a200: 0a40 636c 6963 6b2e 6172 6775 6d65 6e74  .@click.argument
+0001a210: 2822 656e 6422 2c20 7265 7175 6972 6564  ("end", required
+0001a220: 3d46 616c 7365 2c20 7479 7065 3d66 6c6f  =False, type=flo
+0001a230: 6174 2c20 6465 6661 756c 743d 4e6f 6e65  at, default=None
+0001a240: 290a 6465 6620 636c 6970 5f28 736f 6e67  ).def clip_(song
+0001a250: 5f69 642c 2073 7461 7274 2c20 656e 6429  _id, start, end)
+0001a260: 3a0a 2020 2020 2222 220a 2020 2020 4372  :.    """.    Cr
+0001a270: 6561 7465 206f 7220 6564 6974 2074 6865  eate or edit the
+0001a280: 2063 6c69 7020 666f 7220 6120 736f 6e67   clip for a song
+0001a290: 2e0a 0a20 2020 2053 6574 7320 7468 6520  ...    Sets the 
+0001a2a0: 636c 6970 2066 6f72 2074 6865 2073 6f6e  clip for the son
+0001a2b0: 6720 7769 7468 2049 4420 534f 4e47 5f49  g with ID SONG_I
+0001a2c0: 4420 746f 2074 6865 2074 696d 6520 7261  D to the time ra
+0001a2d0: 6e67 6520 5354 4152 5420 746f 2045 4e44  nge START to END
+0001a2e0: 0a20 2020 2028 696e 2073 6563 6f6e 6473  .    (in seconds
+0001a2f0: 292e 0a0a 2020 2020 4966 2045 4e44 2069  )...    If END i
+0001a300: 7320 6e6f 7420 7061 7373 6564 2c20 7468  s not passed, th
+0001a310: 6520 636c 6970 2077 696c 6c20 6265 2066  e clip will be f
+0001a320: 726f 6d20 5354 4152 5420 746f 2074 6865  rom START to the
+0001a330: 2065 6e64 206f 6620 7468 6520 736f 6e67   end of the song
+0001a340: 2e0a 0a20 2020 2049 6620 6e65 6974 6865  ...    If neithe
+0001a350: 7220 5354 4152 5420 6e6f 7220 454e 4420  r START nor END 
+0001a360: 6172 6520 7061 7373 6564 2c20 6120 636c  are passed, a cl
+0001a370: 6970 2065 6469 746f 7220 7769 6c6c 2062  ip editor will b
+0001a380: 6520 6f70 656e 6564 2c20 696e 2077 6869  e opened, in whi
+0001a390: 6368 0a20 2020 2079 6f75 2063 616e 206d  ch.    you can m
+0001a3a0: 6f76 6520 7468 6520 7374 6172 7420 616e  ove the start an
+0001a3b0: 6420 656e 6420 6f66 2074 6865 2063 6c69  d end of the cli
+0001a3c0: 7020 6172 6f75 6e64 2075 7369 6e67 2074  p around using t
+0001a3d0: 6865 2061 7272 6f77 206b 6579 7320 7768  he arrow keys wh
+0001a3e0: 696c 650a 2020 2020 6c69 7374 656e 696e  ile.    listenin
+0001a3f0: 6720 746f 2074 6865 2073 6f6e 6720 2861  g to the song (a
+0001a400: 6c73 6f20 7368 6f77 7320 7761 7665 666f  lso shows wavefo
+0001a410: 726d 292e 0a0a 2020 2020 5c62 0a20 2020  rm)...    \b.   
+0001a420: 2054 6865 2065 6469 746f 7220 7374 6172   The editor star
+0001a430: 7473 206f 7574 2065 6469 7469 6e67 2074  ts out editing t
+0001a440: 6865 2073 7461 7274 206f 6620 7468 6520  he start of the 
+0001a450: 636c 6970 2e0a 2020 2020 5c78 3162 5b31  clip..    \x1b[1
+0001a460: 6d74 5c78 3162 5b30 6d20 746f 2074 6f67  mt\x1b[0m to tog
+0001a470: 676c 6520 6265 7477 6565 6e20 6564 6974  gle between edit
+0001a480: 696e 6720 7468 6520 7374 6172 7420 616e  ing the start an
+0001a490: 6420 656e 6420 6f66 2074 6865 2063 6c69  d end of the cli
+0001a4a0: 702e 0a20 2020 205c 7831 625b 316d 5348  p..    \x1b[1mSH
+0001a4b0: 4946 542b 4c45 4654 2f52 4947 4854 5c78  IFT+LEFT/RIGHT\x
+0001a4c0: 3162 5b30 6d20 7769 6c6c 206d 6f76 6520  1b[0m will move 
+0001a4d0: 7768 6963 6865 7665 7220 636c 6970 2065  whichever clip e
+0001a4e0: 6e64 2079 6f75 2061 7265 2065 6469 7469  nd you are editi
+0001a4f0: 6e67 0a20 2020 2020 2020 2062 7920 302e  ng.        by 0.
+0001a500: 3120 7365 636f 6e64 732c 2073 6e61 7020  1 seconds, snap 
+0001a510: 7468 6520 6375 7272 656e 7420 706c 6179  the current play
+0001a520: 6261 636b 2074 6f20 7468 6174 2063 6c69  back to that cli
+0001a530: 7020 656e 6420 2874 6f20 6578 6163 746c  p end (to exactl
+0001a540: 790a 2020 2020 2020 2020 7468 6520 636c  y.        the cl
+0001a550: 6970 2073 7461 7274 2069 6620 6564 6974  ip start if edit
+0001a560: 696e 6720 7374 6172 742c 2065 6e64 2d31  ing start, end-1
+0001a570: 2069 6620 6564 6974 696e 6720 656e 6429   if editing end)
+0001a580: 2c20 616e 6420 7061 7573 652e 0a20 2020  , and pause..   
+0001a590: 205c 7831 625b 316d 4c45 4654 2f52 4947   \x1b[1mLEFT/RIG
+0001a5a0: 4854 5c78 3162 5b30 6d20 7769 6c6c 206d  HT\x1b[0m will m
+0001a5b0: 6f76 6520 7768 6963 6865 7665 7220 636c  ove whichever cl
+0001a5c0: 6970 2065 6e64 2079 6f75 2061 7265 2065  ip end you are e
+0001a5d0: 6469 7469 6e67 2062 7920 310a 2020 2020  diting by 1.    
+0001a5e0: 2020 2020 7365 636f 6e64 2c20 736e 6170      second, snap
+0001a5f0: 2074 6865 2063 7572 7265 6e74 2070 6c61   the current pla
+0001a600: 7962 6163 6b20 746f 2074 6861 7420 636c  yback to that cl
+0001a610: 6970 2065 6e64 2c20 616e 6420 7061 7573  ip end, and paus
+0001a620: 652e 0a20 2020 205c 7831 625b 316d 454e  e..    \x1b[1mEN
+0001a630: 5445 525c 7831 625b 306d 2077 696c 6c20  TER\x1b[0m will 
+0001a640: 6578 6974 2074 6865 2065 6469 746f 7220  exit the editor 
+0001a650: 616e 6420 7361 7665 2074 6865 2063 6c69  and save the cli
+0001a660: 702e 0a20 2020 205c 7831 625b 316d 715c  p..    \x1b[1mq\
+0001a670: 7831 625b 306d 2077 696c 6c20 6578 6974  x1b[0m will exit
+0001a680: 2074 6865 2065 6469 746f 7220 7769 7468   the editor with
+0001a690: 6f75 7420 7361 7669 6e67 2074 6865 2063  out saving the c
+0001a6a0: 6c69 702e 0a20 2020 2022 2222 0a20 2020  lip..    """.   
+0001a6b0: 2069 6620 7374 6172 7420 6973 206e 6f74   if start is not
+0001a6c0: 204e 6f6e 653a 0a20 2020 2020 2020 2069   None:.        i
+0001a6d0: 6620 7374 6172 7420 3c20 303a 0a20 2020  f start < 0:.   
+0001a6e0: 2020 2020 2020 2020 2063 6c69 636b 2e73           click.s
+0001a6f0: 6563 686f 2822 5354 4152 5420 6d75 7374  echo("START must
+0001a700: 2062 6520 6120 706f 7369 7469 7665 206e   be a positive n
+0001a710: 756d 6265 722e 222c 2066 673d 2272 6564  umber.", fg="red
+0001a720: 2229 0a20 2020 2020 2020 2020 2020 2072  ").            r
+0001a730: 6574 7572 6e0a 2020 2020 2020 2020 6966  eturn.        if
+0001a740: 2065 6e64 2069 7320 6e6f 7420 4e6f 6e65   end is not None
+0001a750: 2061 6e64 2065 6e64 203c 2030 3a0a 2020   and end < 0:.  
+0001a760: 2020 2020 2020 2020 2020 636c 6963 6b2e            click.
+0001a770: 7365 6368 6f28 2245 4e44 206d 7573 7420  secho("END must 
+0001a780: 6265 2061 2070 6f73 6974 6976 6520 6e75  be a positive nu
+0001a790: 6d62 6572 2e22 2c20 6667 3d22 7265 6422  mber.", fg="red"
+0001a7a0: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+0001a7b0: 7475 726e 0a0a 2020 2020 7769 7468 206f  turn..    with o
+0001a7c0: 7065 6e28 534f 4e47 535f 494e 464f 5f50  pen(SONGS_INFO_P
+0001a7d0: 4154 482c 2022 722b 222c 2065 6e63 6f64  ATH, "r+", encod
+0001a7e0: 696e 673d 2275 7466 2d38 2229 2061 7320  ing="utf-8") as 
+0001a7f0: 736f 6e67 735f 6669 6c65 3a0a 2020 2020  songs_file:.    
+0001a800: 2020 2020 6c69 6e65 7320 3d20 736f 6e67      lines = song
+0001a810: 735f 6669 6c65 2e72 6561 646c 696e 6573  s_file.readlines
+0001a820: 2829 0a0a 2020 2020 2020 2020 666f 7220  ()..        for 
+0001a830: 6920 696e 2072 616e 6765 286c 656e 286c  i in range(len(l
+0001a840: 696e 6573 2929 3a0a 2020 2020 2020 2020  ines)):.        
+0001a850: 2020 2020 6465 7461 696c 7320 3d20 6c69      details = li
+0001a860: 6e65 735b 695d 2e73 7472 6970 2829 2e73  nes[i].strip().s
+0001a870: 706c 6974 2822 7c22 290a 2020 2020 2020  plit("|").      
+0001a880: 2020 2020 2020 6966 2069 6e74 2864 6574        if int(det
+0001a890: 6169 6c73 5b30 5d29 203d 3d20 736f 6e67  ails[0]) == song
+0001a8a0: 5f69 643a 0a20 2020 2020 2020 2020 2020  _id:.           
+0001a8b0: 2020 2020 2062 7265 616b 0a20 2020 2020       break.     
+0001a8c0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0001a8d0: 2020 2020 2063 6c69 636b 2e73 6563 686f       click.secho
+0001a8e0: 2866 224e 6f20 736f 6e67 2066 6f75 6e64  (f"No song found
+0001a8f0: 2077 6974 6820 4944 207b 736f 6e67 5f69   with ID {song_i
+0001a900: 647d 2e22 2c20 6667 3d22 7265 6422 290a  d}.", fg="red").
+0001a910: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0001a920: 726e 0a0a 2020 2020 2020 2020 736f 6e67  rn..        song
+0001a930: 5f6e 616d 6520 3d20 6465 7461 696c 735b  _name = details[
+0001a940: 315d 0a20 2020 2020 2020 2069 6620 6e6f  1].        if no
+0001a950: 7420 6f73 2e70 6174 682e 6578 6973 7473  t os.path.exists
+0001a960: 286f 732e 7061 7468 2e6a 6f69 6e28 534f  (os.path.join(SO
+0001a970: 4e47 535f 4449 522c 2073 6f6e 675f 6e61  NGS_DIR, song_na
+0001a980: 6d65 2929 3a0a 2020 2020 2020 2020 2020  me)):.          
+0001a990: 2020 636c 6963 6b2e 7365 6368 6f28 0a20    click.secho(. 
+0001a9a0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0001a9b0: 2253 6f6e 6720 6669 6c65 207b 736f 6e67  "Song file {song
+0001a9c0: 5f6e 616d 657d 2028 4944 207b 736f 6e67  _name} (ID {song
+0001a9d0: 5f69 647d 2920 6e6f 7420 666f 756e 642e  _id}) not found.
+0001a9e0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+0001a9f0: 2020 2066 673d 2272 6564 222c 0a20 2020     fg="red",.   
+0001aa00: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0001aa10: 2020 2020 2020 2072 6574 7572 6e0a 0a20         return.. 
+0001aa20: 2020 2020 2020 2069 6620 7374 6172 7420         if start 
+0001aa30: 6973 204e 6f6e 653a 2020 2320 636c 6970  is None:  # clip
+0001aa40: 2065 6469 746f 720a 2020 2020 2020 2020   editor.        
+0001aa50: 2020 2020 7374 6172 742c 2065 6e64 203d      start, end =
+0001aa60: 2063 7572 7365 732e 7772 6170 7065 7228   curses.wrapper(
+0001aa70: 636c 6970 5f65 6469 746f 722c 2064 6574  clip_editor, det
+0001aa80: 6169 6c73 290a 2020 2020 2020 2020 2020  ails).          
+0001aa90: 2020 6966 2073 7461 7274 2069 7320 4e6f    if start is No
+0001aaa0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0001aab0: 2020 2020 636c 6963 6b2e 7365 6368 6f28      click.secho(
+0001aac0: 6622 4e6f 2063 6861 6e67 6520 696e 2063  f"No change in c
+0001aad0: 6c69 7020 666f 7220 7b73 6f6e 675f 6e61  lip for {song_na
+0001aae0: 6d65 7d2e 222c 2066 673d 2267 7265 656e  me}.", fg="green
+0001aaf0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+0001ab00: 2020 2072 6574 7572 6e0a 0a20 2020 2020     return..     
+0001ab10: 2020 2073 6f6e 675f 7061 7468 203d 206f     song_path = o
+0001ab20: 732e 7061 7468 2e6a 6f69 6e28 534f 4e47  s.path.join(SONG
+0001ab30: 535f 4449 522c 2073 6f6e 675f 6e61 6d65  S_DIR, song_name
+0001ab40: 290a 2020 2020 2020 2020 6475 7261 7469  ).        durati
+0001ab50: 6f6e 203d 206d 7573 6963 5f74 6167 2e6c  on = music_tag.l
+0001ab60: 6f61 645f 6669 6c65 2873 6f6e 675f 7061  oad_file(song_pa
+0001ab70: 7468 295b 2223 6c65 6e67 7468 225d 2e76  th)["#length"].v
+0001ab80: 616c 7565 0a0a 2020 2020 2020 2020 6966  alue..        if
+0001ab90: 2065 6e64 2069 7320 4e6f 6e65 3a0a 2020   end is None:.  
+0001aba0: 2020 2020 2020 2020 2020 656e 6420 3d20            end = 
+0001abb0: 6475 7261 7469 6f6e 0a0a 2020 2020 2020  duration..      
+0001abc0: 2020 6966 2073 7461 7274 203e 2064 7572    if start > dur
+0001abd0: 6174 696f 6e3a 0a20 2020 2020 2020 2020  ation:.         
+0001abe0: 2020 2063 6c69 636b 2e73 6563 686f 280a     click.secho(.
+0001abf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ac00: 2253 5441 5254 206d 7573 7420 6e6f 7420  "START must not 
+0001ac10: 6265 206d 6f72 6520 7468 616e 2074 6865  be more than the
+0001ac20: 2073 6f6e 6720 6475 7261 7469 6f6e 2e22   song duration."
+0001ac30: 2c20 6667 3d22 7265 6422 0a20 2020 2020  , fg="red".     
+0001ac40: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0001ac50: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+0001ac60: 2020 2020 6966 2065 6e64 203e 2064 7572      if end > dur
+0001ac70: 6174 696f 6e3a 0a20 2020 2020 2020 2020  ation:.         
+0001ac80: 2020 2063 6c69 636b 2e73 6563 686f 280a     click.secho(.
+0001ac90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aca0: 2245 4e44 206d 7573 7420 6e6f 7420 6265  "END must not be
+0001acb0: 206d 6f72 6520 7468 616e 2074 6865 2073   more than the s
+0001acc0: 6f6e 6720 6475 7261 7469 6f6e 2e22 2c20  ong duration.", 
+0001acd0: 6667 3d22 7265 6422 0a20 2020 2020 2020  fg="red".       
+0001ace0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+0001acf0: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
+0001ad00: 2020 6966 2073 7461 7274 203e 2065 6e64    if start > end
+0001ad10: 3a0a 2020 2020 2020 2020 2020 2020 636c  :.            cl
+0001ad20: 6963 6b2e 7365 6368 6f28 2253 5441 5254  ick.secho("START
+0001ad30: 206d 7573 7420 6e6f 7420 6265 206d 6f72   must not be mor
+0001ad40: 6520 7468 616e 2045 4e44 2e22 2c20 6667  e than END.", fg
+0001ad50: 3d22 7265 6422 290a 2020 2020 2020 2020  ="red").        
+0001ad60: 2020 2020 7265 7475 726e 0a0a 2020 2020      return..    
+0001ad70: 2020 2020 6c69 6e65 735b 695d 203d 2028      lines[i] = (
+0001ad80: 0a20 2020 2020 2020 2020 2020 2022 7c22  .            "|"
+0001ad90: 2e6a 6f69 6e28 6465 7461 696c 735b 3a33  .join(details[:3
+0001ada0: 5d20 2b20 5b73 7472 2873 7461 7274 2920  ] + [str(start) 
+0001adb0: 2b20 2220 2220 2b20 7374 7228 656e 6429  + " " + str(end)
+0001adc0: 5d20 2b20 6465 7461 696c 735b 353a 5d29  ] + details[5:])
+0001add0: 0a20 2020 2020 2020 2020 2020 202b 2022  .            + "
+0001ade0: 5c6e 220a 2020 2020 2020 2020 290a 0a20  \n".        ).. 
+0001adf0: 2020 2020 2020 2073 6f6e 6773 5f66 696c         songs_fil
+0001ae00: 652e 7365 656b 2830 290a 2020 2020 2020  e.seek(0).      
+0001ae10: 2020 736f 6e67 735f 6669 6c65 2e77 7269    songs_file.wri
+0001ae20: 7465 2822 222e 6a6f 696e 286c 696e 6573  te("".join(lines
+0001ae30: 2929 0a20 2020 2020 2020 2073 6f6e 6773  )).        songs
+0001ae40: 5f66 696c 652e 7472 756e 6361 7465 2829  _file.truncate()
+0001ae50: 0a0a 2020 2020 2020 2020 636c 6963 6b2e  ..        click.
+0001ae60: 7365 6368 6f28 6622 436c 6970 7065 6420  secho(f"Clipped 
+0001ae70: 7b73 6f6e 675f 6e61 6d65 7d20 6672 6f6d  {song_name} from
+0001ae80: 207b 7374 6172 747d 2074 6f20 7b65 6e64   {start} to {end
+0001ae90: 7d2e 222c 2066 673d 2267 7265 656e 2229  }.", fg="green")
+0001aea0: 0a0a 0a40 636c 692e 636f 6d6d 616e 6428  ...@cli.command(
+0001aeb0: 290a 4063 6c69 636b 2e61 7267 756d 656e  ).@click.argumen
+0001aec0: 7428 2273 6f6e 675f 6964 7322 2c20 7479  t("song_ids", ty
+0001aed0: 7065 3d69 6e74 2c20 6e61 7267 733d 2d31  pe=int, nargs=-1
+0001aee0: 2c20 7265 7175 6972 6564 3d46 616c 7365  , required=False
+0001aef0: 290a 4063 6c69 636b 2e6f 7074 696f 6e28  ).@click.option(
+0001af00: 0a20 2020 2022 2d41 2f2d 6e41 222c 0a20  .    "-A/-nA",. 
+0001af10: 2020 2022 2d2d 616c 6c2f 2d2d 6e6f 2d61     "--all/--no-a
+0001af20: 6c6c 222c 0a20 2020 2022 616c 6c5f 222c  ll",.    "all_",
+0001af30: 0a20 2020 2064 6566 6175 6c74 3d46 616c  .    default=Fal
+0001af40: 7365 2c0a 2020 2020 6865 6c70 3d22 5265  se,.    help="Re
+0001af50: 6d6f 7665 2063 6c69 7073 2066 6f72 2061  move clips for a
+0001af60: 6c6c 2073 6f6e 6773 2e20 4967 6e6f 7265  ll songs. Ignore
+0001af70: 7320 534f 4e47 5f49 4453 2e22 2c0a 290a  s SONG_IDS.",.).
+0001af80: 4063 6c69 636b 2e6f 7074 696f 6e28 222d  @click.option("-
+0001af90: 462f 2d6e 4622 2c20 222d 2d66 6f72 6365  F/-nF", "--force
+0001afa0: 2f2d 2d6e 6f2d 666f 7263 6522 2c20 2266  /--no-force", "f
+0001afb0: 6f72 6365 222c 2064 6566 6175 6c74 3d46  orce", default=F
+0001afc0: 616c 7365 290a 6465 6620 756e 636c 6970  alse).def unclip
+0001afd0: 2873 6f6e 675f 6964 732c 2061 6c6c 5f2c  (song_ids, all_,
+0001afe0: 2066 6f72 6365 293a 0a20 2020 2022 2222   force):.    """
+0001aff0: 0a20 2020 2052 656d 6f76 6520 636c 6970  .    Remove clip
+0001b000: 7320 666f 7220 7370 6563 6966 6963 2073  s for specific s
+0001b010: 6f6e 6728 7329 2e0a 0a20 2020 2052 656d  ong(s)...    Rem
+0001b020: 6f76 6573 2063 6c69 7020 666f 7220 7468  oves clip for th
+0001b030: 6520 736f 6e67 2873 2920 7769 7468 2049  e song(s) with I
+0001b040: 4428 7329 2053 4f4e 475f 4944 532e 0a0a  D(s) SONG_IDS...
+0001b050: 2020 2020 4966 2074 6865 2027 2d41 2f2d      If the '-A/-
+0001b060: 2d61 6c6c 2720 666c 6167 2069 7320 7061  -all' flag is pa
+0001b070: 7373 6564 2c20 7468 6520 636c 6970 7320  ssed, the clips 
+0001b080: 666f 7220 616c 6c20 736f 6e67 7320 7769  for all songs wi
+0001b090: 6c6c 2062 6520 7265 6d6f 7665 642c 0a20  ll be removed,. 
+0001b0a0: 2020 2069 676e 6f72 696e 6720 534f 4e47     ignoring SONG
+0001b0b0: 5f49 4453 2e20 5468 6973 2070 726f 6d70  _IDS. This promp
+0001b0c0: 7473 2066 6f72 2063 6f6e 6669 726d 6174  ts for confirmat
+0001b0d0: 696f 6e20 756e 6c65 7373 2074 6865 2027  ion unless the '
+0001b0e0: 2d46 2f2d 2d66 6f72 6365 270a 2020 2020  -F/--force'.    
+0001b0f0: 666c 6167 2069 7320 7061 7373 6564 2e0a  flag is passed..
+0001b100: 2020 2020 2222 220a 2020 2020 6966 206e      """.    if n
+0001b110: 6f74 2061 6c6c 5f3a 0a20 2020 2020 2020  ot all_:.       
+0001b120: 2069 6620 736f 6e67 5f69 6473 3a0a 2020   if song_ids:.  
+0001b130: 2020 2020 2020 2020 2020 736f 6e67 5f69            song_i
+0001b140: 6473 203d 2073 6574 2873 6f6e 675f 6964  ds = set(song_id
+0001b150: 7329 0a20 2020 2020 2020 2065 6c73 653a  s).        else:
+0001b160: 0a20 2020 2020 2020 2020 2020 2063 6c69  .            cli
+0001b170: 636b 2e73 6563 686f 280a 2020 2020 2020  ck.secho(.      
+0001b180: 2020 2020 2020 2020 2020 224e 6f20 736f            "No so
+0001b190: 6e67 2049 4473 2070 6173 7365 642e 2054  ng IDs passed. T
+0001b1a0: 6f20 7265 6d6f 7665 2063 6c69 7073 2066  o remove clips f
+0001b1b0: 6f72 2061 6c6c 2073 6f6e 6773 2c20 7061  or all songs, pa
+0001b1c0: 7373 2074 6865 2027 2d41 2f2d 2d61 6c6c  ss the '-A/--all
+0001b1d0: 2720 666c 6167 2e22 2c0a 2020 2020 2020  ' flag.",.      
+0001b1e0: 2020 2020 2020 2020 2020 6667 3d22 7265            fg="re
+0001b1f0: 6422 2c0a 2020 2020 2020 2020 2020 2020  d",.            
+0001b200: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+0001b210: 7475 726e 0a0a 2020 2020 6966 2061 6c6c  turn..    if all
+0001b220: 5f20 616e 6420 6e6f 7420 666f 7263 653a  _ and not force:
+0001b230: 0a20 2020 2020 2020 2063 6c69 636b 2e65  .        click.e
+0001b240: 6368 6f28 0a20 2020 2020 2020 2020 2020  cho(.           
+0001b250: 2022 4172 6520 796f 7520 7375 7265 2079   "Are you sure y
+0001b260: 6f75 2077 616e 7420 746f 2072 656d 6f76  ou want to remov
+0001b270: 6520 636c 6970 7320 666f 7220 616c 6c20  e clips for all 
+0001b280: 736f 6e67 733f 2054 6869 7320 6361 6e6e  songs? This cann
+0001b290: 6f74 2062 6520 756e 646f 6e65 2e20 5b79  ot be undone. [y
+0001b2a0: 2f6e 5d20 222c 0a20 2020 2020 2020 2029  /n] ",.        )
+0001b2b0: 0a20 2020 2020 2020 2069 6620 696e 7075  .        if inpu
+0001b2c0: 7428 292e 6c6f 7765 7228 2920 213d 2022  t().lower() != "
+0001b2d0: 7922 3a0a 2020 2020 2020 2020 2020 2020  y":.            
+0001b2e0: 7265 7475 726e 0a0a 2020 2020 7769 7468  return..    with
+0001b2f0: 206f 7065 6e28 534f 4e47 535f 494e 464f   open(SONGS_INFO
+0001b300: 5f50 4154 482c 2022 722b 222c 2065 6e63  _PATH, "r+", enc
+0001b310: 6f64 696e 673d 2275 7466 2d38 2229 2061  oding="utf-8") a
+0001b320: 7320 736f 6e67 735f 6669 6c65 3a0a 2020  s songs_file:.  
+0001b330: 2020 2020 2020 6c69 6e65 7320 3d20 736f        lines = so
+0001b340: 6e67 735f 6669 6c65 2e72 6561 646c 696e  ngs_file.readlin
+0001b350: 6573 2829 0a0a 2020 2020 2020 2020 666f  es()..        fo
+0001b360: 7220 6920 696e 2072 616e 6765 286c 656e  r i in range(len
+0001b370: 286c 696e 6573 2929 3a0a 2020 2020 2020  (lines)):.      
+0001b380: 2020 2020 2020 6465 7461 696c 7320 3d20        details = 
+0001b390: 6c69 6e65 735b 695d 2e73 7472 6970 2829  lines[i].strip()
+0001b3a0: 2e73 706c 6974 2822 7c22 290a 2020 2020  .split("|").    
+0001b3b0: 2020 2020 2020 2020 6966 2061 6c6c 5f20          if all_ 
+0001b3c0: 6f72 2069 6e74 2864 6574 6169 6c73 5b30  or int(details[0
+0001b3d0: 5d29 2069 6e20 736f 6e67 5f69 6473 3a0a  ]) in song_ids:.
+0001b3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b3f0: 6c69 6e65 735b 695d 203d 2022 7c22 2e6a  lines[i] = "|".j
+0001b400: 6f69 6e28 6465 7461 696c 735b 3a33 5d20  oin(details[:3] 
+0001b410: 2b20 5b22 225d 202b 2064 6574 6169 6c73  + [""] + details
+0001b420: 5b35 3a5d 2920 2b20 225c 6e22 0a0a 2020  [5:]) + "\n"..  
+0001b430: 2020 2020 2020 736f 6e67 735f 6669 6c65        songs_file
+0001b440: 2e73 6565 6b28 3029 0a20 2020 2020 2020  .seek(0).       
+0001b450: 2073 6f6e 6773 5f66 696c 652e 7772 6974   songs_file.writ
+0001b460: 6528 2222 2e6a 6f69 6e28 6c69 6e65 7329  e("".join(lines)
+0001b470: 290a 2020 2020 2020 2020 736f 6e67 735f  ).        songs_
+0001b480: 6669 6c65 2e74 7275 6e63 6174 6528 290a  file.truncate().
+0001b490: 0a20 2020 2069 6620 616c 6c5f 3a0a 2020  .    if all_:.  
+0001b4a0: 2020 2020 2020 636c 6963 6b2e 7365 6368        click.sech
+0001b4b0: 6f28 2252 656d 6f76 6564 2063 6c69 7073  o("Removed clips
+0001b4c0: 2066 6f72 2061 6c6c 2073 6f6e 6773 2e22   for all songs."
+0001b4d0: 2c20 6667 3d22 6772 6565 6e22 290a 2020  , fg="green").  
+0001b4e0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0001b4f0: 636c 6963 6b2e 7365 6368 6f28 0a20 2020  click.secho(.   
+0001b500: 2020 2020 2020 2020 2066 2252 656d 6f76           f"Remov
+0001b510: 6564 2063 6c69 7028 7329 2066 6f72 2073  ed clip(s) for s
+0001b520: 6f6e 6728 7329 2077 6974 6820 4944 2873  ong(s) with ID(s
+0001b530: 2920 7b27 2c20 272e 6a6f 696e 286d 6170  ) {', '.join(map
+0001b540: 2873 7472 2c20 736f 6e67 5f69 6473 2929  (str, song_ids))
+0001b550: 7d2e 222c 0a20 2020 2020 2020 2020 2020  }.",.           
+0001b560: 2066 673d 2267 7265 656e 222c 0a20 2020   fg="green",.   
+0001b570: 2020 2020 2029 0a0a 0a40 636c 692e 636f       )...@cli.co
+0001b580: 6d6d 616e 6428 290a 4063 6c69 636b 2e61  mmand().@click.a
+0001b590: 7267 756d 656e 7428 2273 6f6e 675f 6964  rgument("song_id
+0001b5a0: 222c 2074 7970 653d 696e 742c 2072 6571  ", type=int, req
+0001b5b0: 7569 7265 643d 5472 7565 290a 4063 6c69  uired=True).@cli
+0001b5c0: 636b 2e61 7267 756d 656e 7428 2270 6169  ck.argument("pai
+0001b5d0: 7273 222c 2074 7970 653d 7374 722c 2072  rs", type=str, r
+0001b5e0: 6571 7569 7265 643d 4661 6c73 6529 0a64  equired=False).d
+0001b5f0: 6566 206d 6574 6164 6174 6128 736f 6e67  ef metadata(song
+0001b600: 5f69 642c 2070 6169 7273 293a 0a20 2020  _id, pairs):.   
+0001b610: 2022 2222 0a20 2020 2056 6965 7720 6f72   """.    View or
+0001b620: 2065 6469 7420 7468 6520 6d65 7461 6461   edit the metada
+0001b630: 7461 2066 6f72 2061 2073 6f6e 672e 0a0a  ta for a song...
+0001b640: 2020 2020 4966 206e 6f20 5041 4952 5320      If no PAIRS 
+0001b650: 6172 6520 7061 7373 6564 2c20 7072 696e  are passed, prin
+0001b660: 7473 2074 6865 206d 6574 6164 6174 6120  ts the metadata 
+0001b670: 666f 7220 7468 6520 736f 6e67 2077 6974  for the song wit
+0001b680: 6820 4944 2053 4f4e 475f 4944 2e0a 0a20  h ID SONG_ID... 
+0001b690: 2020 2049 6620 5041 4952 5320 6172 6520     If PAIRS are 
+0001b6a0: 7061 7373 6564 2c20 7365 7473 2074 6865  passed, sets the
+0001b6b0: 206d 6574 6164 6174 6120 666f 7220 7468   metadata for th
+0001b6c0: 6520 736f 6e67 2077 6974 6820 4944 2053  e song with ID S
+0001b6d0: 4f4e 475f 4944 2074 6f20 7468 650a 2020  ONG_ID to the.  
+0001b6e0: 2020 6b65 792d 7661 6c75 6520 7061 6972    key-value pair
+0001b6f0: 7320 696e 2050 4149 5253 2e20 5041 4952  s in PAIRS. PAIR
+0001b700: 5320 7368 6f75 6c64 2062 6520 6120 7374  S should be a st
+0001b710: 7269 6e67 206f 6620 7468 6520 666f 726d  ring of the form
+0001b720: 0a20 2020 2027 6b65 7931 3a76 616c 7565  .    'key1:value
+0001b730: 317c 6b65 7932 3a76 616c 7565 327c 2e2e  1|key2:value2|..
+0001b740: 2e27 2e0a 0a20 2020 2050 6f73 7369 626c  .'...    Possibl
+0001b750: 6520 6564 6974 6162 6c65 206d 6574 6164  e editable metad
+0001b760: 6174 6120 6b65 7973 2061 7265 3a20 616c  ata keys are: al
+0001b770: 6275 6d2c 2061 6c62 756d 6172 7469 7374  bum, albumartist
+0001b780: 2c20 6172 7469 7374 2c20 6172 7477 6f72  , artist, artwor
+0001b790: 6b2c 0a20 2020 2063 6f6d 6d65 6e74 2c20  k,.    comment, 
+0001b7a0: 636f 6d70 696c 6174 696f 6e2c 2063 6f6d  compilation, com
+0001b7b0: 706f 7365 722c 2064 6973 636e 756d 6265  poser, discnumbe
+0001b7c0: 722c 2067 656e 7265 2c20 6c79 7269 6373  r, genre, lyrics
+0001b7d0: 2c20 746f 7461 6c64 6973 6373 2c0a 2020  , totaldiscs,.  
+0001b7e0: 2020 746f 7461 6c74 7261 636b 732c 2074    totaltracks, t
+0001b7f0: 7261 636b 6e75 6d62 6572 2c20 7472 6163  racknumber, trac
+0001b800: 6b74 6974 6c65 2c20 7965 6172 2c20 6973  ktitle, year, is
+0001b810: 7263 0a0a 2020 2020 4b65 7973 2061 7265  rc..    Keys are
+0001b820: 206e 6f74 2063 6173 6520 7365 6e73 6974   not case sensit
+0001b830: 6976 6520 616e 6420 6361 6e20 636f 6e74  ive and can cont
+0001b840: 6169 6e20 6172 6269 7472 6172 7920 7768  ain arbitrary wh
+0001b850: 6974 6573 7061 6365 2c20 272d 272c 2061  itespace, '-', a
+0001b860: 6e64 0a20 2020 2027 5f27 2063 6861 7261  nd.    '_' chara
+0001b870: 6374 6572 732e 2049 6e20 6f74 6865 7220  cters. In other 
+0001b880: 776f 7264 732c 2027 416c 6275 6d20 4172  words, 'Album Ar
+0001b890: 7469 7374 272c 2027 616c 6275 6d2d 6172  tist', 'album-ar
+0001b8a0: 7469 7374 272c 2061 6e64 0a20 2020 2027  tist', and.    '
+0001b8b0: 616c 6275 6d5f 6172 7469 7374 2720 6172  album_artist' ar
+0001b8c0: 6520 616c 6c20 7379 6e6f 6e79 6d73 2066  e all synonyms f
+0001b8d0: 6f72 2027 616c 6275 6d61 7274 6973 7427  or 'albumartist'
+0001b8e0: 2e20 416c 736f 2c20 2764 6973 6b27 2069  . Also, 'disk' i
+0001b8f0: 730a 2020 2020 7379 6e6f 6e79 6d6f 7573  s.    synonymous
+0001b900: 2077 6974 6820 2764 6973 6327 2e0a 2020   with 'disc'..  
+0001b910: 2020 2222 220a 0a20 2020 2077 6974 6820    """..    with 
+0001b920: 6f70 656e 2853 4f4e 4753 5f49 4e46 4f5f  open(SONGS_INFO_
+0001b930: 5041 5448 2c20 2272 222c 2065 6e63 6f64  PATH, "r", encod
+0001b940: 696e 673d 2275 7466 2d38 2229 2061 7320  ing="utf-8") as 
+0001b950: 736f 6e67 735f 6669 6c65 3a0a 2020 2020  songs_file:.    
+0001b960: 2020 2020 6c69 6e65 7320 3d20 736f 6e67      lines = song
+0001b970: 735f 6669 6c65 2e72 6561 646c 696e 6573  s_file.readlines
+0001b980: 2829 0a0a 2020 2020 2020 2020 666f 7220  ()..        for 
+0001b990: 6920 696e 2072 616e 6765 286c 656e 286c  i in range(len(l
+0001b9a0: 696e 6573 2929 3a0a 2020 2020 2020 2020  ines)):.        
+0001b9b0: 2020 2020 6465 7461 696c 7320 3d20 6c69      details = li
+0001b9c0: 6e65 735b 695d 2e73 7472 6970 2829 2e73  nes[i].strip().s
+0001b9d0: 706c 6974 2822 7c22 290a 2020 2020 2020  plit("|").      
+0001b9e0: 2020 2020 2020 6966 2069 6e74 2864 6574        if int(det
+0001b9f0: 6169 6c73 5b30 5d29 203d 3d20 736f 6e67  ails[0]) == song
+0001ba00: 5f69 643a 0a20 2020 2020 2020 2020 2020  _id:.           
+0001ba10: 2020 2020 2073 6f6e 675f 7061 7468 203d       song_path =
+0001ba20: 206f 732e 7061 7468 2e6a 6f69 6e28 534f   os.path.join(SO
+0001ba30: 4e47 535f 4449 522c 2064 6574 6169 6c73  NGS_DIR, details
+0001ba40: 5b31 5d29 0a20 2020 2020 2020 2020 2020  [1]).           
+0001ba50: 2020 2020 2073 6f6e 675f 6e61 6d65 203d       song_name =
+0001ba60: 2064 6574 6169 6c73 5b31 5d0a 2020 2020   details[1].    
+0001ba70: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+0001ba80: 6f74 206f 732e 7061 7468 2e65 7869 7374  ot os.path.exist
+0001ba90: 7328 736f 6e67 5f70 6174 6829 3a0a 2020  s(song_path):.  
+0001baa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bab0: 2020 636c 6963 6b2e 7365 6368 6f28 0a20    click.secho(. 
+0001bac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bad0: 2020 2020 2020 2066 2253 6f6e 6720 6669         f"Song fi
+0001bae0: 6c65 207b 736f 6e67 5f6e 616d 657d 2028  le {song_name} (
+0001baf0: 4944 207b 736f 6e67 5f69 647d 2920 6e6f  ID {song_id}) no
+0001bb00: 7420 666f 756e 642e 222c 0a20 2020 2020  t found.",.     
+0001bb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bb20: 2020 2066 673d 2272 6564 222c 0a20 2020     fg="red",.   
+0001bb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bb40: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+0001bb50: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+0001bb60: 2020 2020 2020 2020 2020 2020 2020 6272                br
+0001bb70: 6561 6b0a 2020 2020 2020 2020 656c 7365  eak.        else
+0001bb80: 3a0a 2020 2020 2020 2020 2020 2020 636c  :.            cl
+0001bb90: 6963 6b2e 7365 6368 6f28 0a20 2020 2020  ick.secho(.     
+0001bba0: 2020 2020 2020 2020 2020 2066 224e 6f20             f"No 
+0001bbb0: 736f 6e67 2077 6974 6820 4944 207b 736f  song with ID {so
+0001bbc0: 6e67 5f69 647d 2066 6f75 6e64 2e22 2c0a  ng_id} found.",.
+0001bbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bbe0: 6667 3d22 7265 6422 2c0a 2020 2020 2020  fg="red",.      
+0001bbf0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0001bc00: 2020 2020 7265 7475 726e 0a0a 2020 2020      return..    
+0001bc10: 6966 2070 6169 7273 3a0a 2020 2020 2020  if pairs:.      
+0001bc20: 2020 7061 6972 7320 3d20 5b74 7570 6c65    pairs = [tuple
+0001bc30: 2870 6169 722e 7374 7269 7028 292e 7370  (pair.strip().sp
+0001bc40: 6c69 7428 223a 2229 2920 666f 7220 7061  lit(":")) for pa
+0001bc50: 6972 2069 6e20 7061 6972 732e 7370 6c69  ir in pairs.spli
+0001bc60: 7428 227c 2229 5d0a 0a20 2020 2020 2020  t("|")]..       
+0001bc70: 2073 6f6e 675f 6461 7461 203d 206d 7573   song_data = mus
+0001bc80: 6963 5f74 6167 2e6c 6f61 645f 6669 6c65  ic_tag.load_file
+0001bc90: 2873 6f6e 675f 7061 7468 290a 2020 2020  (song_path).    
+0001bca0: 2020 2020 7661 6c69 645f 7061 6972 7320      valid_pairs 
+0001bcb0: 3d20 7061 6972 735b 3a5d 0a20 2020 2020  = pairs[:].     
+0001bcc0: 2020 2066 6f72 206b 6579 2c20 7661 6c75     for key, valu
+0001bcd0: 6520 696e 2070 6169 7273 3a0a 2020 2020  e in pairs:.    
+0001bce0: 2020 2020 2020 2020 6966 206b 6579 206e          if key n
+0001bcf0: 6f74 2069 6e20 4d45 5441 4441 5441 5f4b  ot in METADATA_K
+0001bd00: 4559 5320 6f72 206b 6579 2e73 7461 7274  EYS or key.start
+0001bd10: 7377 6974 6828 2223 2229 3a0a 2020 2020  swith("#"):.    
+0001bd20: 2020 2020 2020 2020 2020 2020 636c 6963              clic
+0001bd30: 6b2e 7365 6368 6f28 0a20 2020 2020 2020  k.secho(.       
+0001bd40: 2020 2020 2020 2020 2020 2020 2066 2227               f"'
+0001bd50: 7b6b 6579 7d27 2069 7320 6e6f 7420 6120  {key}' is not a 
+0001bd60: 7661 6c69 6420 6564 6974 6162 6c65 206d  valid editable m
+0001bd70: 6574 6164 6174 6120 6b65 792e 222c 2066  etadata key.", f
+0001bd80: 673d 2272 6564 220a 2020 2020 2020 2020  g="red".        
+0001bd90: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0001bda0: 2020 2020 2020 2020 2020 7661 6c69 645f            valid_
+0001bdb0: 7061 6972 732e 7265 6d6f 7665 2828 6b65  pairs.remove((ke
+0001bdc0: 792c 2076 616c 7565 2929 0a20 2020 2020  y, value)).     
+0001bdd0: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
+0001bde0: 6e75 650a 2020 2020 2020 2020 2020 2020  nue.            
+0001bdf0: 736f 6e67 5f64 6174 615b 6b65 795d 203d  song_data[key] =
+0001be00: 2076 616c 7565 0a0a 2020 2020 2020 2020   value..        
+0001be10: 736f 6e67 5f64 6174 612e 7361 7665 2829  song_data.save()
+0001be20: 0a0a 2020 2020 2020 2020 636c 6963 6b2e  ..        click.
+0001be30: 7365 6368 6f28 0a20 2020 2020 2020 2020  secho(.         
+0001be40: 2020 2066 2253 6574 206d 6574 6164 6174     f"Set metadat
+0001be50: 6120 666f 7220 277b 736f 6e67 5f6e 616d  a for '{song_nam
+0001be60: 657d 2720 7769 7468 2049 4420 7b73 6f6e  e}' with ID {son
+0001be70: 675f 6964 7d20 746f 207b 7661 6c69 645f  g_id} to {valid_
+0001be80: 7061 6972 737d 2e22 2c0a 2020 2020 2020  pairs}.",.      
+0001be90: 2020 2020 2020 6667 3d22 6772 6565 6e22        fg="green"
+0001bea0: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
+0001beb0: 656c 7365 3a0a 2020 2020 2020 2020 736f  else:.        so
+0001bec0: 6e67 5f64 6174 6120 3d20 6d75 7369 635f  ng_data = music_
+0001bed0: 7461 672e 6c6f 6164 5f66 696c 6528 736f  tag.load_file(so
+0001bee0: 6e67 5f70 6174 6829 0a20 2020 2020 2020  ng_path).       
+0001bef0: 2063 6c69 636b 2e65 6368 6f28 224d 6574   click.echo("Met
+0001bf00: 6164 6174 6120 666f 7220 222c 206e 6c3d  adata for ", nl=
+0001bf10: 4661 6c73 6529 0a20 2020 2020 2020 2063  False).        c
+0001bf20: 6c69 636b 2e73 6563 686f 2873 6f6e 675f  lick.secho(song_
+0001bf30: 6e61 6d65 2c20 6667 3d22 626c 7565 222c  name, fg="blue",
+0001bf40: 2062 6f6c 643d 5472 7565 2c20 6e6c 3d46   bold=True, nl=F
+0001bf50: 616c 7365 290a 2020 2020 2020 2020 636c  alse).        cl
+0001bf60: 6963 6b2e 6563 686f 2866 2220 7769 7468  ick.echo(f" with
+0001bf70: 2049 4420 7b73 6f6e 675f 6964 7d3a 2229   ID {song_id}:")
+0001bf80: 0a0a 2020 2020 2020 2020 666f 7220 6b65  ..        for ke
+0001bf90: 7920 696e 204d 4554 4144 4154 415f 4b45  y in METADATA_KE
+0001bfa0: 5953 3a0a 2020 2020 2020 2020 2020 2020  YS:.            
+0001bfb0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+0001bfc0: 2020 2020 2063 6c69 636b 2e65 6368 6f28       click.echo(
+0001bfd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001bfe0: 2020 2020 2066 225c 747b 6b65 7920 6966       f"\t{key if
+0001bff0: 206e 6f74 206b 6579 2e73 7461 7274 7377   not key.startsw
+0001c000: 6974 6828 2723 2729 2065 6c73 6520 6b65  ith('#') else ke
+0001c010: 795b 313a 5d7d 3a20 7b73 6f6e 675f 6461  y[1:]}: {song_da
+0001c020: 7461 5b6b 6579 5d2e 7661 6c75 657d 220a  ta[key].value}".
+0001c030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c040: 290a 2020 2020 2020 2020 2020 2020 6578  ).            ex
+0001c050: 6365 7074 3a20 2023 2070 796c 696e 743a  cept:  # pylint:
+0001c060: 2064 6973 6162 6c65 3d62 6172 652d 6578   disable=bare-ex
+0001c070: 6365 7074 0a20 2020 2020 2020 2020 2020  cept.           
+0001c080: 2020 2020 2070 6173 730a 0a0a 4063 6c69       pass...@cli
+0001c090: 2e63 6f6d 6d61 6e64 286e 616d 653d 2264  .command(name="d
+0001c0a0: 6972 2229 0a40 636c 6963 6b2e 6172 6775  ir").@click.argu
+0001c0b0: 6d65 6e74 2822 6469 7265 6374 6f72 7922  ment("directory"
+0001c0c0: 2c20 7479 7065 3d63 6c69 636b 2e50 6174  , type=click.Pat
+0001c0d0: 6828 6669 6c65 5f6f 6b61 793d 4661 6c73  h(file_okay=Fals
+0001c0e0: 6529 2c20 7265 7175 6972 6564 3d46 616c  e), required=Fal
+0001c0f0: 7365 290a 6465 6620 6469 725f 2864 6972  se).def dir_(dir
+0001c100: 6563 746f 7279 293a 0a20 2020 2022 2222  ectory):.    """
+0001c110: 0a20 2020 2043 6861 6e67 6520 7468 6520  .    Change the 
+0001c120: 6469 7265 6374 6f72 7920 7768 6572 6520  directory where 
+0001c130: 6d61 6573 7472 6f20 6c6f 6f6b 7320 666f  maestro looks fo
+0001c140: 7220 736f 6e67 732e 0a20 2020 204e 4f54  r songs..    NOT
+0001c150: 453a 2054 6869 7320 646f 6573 206e 6f74  E: This does not
+0001c160: 206d 6f76 6520 616e 7920 736f 6e67 732e   move any songs.
+0001c170: 2049 7420 6f6e 6c79 2063 6861 6e67 6573   It only changes
+0001c180: 2077 6865 7265 206d 6165 7374 726f 206c   where maestro l
+0001c190: 6f6f 6b73 2066 6f72 0a20 2020 2073 6f6e  ooks for.    son
+0001c1a0: 6773 2e20 596f 7520 7769 6c6c 2068 6176  gs. You will hav
+0001c1b0: 6520 746f 206d 6f76 6520 7468 6520 736f  e to move the so
+0001c1c0: 6e67 7320 796f 7572 7365 6c66 2e0a 0a20  ngs yourself... 
+0001c1d0: 2020 2049 6620 6e6f 2061 7267 756d 656e     If no argumen
+0001c1e0: 7420 6973 2070 6173 7365 642c 2070 7269  t is passed, pri
+0001c1f0: 6e74 7320 7468 6520 6375 7272 656e 7420  nts the current 
+0001c200: 6469 7265 6374 6f72 792e 0a20 2020 2022  directory..    "
+0001c210: 2222 0a0a 2020 2020 6966 2064 6972 6563  ""..    if direc
+0001c220: 746f 7279 2069 7320 4e6f 6e65 3a0a 2020  tory is None:.  
+0001c230: 2020 2020 2020 636c 6963 6b2e 6563 686f        click.echo
+0001c240: 2853 4f4e 4753 5f44 4952 290a 2020 2020  (SONGS_DIR).    
+0001c250: 2020 2020 7265 7475 726e 0a0a 2020 2020      return..    
+0001c260: 6966 206e 6f74 206f 732e 7061 7468 2e65  if not os.path.e
+0001c270: 7869 7374 7328 6469 7265 6374 6f72 7929  xists(directory)
+0001c280: 3a0a 2020 2020 2020 2020 6f73 2e6d 616b  :.        os.mak
+0001c290: 6564 6972 7328 6469 7265 6374 6f72 7929  edirs(directory)
+0001c2a0: 0a0a 2020 2020 7769 7468 206f 7065 6e28  ..    with open(
+0001c2b0: 5345 5454 494e 4753 5f46 494c 452c 2022  SETTINGS_FILE, "
+0001c2c0: 722b 222c 2065 6e63 6f64 696e 673d 2275  r+", encoding="u
+0001c2d0: 7466 2d38 2229 2061 7320 7365 7474 696e  tf-8") as settin
+0001c2e0: 6773 5f66 696c 653a 0a20 2020 2020 2020  gs_file:.       
+0001c2f0: 2073 6574 7469 6e67 7320 3d20 6a73 6f6e   settings = json
+0001c300: 2e6c 6f61 6428 7365 7474 696e 6773 5f66  .load(settings_f
+0001c310: 696c 6529 0a20 2020 2020 2020 2073 6574  ile).        set
+0001c320: 7469 6e67 735b 2273 6f6e 675f 6469 7265  tings["song_dire
+0001c330: 6374 6f72 7922 5d20 3d20 6469 7265 6374  ctory"] = direct
+0001c340: 6f72 790a 2020 2020 2020 2020 7365 7474  ory.        sett
+0001c350: 696e 6773 5f66 696c 652e 7365 656b 2830  ings_file.seek(0
+0001c360: 290a 2020 2020 2020 2020 6a73 6f6e 2e64  ).        json.d
+0001c370: 756d 7028 7365 7474 696e 6773 2c20 7365  ump(settings, se
+0001c380: 7474 696e 6773 5f66 696c 6529 0a20 2020  ttings_file).   
+0001c390: 2020 2020 2073 6574 7469 6e67 735f 6669       settings_fi
+0001c3a0: 6c65 2e74 7275 6e63 6174 6528 290a 0a20  le.truncate().. 
+0001c3b0: 2020 2063 6c69 636b 2e73 6563 686f 2866     click.secho(f
+0001c3c0: 2243 6861 6e67 6564 2073 6f6e 6720 6469  "Changed song di
+0001c3d0: 7265 6374 6f72 7920 746f 207b 6469 7265  rectory to {dire
+0001c3e0: 6374 6f72 797d 2e22 2c20 6667 3d22 6772  ctory}.", fg="gr
+0001c3f0: 6565 6e22 29                             een")
```

### Comparing `maestro-music-1.0.5/maestro_music.egg-info/PKG-INFO` & `maestro-music-1.0.6/maestro_music.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maestro-music
-Version: 1.0.5
+Version: 1.0.6
 Summary: A simple command line tool to play songs (or any audio files, really).
 Home-page: https://github.com/PrajwalVandana/maestro-cli
 Author: Prajwal Vandana
 License: MIT
 Keywords: music,sound,audio,music-player,cli,ogg,flac,mp3,wav,spotify,youtube,audio-visualization,audio-visualizer
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

