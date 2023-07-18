# Comparing `tmp/quisk-4.2.8.tar.gz` & `tmp/quisk-4.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quisk-4.2.8.tar", last modified: Fri Sep 30 15:26:32 2022, max compression
+gzip compressed data, was "quisk-4.2.9.tar", last modified: Wed Oct  5 16:46:56 2022, max compression
```

## Comparing `quisk-4.2.8.tar` & `quisk-4.2.9.tar`

### file list

```diff
@@ -1,196 +1,196 @@
-drwxrwxrwx   0 jim       (1000) jim       (1000)        0 2022-09-30 15:26:32.681439 quisk-4.2.8/
--rwxrwxrwx   0 jim       (1000) jim       (1000)   100741 2022-09-29 13:49:37.000000 quisk-4.2.8/CHANGELOG.txt
--rwxrwxrwx   0 jim       (1000) jim       (1000)       52 2011-09-09 11:12:18.000000 quisk-4.2.8/Extensions.txt
--rwxrwxrwx   0 jim       (1000) jim       (1000)      287 2022-08-15 19:42:43.000000 quisk-4.2.8/MANIFEST.in
--rwxrwxrwx   0 jim       (1000) jim       (1000)     1571 2022-09-30 15:26:32.681134 quisk-4.2.8/PKG-INFO
--rwxrwxrwx   0 jim       (1000) jim       (1000)       52 2011-09-09 11:12:20.000000 quisk-4.2.8/README.txt
--rwxrwxrwx   0 jim       (1000) jim       (1000)     2300 2018-11-23 19:45:24.000000 quisk-4.2.8/WinEdit.pyw
--rwxrwxrwx   0 jim       (1000) jim       (1000)      176 2018-11-23 19:45:24.000000 quisk-4.2.8/WinQuisk.pyw
--rwxrwxrwx   0 jim       (1000) jim       (1000)      213 2018-11-23 19:45:24.000000 quisk-4.2.8/WinQuiskVna.pyw
--rwxrwxrwx   0 jim       (1000) jim       (1000)       45 2022-09-30 15:26:32.000000 quisk-4.2.8/__init__.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)      177 2019-11-23 21:29:34.000000 quisk-4.2.8/__main__.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)   257024 2022-09-05 17:24:06.000000 quisk-4.2.8/_quisk.pyd
-drwxrwxrwx   0 jim       (1000) jim       (1000)        0 2022-09-30 15:26:32.651282 quisk-4.2.8/ac2yd/
--rwxrwxrwx   0 jim       (1000) jim       (1000)   371367 2022-08-14 16:18:32.000000 quisk-4.2.8/ac2yd/Design_2022_0531.pdf
--rwxrwxrwx   0 jim       (1000) jim       (1000)        2 2022-08-30 20:10:29.000000 quisk-4.2.8/ac2yd/__init__.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)    16138 2022-09-27 18:05:44.000000 quisk-4.2.8/ac2yd/control_common.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)     1898 2022-09-26 19:26:38.000000 quisk-4.2.8/ac2yd/control_hermes.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)      347 2022-08-24 20:42:19.000000 quisk-4.2.8/ac2yd/control_softrock.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)    29580 2022-09-30 15:10:14.000000 quisk-4.2.8/ac2yd/remote.c
--rwxrwxrwx   0 jim       (1000) jim       (1000)    16977 2022-09-27 18:05:26.000000 quisk-4.2.8/ac2yd/remote_common.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)      841 2022-09-15 20:06:21.000000 quisk-4.2.8/ac2yd/remote_hermes.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)      554 2022-09-15 20:16:05.000000 quisk-4.2.8/ac2yd/remote_softrock.py
-drwxrwxrwx   0 jim       (1000) jim       (1000)        0 2022-09-30 15:26:32.655202 quisk-4.2.8/afedrinet/
--rwxrwxrwx   0 jim       (1000) jim       (1000)      173 2019-01-26 19:28:41.000000 quisk-4.2.8/afedrinet/SOURCE.txt
--rwxrwxrwx   0 jim       (1000) jim       (1000)        2 2014-12-10 16:01:00.000000 quisk-4.2.8/afedrinet/__init__.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)      183 2014-12-10 16:01:00.000000 quisk-4.2.8/afedrinet/af_comp.bat.makeit
--rwxrwxrwx   0 jim       (1000) jim       (1000)      313 2016-04-14 00:44:28.000000 quisk-4.2.8/afedrinet/afe_library
--rwxrwxrwx   0 jim       (1000) jim       (1000)      518 2015-12-13 16:29:58.000000 quisk-4.2.8/afedrinet/afe_library.mac
--rwxrwxrwx   0 jim       (1000) jim       (1000)     8526 2020-01-09 18:56:17.000000 quisk-4.2.8/afedrinet/afedri.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)    11632 2019-09-22 18:48:57.000000 quisk-4.2.8/afedrinet/afedrinet_io.c
--rwxrwxrwx   0 jim       (1000) jim       (1000)    21504 2022-09-05 17:24:07.000000 quisk-4.2.8/afedrinet/afedrinet_io.pyd
-drwxrwxrwx   0 jim       (1000) jim       (1000)        0 2022-09-30 15:26:32.657901 quisk-4.2.8/afedrinet/build/
--rwxrwxrwx   0 jim       (1000) jim       (1000)    34320 2020-12-20 17:44:14.000000 quisk-4.2.8/afedrinet/build/import_quisk_api.o
--rwxrwxrwx   0 jim       (1000) jim       (1000)    52640 2020-12-20 17:44:14.000000 quisk-4.2.8/afedrinet/build/is_key_down.o
-drwxrwxrwx   0 jim       (1000) jim       (1000)        0 2022-09-30 15:26:32.659127 quisk-4.2.8/afedrinet/build/temp.linux-x86_64-3.6/
--rwxrwxrwx   0 jim       (1000) jim       (1000)    67672 2020-12-20 17:44:14.000000 quisk-4.2.8/afedrinet/build/temp.linux-x86_64-3.6/afedrinet_io.o
--rwxrwxrwx   0 jim       (1000) jim       (1000)      119 2020-11-30 16:57:37.000000 quisk-4.2.8/afedrinet/makefile
--rwxrwxrwx   0 jim       (1000) jim       (1000)     3676 2015-11-22 23:00:54.000000 quisk-4.2.8/afedrinet/quisk_conf.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)     3600 2015-12-10 15:25:14.000000 quisk-4.2.8/afedrinet/quisk_conf_linux.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)     3600 2015-12-10 15:25:14.000000 quisk-4.2.8/afedrinet/quisk_conf_mac.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)     3370 2020-05-23 21:28:44.000000 quisk-4.2.8/afedrinet/quisk_hardware.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)     2645 2015-12-13 21:10:59.000000 quisk-4.2.8/afedrinet/readme.txt
--rwxrwxrwx   0 jim       (1000) jim       (1000)     1222 2020-01-09 18:03:05.000000 quisk-4.2.8/afedrinet/sdr_control.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)     1368 2020-11-30 17:32:20.000000 quisk-4.2.8/afedrinet/setup.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)      383 2019-11-09 18:50:03.000000 quisk-4.2.8/afedrinet/test.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)   146628 2022-09-11 19:13:27.000000 quisk-4.2.8/configure.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)      835 2015-04-30 19:09:49.000000 quisk-4.2.8/defaults.html
--rwxrwxrwx   0 jim       (1000) jim       (1000)    62821 2022-09-30 14:46:27.000000 quisk-4.2.8/docs.html
--rwxrwxrwx   0 jim       (1000) jim       (1000)     3882 2020-02-24 19:03:52.000000 quisk-4.2.8/dxcluster.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)     1847 2014-05-30 17:23:01.000000 quisk-4.2.8/extdemod.c
--rwxrwxrwx   0 jim       (1000) jim       (1000)    16225 2022-06-25 13:22:32.000000 quisk-4.2.8/filter.c
--rwxrwxrwx   0 jim       (1000) jim       (1000)     3879 2022-06-25 13:27:48.000000 quisk-4.2.8/filter.h
--rwxrwxrwx   0 jim       (1000) jim       (1000)   151504 2022-06-22 16:35:27.000000 quisk-4.2.8/filters.h
--rwxrwxrwx   0 jim       (1000) jim       (1000)    98898 2018-11-21 21:45:42.000000 quisk-4.2.8/filters.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)    23718 2021-05-29 17:39:40.000000 quisk-4.2.8/freedv.c
--rwxrwxrwx   0 jim       (1000) jim       (1000)      429 2021-05-29 17:40:42.000000 quisk-4.2.8/freedv.h
-drwxrwxrwx   0 jim       (1000) jim       (1000)        0 2022-09-30 15:26:32.620782 quisk-4.2.8/freedvpkg/
--rwxrwxrwx   0 jim       (1000) jim       (1000)     5651 2020-07-01 11:44:54.000000 quisk-4.2.8/freedvpkg/README.txt
--rwxrwxrwx   0 jim       (1000) jim       (1000)        2 2018-10-06 20:55:49.000000 quisk-4.2.8/freedvpkg/__init__.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)   875574 2020-06-05 16:16:20.000000 quisk-4.2.8/freedvpkg/libcodec2_32.dll
--rwxrwxrwx   0 jim       (1000) jim       (1000)   579488 2020-06-05 16:19:55.000000 quisk-4.2.8/freedvpkg/libcodec2_32.so
--rwxrwxrwx   0 jim       (1000) jim       (1000)  1052823 2020-06-05 16:17:02.000000 quisk-4.2.8/freedvpkg/libcodec2_64.dll
--rwxrwxrwx   0 jim       (1000) jim       (1000)   663848 2020-06-05 16:20:10.000000 quisk-4.2.8/freedvpkg/libcodec2_64.so
--rwxrwxrwx   0 jim       (1000) jim       (1000)    26954 2022-08-13 13:46:07.000000 quisk-4.2.8/help.html
--rwxrwxrwx   0 jim       (1000) jim       (1000)     7051 2018-10-09 13:22:13.000000 quisk-4.2.8/help_conf.html
--rwxrwxrwx   0 jim       (1000) jim       (1000)     7039 2016-12-08 22:49:26.000000 quisk-4.2.8/help_vna.html
-drwxrwxrwx   0 jim       (1000) jim       (1000)        0 2022-09-30 15:26:32.627010 quisk-4.2.8/hermes/
--rwxrwxrwx   0 jim       (1000) jim       (1000)     2981 2018-02-07 14:45:14.000000 quisk-4.2.8/hermes/README.txt
--rwxrwxrwx   0 jim       (1000) jim       (1000)        2 2015-06-22 16:17:58.000000 quisk-4.2.8/hermes/__init__.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)       88 2018-01-31 20:22:44.000000 quisk-4.2.8/hermes/quisk_conf.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)       88 2018-01-31 20:41:39.000000 quisk-4.2.8/hermes/quisk_conf2.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)    47595 2022-08-21 12:48:00.000000 quisk-4.2.8/hermes/quisk_hardware.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)     7076 2022-08-18 17:06:55.000000 quisk-4.2.8/hermes/quisk_widgets.py
-drwxrwxrwx   0 jim       (1000) jim       (1000)        0 2022-09-30 15:26:32.628399 quisk-4.2.8/hiqsdr/
--rwxrwxrwx   0 jim       (1000) jim       (1000)        2 2011-09-09 11:12:24.000000 quisk-4.2.8/hiqsdr/__init__.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)     1155 2018-11-26 17:49:15.000000 quisk-4.2.8/hiqsdr/quisk_conf.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)    17310 2020-06-08 13:24:46.000000 quisk-4.2.8/hiqsdr/quisk_hardware.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)     2760 2012-03-03 16:06:44.000000 quisk-4.2.8/import_quisk_api.c
--rwxrwxrwx   0 jim       (1000) jim       (1000)     6371 2021-10-13 18:32:35.000000 quisk-4.2.8/is_key_down.c
--rwxrwxrwx   0 jim       (1000) jim       (1000)  2310215 2022-09-30 15:11:23.000000 quisk-4.2.8/libfftw3-3.dll
--rwxrwxrwx   0 jim       (1000) jim       (1000)   124020 2022-09-30 15:11:23.000000 quisk-4.2.8/libgcc_s_dw2-1.dll
--rwxrwxrwx   0 jim       (1000) jim       (1000)     1369 2011-09-09 11:12:18.000000 quisk-4.2.8/libusb.txt
--rwxrwxrwx   0 jim       (1000) jim       (1000)  1633363 2022-04-07 17:55:14.000000 quisk-4.2.8/libwdsp.dll
--rwxrwxrwx   0 jim       (1000) jim       (1000)    63502 2022-09-30 15:11:23.000000 quisk-4.2.8/libwinpthread-1.dll
--rwxrwxrwx   0 jim       (1000) jim       (1000)    17908 2020-08-13 12:21:09.000000 quisk-4.2.8/license.txt
--rwxrwxrwx   0 jim       (1000) jim       (1000)      464 2020-12-21 12:03:03.000000 quisk-4.2.8/makefile
--rwxrwxrwx   0 jim       (1000) jim       (1000)    54987 2022-05-20 20:22:23.000000 quisk-4.2.8/microphone.c
--rwxrwxrwx   0 jim       (1000) jim       (1000)       36 2011-12-09 11:48:24.000000 quisk-4.2.8/microphone.h
--rwxrwxrwx   0 jim       (1000) jim       (1000)     6719 2022-09-29 14:45:13.000000 quisk-4.2.8/midi_handler.py
-drwxrwxrwx   0 jim       (1000) jim       (1000)        0 2022-09-30 15:26:32.665169 quisk-4.2.8/n2adr/
--rwxrwxrwx   0 jim       (1000) jim       (1000)     1718 2019-04-22 16:18:43.000000 quisk-4.2.8/n2adr/.quisk_init.pkl
--rwxrwxrwx   0 jim       (1000) jim       (1000)        2 2011-09-09 11:12:20.000000 quisk-4.2.8/n2adr/__init__.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)      480 2015-10-20 14:41:12.000000 quisk-4.2.8/n2adr/conf1.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)      709 2015-10-27 18:07:45.000000 quisk-4.2.8/n2adr/conf2.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)      459 2015-10-20 14:40:29.000000 quisk-4.2.8/n2adr/conf3.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)       93 2015-10-20 14:43:30.000000 quisk-4.2.8/n2adr/conf3A.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)     1237 2020-05-23 21:26:11.000000 quisk-4.2.8/n2adr/conf4.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)      434 2015-10-20 14:39:31.000000 quisk-4.2.8/n2adr/conf5.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)      891 2020-07-30 12:34:50.000000 quisk-4.2.8/n2adr/conf6.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)      285 2015-10-20 14:40:06.000000 quisk-4.2.8/n2adr/conf7.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)     2527 2020-09-15 12:53:34.000000 quisk-4.2.8/n2adr/hl2_hardware.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)     1676 2019-04-04 13:41:57.000000 quisk-4.2.8/n2adr/quisk_conf.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)     7456 2018-11-26 18:54:20.000000 quisk-4.2.8/n2adr/quisk_conf_8600.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)     3298 2022-05-12 15:36:18.000000 quisk-4.2.8/n2adr/quisk_hardware.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)     2503 2018-11-27 22:16:39.000000 quisk-4.2.8/n2adr/quisk_widgets.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)     5429 2018-11-27 22:16:50.000000 quisk-4.2.8/n2adr/scanner_widgets.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)     3226 2015-08-25 17:43:27.000000 quisk-4.2.8/n2adr/startup.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)    36864 2022-05-23 21:01:01.000000 quisk-4.2.8/n2adr/station_hardware.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)     2218 2019-04-22 17:12:54.000000 quisk-4.2.8/n2adr/uhf_conf.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)    21104 2022-05-27 18:43:27.000000 quisk-4.2.8/n2adr/uhf_hardware.old
--rwxrwxrwx   0 jim       (1000) jim       (1000)    21700 2022-05-28 15:14:37.000000 quisk-4.2.8/n2adr/uhf_hardware.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)     6172 2019-04-22 16:28:26.000000 quisk-4.2.8/n2adr/uhf_widgets.py
-drwxrwxrwx   0 jim       (1000) jim       (1000)        0 2022-09-30 15:26:32.666727 quisk-4.2.8/perseuspkg/
--rwxrwxrwx   0 jim       (1000) jim       (1000)      201 2020-03-28 21:12:37.000000 quisk-4.2.8/perseuspkg/README.txt
--rwxrwxrwx   0 jim       (1000) jim       (1000)        2 2020-03-28 21:12:37.000000 quisk-4.2.8/perseuspkg/__init__.py
-drwxrwxrwx   0 jim       (1000) jim       (1000)        0 2022-09-30 15:26:32.667711 quisk-4.2.8/perseuspkg/build/
--rwxrwxrwx   0 jim       (1000) jim       (1000)    29784 2020-12-21 12:01:53.000000 quisk-4.2.8/perseuspkg/build/import_quisk_api.o
--rwxrwxrwx   0 jim       (1000) jim       (1000)      115 2020-03-28 21:12:37.000000 quisk-4.2.8/perseuspkg/makefile
--rwxrwxrwx   0 jim       (1000) jim       (1000)    14184 2020-05-22 12:19:47.000000 quisk-4.2.8/perseuspkg/perseus.c
--rwxrwxrwx   0 jim       (1000) jim       (1000)     6054 2020-05-22 12:19:47.000000 quisk-4.2.8/perseuspkg/quisk_hardware.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)     1438 2020-03-28 21:12:37.000000 quisk-4.2.8/perseuspkg/quisk_widgets.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)     1386 2020-03-28 21:12:37.000000 quisk-4.2.8/perseuspkg/setup.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)       33 2018-03-19 15:12:25.000000 quisk-4.2.8/plot_wxmplot.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)     2911 2018-11-26 19:19:45.000000 quisk-4.2.8/portaudio.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)      180 2020-12-01 18:06:12.000000 quisk-4.2.8/quisk
--rwxrwxrwx   0 jim       (1000) jim       (1000)   203658 2022-09-04 13:05:08.000000 quisk-4.2.8/quisk.c
-drwxrwxrwx   0 jim       (1000) jim       (1000)        0 2022-09-30 15:26:32.670382 quisk-4.2.8/quisk.egg-info/
--rwxrwxrwx   0 jim       (1000) jim       (1000)     1571 2022-09-30 15:26:32.000000 quisk-4.2.8/quisk.egg-info/PKG-INFO
--rwxrwxrwx   0 jim       (1000) jim       (1000)     5929 2022-09-30 15:26:32.000000 quisk-4.2.8/quisk.egg-info/SOURCES.txt
--rwxrwxrwx   0 jim       (1000) jim       (1000)        1 2022-09-30 15:26:32.000000 quisk-4.2.8/quisk.egg-info/dependency_links.txt
--rwxrwxrwx   0 jim       (1000) jim       (1000)       73 2022-09-30 15:26:32.000000 quisk-4.2.8/quisk.egg-info/entry_points.txt
--rwxrwxrwx   0 jim       (1000) jim       (1000)       15 2022-09-30 15:26:32.000000 quisk-4.2.8/quisk.egg-info/requires.txt
--rwxrwxrwx   0 jim       (1000) jim       (1000)        6 2022-09-30 15:26:32.000000 quisk-4.2.8/quisk.egg-info/top_level.txt
--rwxrwxrwx   0 jim       (1000) jim       (1000)    22335 2022-09-03 20:43:50.000000 quisk-4.2.8/quisk.h
--rwxrwxrwx   0 jim       (1000) jim       (1000)   270744 2022-09-22 19:11:52.000000 quisk-4.2.8/quisk.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)    99748 2022-09-14 16:26:42.000000 quisk-4.2.8/quisk_conf_defaults.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)     1353 2020-05-22 14:55:47.000000 quisk-4.2.8/quisk_conf_kx3.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)     1230 2014-05-25 21:04:10.000000 quisk-4.2.8/quisk_conf_model.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)     3890 2020-01-15 14:27:34.000000 quisk-4.2.8/quisk_conf_openradio.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)      384 2018-11-24 21:17:03.000000 quisk-4.2.8/quisk_conf_peaberry.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)     1332 2018-11-24 22:27:12.000000 quisk-4.2.8/quisk_conf_sdr8600.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)     1479 2019-08-20 13:00:58.000000 quisk-4.2.8/quisk_conf_sdriq.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)     2900 2011-09-09 11:12:20.000000 quisk-4.2.8/quisk_conf_win.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)     1042 2018-11-24 21:18:11.000000 quisk-4.2.8/quisk_hardware_fixed.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)     6049 2021-02-12 14:25:51.000000 quisk-4.2.8/quisk_hardware_hamlib.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)     2176 2021-09-01 19:09:12.000000 quisk-4.2.8/quisk_hardware_hl2_oob.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)     9069 2022-08-24 20:46:55.000000 quisk-4.2.8/quisk_hardware_model.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)     2953 2019-08-20 13:08:11.000000 quisk-4.2.8/quisk_hardware_sdr8600.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)    21911 2022-08-06 18:15:41.000000 quisk-4.2.8/quisk_hardware_sdriq.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)     2589 2022-08-06 18:19:29.000000 quisk-4.2.8/quisk_utils.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)    54238 2021-09-12 13:19:59.000000 quisk-4.2.8/quisk_vna.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)     2953 2022-01-04 17:07:57.000000 quisk-4.2.8/quisk_wdsp.c
--rwxrwxrwx   0 jim       (1000) jim       (1000)     3922 2022-03-18 19:57:03.000000 quisk-4.2.8/quisk_wdsp.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)    57429 2022-09-29 14:32:00.000000 quisk-4.2.8/quisk_widgets.py
-drwxrwxrwx   0 jim       (1000) jim       (1000)        0 2022-09-30 15:26:32.673412 quisk-4.2.8/sdriqpkg/
--rwxrwxrwx   0 jim       (1000) jim       (1000)      177 2019-08-20 17:40:20.000000 quisk-4.2.8/sdriqpkg/README.txt
--rwxrwxrwx   0 jim       (1000) jim       (1000)        2 2011-09-09 11:12:24.000000 quisk-4.2.8/sdriqpkg/__init__.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)     3039 2018-11-26 17:46:05.000000 quisk-4.2.8/sdriqpkg/quisk_hardware.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)    24258 2019-09-22 18:42:30.000000 quisk-4.2.8/sdriqpkg/sdriq.c
--rwxrwxrwx   0 jim       (1000) jim       (1000)     7235 2011-09-09 11:12:24.000000 quisk-4.2.8/sdriqpkg/sdriq.h
--rwxrwxrwx   0 jim       (1000) jim       (1000)    27136 2020-11-30 20:04:41.000000 quisk-4.2.8/sdriqpkg/sdriq.pyd
-drwxrwxrwx   0 jim       (1000) jim       (1000)        0 2022-09-30 15:26:32.643509 quisk-4.2.8/sdrmicronpkg/
--rwxrwxrwx   0 jim       (1000) jim       (1000)        2 2020-04-03 12:11:52.000000 quisk-4.2.8/sdrmicronpkg/__init__.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)     9400 2020-04-04 11:52:12.000000 quisk-4.2.8/sdrmicronpkg/quisk_hardware.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)       38 2022-09-30 15:26:32.681508 quisk-4.2.8/setup.cfg
--rwxrwxrwx   0 jim       (1000) jim       (1000)     4563 2022-09-23 17:24:12.000000 quisk-4.2.8/setup.py
-drwxrwxrwx   0 jim       (1000) jim       (1000)        0 2022-09-30 15:26:32.675856 quisk-4.2.8/soapypkg/
--rwxrwxrwx   0 jim       (1000) jim       (1000)        2 2019-01-25 17:54:17.000000 quisk-4.2.8/soapypkg/__init__.py
-drwxrwxrwx   0 jim       (1000) jim       (1000)        0 2022-09-30 15:26:32.676603 quisk-4.2.8/soapypkg/build/
--rwxrwxrwx   0 jim       (1000) jim       (1000)    34320 2020-12-20 17:43:51.000000 quisk-4.2.8/soapypkg/build/import_quisk_api.o
-drwxrwxrwx   0 jim       (1000) jim       (1000)        0 2022-09-30 15:26:32.677510 quisk-4.2.8/soapypkg/build/temp.linux-x86_64-2.7/
--rwxrwxrwx   0 jim       (1000) jim       (1000)    67824 2020-11-11 18:29:04.000000 quisk-4.2.8/soapypkg/build/temp.linux-x86_64-2.7/soapy.o
-drwxrwxrwx   0 jim       (1000) jim       (1000)        0 2022-09-30 15:26:32.678764 quisk-4.2.8/soapypkg/build/temp.linux-x86_64-3.6/
--rwxrwxrwx   0 jim       (1000) jim       (1000)    92232 2020-12-20 17:43:51.000000 quisk-4.2.8/soapypkg/build/temp.linux-x86_64-3.6/soapy.o
-drwxrwxrwx   0 jim       (1000) jim       (1000)        0 2022-09-30 15:26:32.679889 quisk-4.2.8/soapypkg/build/temp.win32-2.7/
--rwxrwxrwx   0 jim       (1000) jim       (1000)     1135 2019-07-30 17:59:19.000000 quisk-4.2.8/soapypkg/build/temp.win32-2.7/import_quisk_api.o
--rwxrwxrwx   0 jim       (1000) jim       (1000)      111 2019-11-21 22:44:24.000000 quisk-4.2.8/soapypkg/makefile
--rwxrwxrwx   0 jim       (1000) jim       (1000)     6563 2021-07-15 17:57:39.000000 quisk-4.2.8/soapypkg/quisk_hardware.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)     1550 2019-02-19 18:20:47.000000 quisk-4.2.8/soapypkg/setup.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)    17058 2021-01-02 17:43:04.000000 quisk-4.2.8/soapypkg/soapy.c
--rwxrwxrwx   0 jim       (1000) jim       (1000)    26112 2022-09-05 17:24:08.000000 quisk-4.2.8/soapypkg/soapy.pyd
-drwxrwxrwx   0 jim       (1000) jim       (1000)        0 2022-09-30 15:26:32.647816 quisk-4.2.8/softrock/
--rwxrwxrwx   0 jim       (1000) jim       (1000)        2 2011-09-09 11:12:24.000000 quisk-4.2.8/softrock/__init__.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)     3286 2021-01-20 19:30:36.000000 quisk-4.2.8/softrock/hardware_net.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)    11256 2022-08-13 13:49:49.000000 quisk-4.2.8/softrock/hardware_usb.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)      531 2021-01-20 19:30:58.000000 quisk-4.2.8/softrock/widgets_tx.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)      846 2019-12-19 14:23:24.000000 quisk-4.2.8/softrock_tune_vfo.py
--rwxrwxrwx   0 jim       (1000) jim       (1000)    55130 2022-08-26 19:05:15.000000 quisk-4.2.8/sound.c
--rwxrwxrwx   0 jim       (1000) jim       (1000)    42656 2022-02-18 15:29:28.000000 quisk-4.2.8/sound_alsa.c
--rwxrwxrwx   0 jim       (1000) jim       (1000)    23140 2021-02-19 13:56:21.000000 quisk-4.2.8/sound_directx.c
--rwxrwxrwx   0 jim       (1000) jim       (1000)    17299 2021-05-13 12:20:57.000000 quisk-4.2.8/sound_portaudio.c
--rwxrwxrwx   0 jim       (1000) jim       (1000)    35540 2021-09-30 13:00:35.000000 quisk-4.2.8/sound_pulseaudio.c
--rwxrwxrwx   0 jim       (1000) jim       (1000)    47735 2022-02-18 16:18:09.000000 quisk-4.2.8/sound_wasapi.c
--rwxrwxrwx   0 jim       (1000) jim       (1000)     8563 2022-09-03 20:56:01.000000 quisk-4.2.8/utility.c
--rwxrwxrwx   0 jim       (1000) jim       (1000)      773 2011-09-09 11:12:18.000000 quisk-4.2.8/windows.txt
--rwxrwxrwx   0 jim       (1000) jim       (1000)      717 2011-09-09 11:12:20.000000 quisk-4.2.8/winsound.txt
+drwxrwxrwx   0 jim       (1000) jim       (1000)        0 2022-10-05 16:46:56.534555 quisk-4.2.9/
+-rwxrwxrwx   0 jim       (1000) jim       (1000)   101006 2022-10-04 17:03:32.000000 quisk-4.2.9/CHANGELOG.txt
+-rwxrwxrwx   0 jim       (1000) jim       (1000)       52 2011-09-09 11:12:18.000000 quisk-4.2.9/Extensions.txt
+-rwxrwxrwx   0 jim       (1000) jim       (1000)      287 2022-08-15 19:42:43.000000 quisk-4.2.9/MANIFEST.in
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     1571 2022-10-05 16:46:56.534372 quisk-4.2.9/PKG-INFO
+-rwxrwxrwx   0 jim       (1000) jim       (1000)       52 2011-09-09 11:12:20.000000 quisk-4.2.9/README.txt
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     2300 2018-11-23 19:45:24.000000 quisk-4.2.9/WinEdit.pyw
+-rwxrwxrwx   0 jim       (1000) jim       (1000)      176 2018-11-23 19:45:24.000000 quisk-4.2.9/WinQuisk.pyw
+-rwxrwxrwx   0 jim       (1000) jim       (1000)      213 2018-11-23 19:45:24.000000 quisk-4.2.9/WinQuiskVna.pyw
+-rwxrwxrwx   0 jim       (1000) jim       (1000)       45 2022-10-05 16:46:56.000000 quisk-4.2.9/__init__.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)      177 2019-11-23 21:29:34.000000 quisk-4.2.9/__main__.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)   257024 2022-09-05 17:24:06.000000 quisk-4.2.9/_quisk.pyd
+drwxrwxrwx   0 jim       (1000) jim       (1000)        0 2022-10-05 16:46:56.506294 quisk-4.2.9/ac2yd/
+-rwxrwxrwx   0 jim       (1000) jim       (1000)   371367 2022-08-14 16:18:32.000000 quisk-4.2.9/ac2yd/Design_2022_0531.pdf
+-rwxrwxrwx   0 jim       (1000) jim       (1000)        2 2022-08-30 20:10:29.000000 quisk-4.2.9/ac2yd/__init__.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)    16152 2022-10-03 16:43:26.000000 quisk-4.2.9/ac2yd/control_common.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     1919 2022-10-03 16:55:39.000000 quisk-4.2.9/ac2yd/control_hermes.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)      347 2022-08-24 20:42:19.000000 quisk-4.2.9/ac2yd/control_softrock.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)    29580 2022-09-30 15:10:14.000000 quisk-4.2.9/ac2yd/remote.c
+-rwxrwxrwx   0 jim       (1000) jim       (1000)    16977 2022-10-04 17:07:01.000000 quisk-4.2.9/ac2yd/remote_common.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)      841 2022-09-15 20:06:21.000000 quisk-4.2.9/ac2yd/remote_hermes.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)      554 2022-09-15 20:16:05.000000 quisk-4.2.9/ac2yd/remote_softrock.py
+drwxrwxrwx   0 jim       (1000) jim       (1000)        0 2022-10-05 16:46:56.509943 quisk-4.2.9/afedrinet/
+-rwxrwxrwx   0 jim       (1000) jim       (1000)      173 2019-01-26 19:28:41.000000 quisk-4.2.9/afedrinet/SOURCE.txt
+-rwxrwxrwx   0 jim       (1000) jim       (1000)        2 2014-12-10 16:01:00.000000 quisk-4.2.9/afedrinet/__init__.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)      183 2014-12-10 16:01:00.000000 quisk-4.2.9/afedrinet/af_comp.bat.makeit
+-rwxrwxrwx   0 jim       (1000) jim       (1000)      313 2016-04-14 00:44:28.000000 quisk-4.2.9/afedrinet/afe_library
+-rwxrwxrwx   0 jim       (1000) jim       (1000)      518 2015-12-13 16:29:58.000000 quisk-4.2.9/afedrinet/afe_library.mac
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     8526 2020-01-09 18:56:17.000000 quisk-4.2.9/afedrinet/afedri.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)    11632 2019-09-22 18:48:57.000000 quisk-4.2.9/afedrinet/afedrinet_io.c
+-rwxrwxrwx   0 jim       (1000) jim       (1000)    21504 2022-09-05 17:24:07.000000 quisk-4.2.9/afedrinet/afedrinet_io.pyd
+drwxrwxrwx   0 jim       (1000) jim       (1000)        0 2022-10-05 16:46:56.512354 quisk-4.2.9/afedrinet/build/
+-rwxrwxrwx   0 jim       (1000) jim       (1000)    34320 2020-12-20 17:44:14.000000 quisk-4.2.9/afedrinet/build/import_quisk_api.o
+-rwxrwxrwx   0 jim       (1000) jim       (1000)    52640 2020-12-20 17:44:14.000000 quisk-4.2.9/afedrinet/build/is_key_down.o
+drwxrwxrwx   0 jim       (1000) jim       (1000)        0 2022-10-05 16:46:56.513489 quisk-4.2.9/afedrinet/build/temp.linux-x86_64-3.6/
+-rwxrwxrwx   0 jim       (1000) jim       (1000)    67672 2020-12-20 17:44:14.000000 quisk-4.2.9/afedrinet/build/temp.linux-x86_64-3.6/afedrinet_io.o
+-rwxrwxrwx   0 jim       (1000) jim       (1000)      119 2020-11-30 16:57:37.000000 quisk-4.2.9/afedrinet/makefile
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     3676 2015-11-22 23:00:54.000000 quisk-4.2.9/afedrinet/quisk_conf.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     3600 2015-12-10 15:25:14.000000 quisk-4.2.9/afedrinet/quisk_conf_linux.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     3600 2015-12-10 15:25:14.000000 quisk-4.2.9/afedrinet/quisk_conf_mac.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     3370 2020-05-23 21:28:44.000000 quisk-4.2.9/afedrinet/quisk_hardware.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     2645 2015-12-13 21:10:59.000000 quisk-4.2.9/afedrinet/readme.txt
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     1222 2020-01-09 18:03:05.000000 quisk-4.2.9/afedrinet/sdr_control.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     1368 2020-11-30 17:32:20.000000 quisk-4.2.9/afedrinet/setup.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)      383 2019-11-09 18:50:03.000000 quisk-4.2.9/afedrinet/test.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)   146628 2022-09-11 19:13:27.000000 quisk-4.2.9/configure.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)      835 2015-04-30 19:09:49.000000 quisk-4.2.9/defaults.html
+-rwxrwxrwx   0 jim       (1000) jim       (1000)    62821 2022-09-30 14:46:27.000000 quisk-4.2.9/docs.html
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     3882 2020-02-24 19:03:52.000000 quisk-4.2.9/dxcluster.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     1847 2014-05-30 17:23:01.000000 quisk-4.2.9/extdemod.c
+-rwxrwxrwx   0 jim       (1000) jim       (1000)    16225 2022-06-25 13:22:32.000000 quisk-4.2.9/filter.c
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     3879 2022-06-25 13:27:48.000000 quisk-4.2.9/filter.h
+-rwxrwxrwx   0 jim       (1000) jim       (1000)   151504 2022-06-22 16:35:27.000000 quisk-4.2.9/filters.h
+-rwxrwxrwx   0 jim       (1000) jim       (1000)    98898 2018-11-21 21:45:42.000000 quisk-4.2.9/filters.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)    23718 2021-05-29 17:39:40.000000 quisk-4.2.9/freedv.c
+-rwxrwxrwx   0 jim       (1000) jim       (1000)      429 2021-05-29 17:40:42.000000 quisk-4.2.9/freedv.h
+drwxrwxrwx   0 jim       (1000) jim       (1000)        0 2022-10-05 16:46:56.477363 quisk-4.2.9/freedvpkg/
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     5651 2020-07-01 11:44:54.000000 quisk-4.2.9/freedvpkg/README.txt
+-rwxrwxrwx   0 jim       (1000) jim       (1000)        2 2018-10-06 20:55:49.000000 quisk-4.2.9/freedvpkg/__init__.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)   875574 2020-06-05 16:16:20.000000 quisk-4.2.9/freedvpkg/libcodec2_32.dll
+-rwxrwxrwx   0 jim       (1000) jim       (1000)   579488 2020-06-05 16:19:55.000000 quisk-4.2.9/freedvpkg/libcodec2_32.so
+-rwxrwxrwx   0 jim       (1000) jim       (1000)  1052823 2020-06-05 16:17:02.000000 quisk-4.2.9/freedvpkg/libcodec2_64.dll
+-rwxrwxrwx   0 jim       (1000) jim       (1000)   663848 2020-06-05 16:20:10.000000 quisk-4.2.9/freedvpkg/libcodec2_64.so
+-rwxrwxrwx   0 jim       (1000) jim       (1000)    26954 2022-08-13 13:46:07.000000 quisk-4.2.9/help.html
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     7051 2018-10-09 13:22:13.000000 quisk-4.2.9/help_conf.html
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     7039 2016-12-08 22:49:26.000000 quisk-4.2.9/help_vna.html
+drwxrwxrwx   0 jim       (1000) jim       (1000)        0 2022-10-05 16:46:56.483627 quisk-4.2.9/hermes/
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     2981 2018-02-07 14:45:14.000000 quisk-4.2.9/hermes/README.txt
+-rwxrwxrwx   0 jim       (1000) jim       (1000)        2 2015-06-22 16:17:58.000000 quisk-4.2.9/hermes/__init__.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)       88 2018-01-31 20:22:44.000000 quisk-4.2.9/hermes/quisk_conf.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)       88 2018-01-31 20:41:39.000000 quisk-4.2.9/hermes/quisk_conf2.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)    47595 2022-08-21 12:48:00.000000 quisk-4.2.9/hermes/quisk_hardware.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     7076 2022-08-18 17:06:55.000000 quisk-4.2.9/hermes/quisk_widgets.py
+drwxrwxrwx   0 jim       (1000) jim       (1000)        0 2022-10-05 16:46:56.485015 quisk-4.2.9/hiqsdr/
+-rwxrwxrwx   0 jim       (1000) jim       (1000)        2 2011-09-09 11:12:24.000000 quisk-4.2.9/hiqsdr/__init__.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     1155 2018-11-26 17:49:15.000000 quisk-4.2.9/hiqsdr/quisk_conf.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)    17310 2020-06-08 13:24:46.000000 quisk-4.2.9/hiqsdr/quisk_hardware.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     2760 2012-03-03 16:06:44.000000 quisk-4.2.9/import_quisk_api.c
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     6371 2021-10-13 18:32:35.000000 quisk-4.2.9/is_key_down.c
+-rwxrwxrwx   0 jim       (1000) jim       (1000)  2310215 2022-10-05 16:33:48.000000 quisk-4.2.9/libfftw3-3.dll
+-rwxrwxrwx   0 jim       (1000) jim       (1000)   124020 2022-10-05 16:33:48.000000 quisk-4.2.9/libgcc_s_dw2-1.dll
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     1369 2011-09-09 11:12:18.000000 quisk-4.2.9/libusb.txt
+-rwxrwxrwx   0 jim       (1000) jim       (1000)  1633363 2022-04-07 17:55:14.000000 quisk-4.2.9/libwdsp.dll
+-rwxrwxrwx   0 jim       (1000) jim       (1000)    63502 2022-10-05 16:33:48.000000 quisk-4.2.9/libwinpthread-1.dll
+-rwxrwxrwx   0 jim       (1000) jim       (1000)    17908 2020-08-13 12:21:09.000000 quisk-4.2.9/license.txt
+-rwxrwxrwx   0 jim       (1000) jim       (1000)      464 2020-12-21 12:03:03.000000 quisk-4.2.9/makefile
+-rwxrwxrwx   0 jim       (1000) jim       (1000)    54987 2022-05-20 20:22:23.000000 quisk-4.2.9/microphone.c
+-rwxrwxrwx   0 jim       (1000) jim       (1000)       36 2011-12-09 11:48:24.000000 quisk-4.2.9/microphone.h
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     6719 2022-09-29 14:45:13.000000 quisk-4.2.9/midi_handler.py
+drwxrwxrwx   0 jim       (1000) jim       (1000)        0 2022-10-05 16:46:56.519321 quisk-4.2.9/n2adr/
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     1718 2019-04-22 16:18:43.000000 quisk-4.2.9/n2adr/.quisk_init.pkl
+-rwxrwxrwx   0 jim       (1000) jim       (1000)        2 2011-09-09 11:12:20.000000 quisk-4.2.9/n2adr/__init__.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)      480 2015-10-20 14:41:12.000000 quisk-4.2.9/n2adr/conf1.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)      709 2015-10-27 18:07:45.000000 quisk-4.2.9/n2adr/conf2.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)      459 2015-10-20 14:40:29.000000 quisk-4.2.9/n2adr/conf3.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)       93 2015-10-20 14:43:30.000000 quisk-4.2.9/n2adr/conf3A.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     1237 2020-05-23 21:26:11.000000 quisk-4.2.9/n2adr/conf4.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)      434 2015-10-20 14:39:31.000000 quisk-4.2.9/n2adr/conf5.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)      891 2020-07-30 12:34:50.000000 quisk-4.2.9/n2adr/conf6.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)      285 2015-10-20 14:40:06.000000 quisk-4.2.9/n2adr/conf7.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     2527 2020-09-15 12:53:34.000000 quisk-4.2.9/n2adr/hl2_hardware.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     1676 2019-04-04 13:41:57.000000 quisk-4.2.9/n2adr/quisk_conf.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     7456 2018-11-26 18:54:20.000000 quisk-4.2.9/n2adr/quisk_conf_8600.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     3298 2022-05-12 15:36:18.000000 quisk-4.2.9/n2adr/quisk_hardware.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     2503 2018-11-27 22:16:39.000000 quisk-4.2.9/n2adr/quisk_widgets.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     5429 2018-11-27 22:16:50.000000 quisk-4.2.9/n2adr/scanner_widgets.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     3226 2015-08-25 17:43:27.000000 quisk-4.2.9/n2adr/startup.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)    36864 2022-05-23 21:01:01.000000 quisk-4.2.9/n2adr/station_hardware.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     2218 2019-04-22 17:12:54.000000 quisk-4.2.9/n2adr/uhf_conf.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)    21104 2022-05-27 18:43:27.000000 quisk-4.2.9/n2adr/uhf_hardware.old
+-rwxrwxrwx   0 jim       (1000) jim       (1000)    21700 2022-05-28 15:14:37.000000 quisk-4.2.9/n2adr/uhf_hardware.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     6172 2019-04-22 16:28:26.000000 quisk-4.2.9/n2adr/uhf_widgets.py
+drwxrwxrwx   0 jim       (1000) jim       (1000)        0 2022-10-05 16:46:56.520767 quisk-4.2.9/perseuspkg/
+-rwxrwxrwx   0 jim       (1000) jim       (1000)      201 2020-03-28 21:12:37.000000 quisk-4.2.9/perseuspkg/README.txt
+-rwxrwxrwx   0 jim       (1000) jim       (1000)        2 2020-03-28 21:12:37.000000 quisk-4.2.9/perseuspkg/__init__.py
+drwxrwxrwx   0 jim       (1000) jim       (1000)        0 2022-10-05 16:46:56.521690 quisk-4.2.9/perseuspkg/build/
+-rwxrwxrwx   0 jim       (1000) jim       (1000)    29784 2020-12-21 12:01:53.000000 quisk-4.2.9/perseuspkg/build/import_quisk_api.o
+-rwxrwxrwx   0 jim       (1000) jim       (1000)      115 2020-03-28 21:12:37.000000 quisk-4.2.9/perseuspkg/makefile
+-rwxrwxrwx   0 jim       (1000) jim       (1000)    14184 2020-05-22 12:19:47.000000 quisk-4.2.9/perseuspkg/perseus.c
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     6054 2020-05-22 12:19:47.000000 quisk-4.2.9/perseuspkg/quisk_hardware.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     1438 2020-03-28 21:12:37.000000 quisk-4.2.9/perseuspkg/quisk_widgets.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     1386 2020-03-28 21:12:37.000000 quisk-4.2.9/perseuspkg/setup.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)       33 2018-03-19 15:12:25.000000 quisk-4.2.9/plot_wxmplot.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     2911 2018-11-26 19:19:45.000000 quisk-4.2.9/portaudio.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)      180 2020-12-01 18:06:12.000000 quisk-4.2.9/quisk
+-rwxrwxrwx   0 jim       (1000) jim       (1000)   203658 2022-09-04 13:05:08.000000 quisk-4.2.9/quisk.c
+drwxrwxrwx   0 jim       (1000) jim       (1000)        0 2022-10-05 16:46:56.524285 quisk-4.2.9/quisk.egg-info/
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     1571 2022-10-05 16:46:56.000000 quisk-4.2.9/quisk.egg-info/PKG-INFO
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     5929 2022-10-05 16:46:56.000000 quisk-4.2.9/quisk.egg-info/SOURCES.txt
+-rwxrwxrwx   0 jim       (1000) jim       (1000)        1 2022-10-05 16:46:56.000000 quisk-4.2.9/quisk.egg-info/dependency_links.txt
+-rwxrwxrwx   0 jim       (1000) jim       (1000)       73 2022-10-05 16:46:56.000000 quisk-4.2.9/quisk.egg-info/entry_points.txt
+-rwxrwxrwx   0 jim       (1000) jim       (1000)       15 2022-10-05 16:46:56.000000 quisk-4.2.9/quisk.egg-info/requires.txt
+-rwxrwxrwx   0 jim       (1000) jim       (1000)        6 2022-10-05 16:46:56.000000 quisk-4.2.9/quisk.egg-info/top_level.txt
+-rwxrwxrwx   0 jim       (1000) jim       (1000)    22335 2022-09-03 20:43:50.000000 quisk-4.2.9/quisk.h
+-rwxrwxrwx   0 jim       (1000) jim       (1000)   270791 2022-10-04 17:11:48.000000 quisk-4.2.9/quisk.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)    99748 2022-09-14 16:26:42.000000 quisk-4.2.9/quisk_conf_defaults.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     1353 2020-05-22 14:55:47.000000 quisk-4.2.9/quisk_conf_kx3.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     1230 2014-05-25 21:04:10.000000 quisk-4.2.9/quisk_conf_model.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     3890 2020-01-15 14:27:34.000000 quisk-4.2.9/quisk_conf_openradio.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)      384 2018-11-24 21:17:03.000000 quisk-4.2.9/quisk_conf_peaberry.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     1332 2018-11-24 22:27:12.000000 quisk-4.2.9/quisk_conf_sdr8600.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     1479 2019-08-20 13:00:58.000000 quisk-4.2.9/quisk_conf_sdriq.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     2900 2011-09-09 11:12:20.000000 quisk-4.2.9/quisk_conf_win.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     1042 2018-11-24 21:18:11.000000 quisk-4.2.9/quisk_hardware_fixed.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     6058 2022-10-02 18:15:44.000000 quisk-4.2.9/quisk_hardware_hamlib.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     2176 2021-09-01 19:09:12.000000 quisk-4.2.9/quisk_hardware_hl2_oob.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     9069 2022-08-24 20:46:55.000000 quisk-4.2.9/quisk_hardware_model.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     2953 2019-08-20 13:08:11.000000 quisk-4.2.9/quisk_hardware_sdr8600.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)    21911 2022-08-06 18:15:41.000000 quisk-4.2.9/quisk_hardware_sdriq.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     2589 2022-08-06 18:19:29.000000 quisk-4.2.9/quisk_utils.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)    54238 2021-09-12 13:19:59.000000 quisk-4.2.9/quisk_vna.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     2953 2022-01-04 17:07:57.000000 quisk-4.2.9/quisk_wdsp.c
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     3922 2022-03-18 19:57:03.000000 quisk-4.2.9/quisk_wdsp.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)    57429 2022-10-03 16:52:24.000000 quisk-4.2.9/quisk_widgets.py
+drwxrwxrwx   0 jim       (1000) jim       (1000)        0 2022-10-05 16:46:56.526954 quisk-4.2.9/sdriqpkg/
+-rwxrwxrwx   0 jim       (1000) jim       (1000)      177 2019-08-20 17:40:20.000000 quisk-4.2.9/sdriqpkg/README.txt
+-rwxrwxrwx   0 jim       (1000) jim       (1000)        2 2011-09-09 11:12:24.000000 quisk-4.2.9/sdriqpkg/__init__.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     3039 2018-11-26 17:46:05.000000 quisk-4.2.9/sdriqpkg/quisk_hardware.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)    24258 2019-09-22 18:42:30.000000 quisk-4.2.9/sdriqpkg/sdriq.c
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     7235 2011-09-09 11:12:24.000000 quisk-4.2.9/sdriqpkg/sdriq.h
+-rwxrwxrwx   0 jim       (1000) jim       (1000)    27136 2020-11-30 20:04:41.000000 quisk-4.2.9/sdriqpkg/sdriq.pyd
+drwxrwxrwx   0 jim       (1000) jim       (1000)        0 2022-10-05 16:46:56.499090 quisk-4.2.9/sdrmicronpkg/
+-rwxrwxrwx   0 jim       (1000) jim       (1000)        2 2020-04-03 12:11:52.000000 quisk-4.2.9/sdrmicronpkg/__init__.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     9400 2020-04-04 11:52:12.000000 quisk-4.2.9/sdrmicronpkg/quisk_hardware.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)       38 2022-10-05 16:46:56.534621 quisk-4.2.9/setup.cfg
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     4563 2022-09-30 15:31:34.000000 quisk-4.2.9/setup.py
+drwxrwxrwx   0 jim       (1000) jim       (1000)        0 2022-10-05 16:46:56.529199 quisk-4.2.9/soapypkg/
+-rwxrwxrwx   0 jim       (1000) jim       (1000)        2 2019-01-25 17:54:17.000000 quisk-4.2.9/soapypkg/__init__.py
+drwxrwxrwx   0 jim       (1000) jim       (1000)        0 2022-10-05 16:46:56.529860 quisk-4.2.9/soapypkg/build/
+-rwxrwxrwx   0 jim       (1000) jim       (1000)    34320 2020-12-20 17:43:51.000000 quisk-4.2.9/soapypkg/build/import_quisk_api.o
+drwxrwxrwx   0 jim       (1000) jim       (1000)        0 2022-10-05 16:46:56.530847 quisk-4.2.9/soapypkg/build/temp.linux-x86_64-2.7/
+-rwxrwxrwx   0 jim       (1000) jim       (1000)    67824 2020-11-11 18:29:04.000000 quisk-4.2.9/soapypkg/build/temp.linux-x86_64-2.7/soapy.o
+drwxrwxrwx   0 jim       (1000) jim       (1000)        0 2022-10-05 16:46:56.532094 quisk-4.2.9/soapypkg/build/temp.linux-x86_64-3.6/
+-rwxrwxrwx   0 jim       (1000) jim       (1000)    92232 2020-12-20 17:43:51.000000 quisk-4.2.9/soapypkg/build/temp.linux-x86_64-3.6/soapy.o
+drwxrwxrwx   0 jim       (1000) jim       (1000)        0 2022-10-05 16:46:56.533142 quisk-4.2.9/soapypkg/build/temp.win32-2.7/
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     1135 2019-07-30 17:59:19.000000 quisk-4.2.9/soapypkg/build/temp.win32-2.7/import_quisk_api.o
+-rwxrwxrwx   0 jim       (1000) jim       (1000)      111 2019-11-21 22:44:24.000000 quisk-4.2.9/soapypkg/makefile
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     6563 2021-07-15 17:57:39.000000 quisk-4.2.9/soapypkg/quisk_hardware.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     1550 2019-02-19 18:20:47.000000 quisk-4.2.9/soapypkg/setup.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)    17058 2021-01-02 17:43:04.000000 quisk-4.2.9/soapypkg/soapy.c
+-rwxrwxrwx   0 jim       (1000) jim       (1000)    26112 2022-09-05 17:24:08.000000 quisk-4.2.9/soapypkg/soapy.pyd
+drwxrwxrwx   0 jim       (1000) jim       (1000)        0 2022-10-05 16:46:56.503005 quisk-4.2.9/softrock/
+-rwxrwxrwx   0 jim       (1000) jim       (1000)        2 2011-09-09 11:12:24.000000 quisk-4.2.9/softrock/__init__.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     3286 2021-01-20 19:30:36.000000 quisk-4.2.9/softrock/hardware_net.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)    11256 2022-08-13 13:49:49.000000 quisk-4.2.9/softrock/hardware_usb.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)      531 2021-01-20 19:30:58.000000 quisk-4.2.9/softrock/widgets_tx.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)      846 2019-12-19 14:23:24.000000 quisk-4.2.9/softrock_tune_vfo.py
+-rwxrwxrwx   0 jim       (1000) jim       (1000)    55130 2022-08-26 19:05:15.000000 quisk-4.2.9/sound.c
+-rwxrwxrwx   0 jim       (1000) jim       (1000)    42656 2022-02-18 15:29:28.000000 quisk-4.2.9/sound_alsa.c
+-rwxrwxrwx   0 jim       (1000) jim       (1000)    23140 2021-02-19 13:56:21.000000 quisk-4.2.9/sound_directx.c
+-rwxrwxrwx   0 jim       (1000) jim       (1000)    17299 2021-05-13 12:20:57.000000 quisk-4.2.9/sound_portaudio.c
+-rwxrwxrwx   0 jim       (1000) jim       (1000)    35540 2021-09-30 13:00:35.000000 quisk-4.2.9/sound_pulseaudio.c
+-rwxrwxrwx   0 jim       (1000) jim       (1000)    47735 2022-02-18 16:18:09.000000 quisk-4.2.9/sound_wasapi.c
+-rwxrwxrwx   0 jim       (1000) jim       (1000)     8563 2022-09-03 20:56:01.000000 quisk-4.2.9/utility.c
+-rwxrwxrwx   0 jim       (1000) jim       (1000)      773 2011-09-09 11:12:18.000000 quisk-4.2.9/windows.txt
+-rwxrwxrwx   0 jim       (1000) jim       (1000)      717 2011-09-09 11:12:20.000000 quisk-4.2.9/winsound.txt
```

### Comparing `quisk-4.2.8/CHANGELOG.txt` & `quisk-4.2.9/CHANGELOG.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+Quisk Version 4.2.9  October 2022
+=================================
+This is an update to the new Quisk Remote feature by Ben, AC2YD. I fixed the problem with the favorites screen
+and the station buttons below the X-axis. I fixed the "Failure in OnFreedvMenu" bug.
+
 Quisk Version 4.2.8  September 2022
 ===================================
 This is an update to the new Quisk Remote feature by Ben, AC2YD.
 
 Midi now works with the control head. For HermesLite2, the RfLna is correctly initialized.
 I changed the ports to 4585:TCP control; 4586: graph data; 4587:radio sound and mic. This should
 work correctly with NAT.
```

### Comparing `quisk-4.2.8/PKG-INFO` & `quisk-4.2.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quisk
-Version: 4.2.8
+Version: 4.2.9
 Summary: QUISK is a Software Defined Radio (SDR) transceiver that can control various radio hardware.
 Home-page: http://james.ahlstrom.name/quisk/
 Author: James C. Ahlstrom
 Author-email: jahlstr@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 6 - Mature
```

### Comparing `quisk-4.2.8/WinEdit.pyw` & `quisk-4.2.9/WinEdit.pyw`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/ac2yd/Design_2022_0531.pdf` & `quisk-4.2.9/ac2yd/Design_2022_0531.pdf`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/ac2yd/control_common.py` & `quisk-4.2.9/ac2yd/control_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -322,15 +322,16 @@
     btn = app.modeButns.GetSelectedButton()
     self.RemoteCtlSend("%s;%d\n" % (btn.idName, btn.GetIndex()))
     # Filter and adjustable bandwidth
     name = "Filter 6Slider"
     value = app.midiControls[name][0].button.slider_value
     self.RemoteCtlSend("%s;%d\n" % (name, value))
     btn = app.filterButns.GetSelectedButton()
-    self.RemoteCtlSend("%s;%d\n" % (btn.idName, btn.GetIndex()))
+    if btn:
+      self.RemoteCtlSend("%s;%d\n" % (btn.idName, btn.GetIndex()))
     # AGC and Squelch levels, split offset
     self.RemoteCtlSend("Split;0\n")
     btn = app.BtnAGC
     self.RemoteCtlSend("AGCSQLCH;%d;%d;%d;%d;%d\n" % (btn.slider_value_off, btn.slider_value_on,
            app.levelSquelch, app.levelSquelchSSB, app.split_offset))
     idName = "SqlchSlider"
     value = app.midiControls[idName][0].button.slider_value
```

### Comparing `quisk-4.2.8/ac2yd/control_hermes.py` & `quisk-4.2.9/ac2yd/control_hermes.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,19 @@
     pass
   def ChangeAGC(self, value):
     pass
   def HeartBeat(self):
     ControlCommon.HeartBeat(self)
     args = self.HL2_TEMP.split(';')
     widg = self.app.bottom_widgets
-    widg.text_temperature.SetLabel(args[0])
-    widg.text_pa_current.SetLabel(args[1])
-    widg.text_fwd_power.SetLabel(args[2])
-    widg.text_swr.SetLabel(args[3])
+    if widg:
+      widg.text_temperature.SetLabel(args[0])
+      widg.text_pa_current.SetLabel(args[1])
+      widg.text_fwd_power.SetLabel(args[2])
+      widg.text_swr.SetLabel(args[3])
   def RadioInit(self):	# Send initial parameters not covered by CommonInit()
     idName = "RfLna"
     value = self.app.midiControls[idName][0].GetValue()
     self.RemoteCtlSend("%s;%d\n" % (idName, value))
   def VarDecimGetChoices(self):		# return text labels for the control
     return self.var_rates
   def VarDecimGetLabel(self):		# return a text label for the control
```

### Comparing `quisk-4.2.8/ac2yd/remote.c` & `quisk-4.2.9/ac2yd/remote.c`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/ac2yd/remote_common.py` & `quisk-4.2.9/ac2yd/remote_common.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/ac2yd/remote_hermes.py` & `quisk-4.2.9/ac2yd/remote_hermes.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/ac2yd/remote_softrock.py` & `quisk-4.2.9/ac2yd/remote_softrock.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/afedrinet/afe_library.mac` & `quisk-4.2.9/afedrinet/afe_library.mac`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/afedrinet/afedri.py` & `quisk-4.2.9/afedrinet/afedri.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/afedrinet/afedrinet_io.c` & `quisk-4.2.9/afedrinet/afedrinet_io.c`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/afedrinet/build/import_quisk_api.o` & `quisk-4.2.9/afedrinet/build/import_quisk_api.o`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/afedrinet/build/is_key_down.o` & `quisk-4.2.9/afedrinet/build/is_key_down.o`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/afedrinet/build/temp.linux-x86_64-3.6/afedrinet_io.o` & `quisk-4.2.9/afedrinet/build/temp.linux-x86_64-3.6/afedrinet_io.o`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/afedrinet/quisk_conf.py` & `quisk-4.2.9/afedrinet/quisk_conf.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/afedrinet/quisk_conf_linux.py` & `quisk-4.2.9/afedrinet/quisk_conf_linux.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/afedrinet/quisk_conf_mac.py` & `quisk-4.2.9/afedrinet/quisk_conf_mac.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/afedrinet/quisk_hardware.py` & `quisk-4.2.9/afedrinet/quisk_hardware.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/afedrinet/readme.txt` & `quisk-4.2.9/afedrinet/readme.txt`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/afedrinet/sdr_control.py` & `quisk-4.2.9/afedrinet/sdr_control.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/afedrinet/setup.py` & `quisk-4.2.9/afedrinet/setup.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/configure.py` & `quisk-4.2.9/configure.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/defaults.html` & `quisk-4.2.9/defaults.html`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/docs.html` & `quisk-4.2.9/docs.html`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/dxcluster.py` & `quisk-4.2.9/dxcluster.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/extdemod.c` & `quisk-4.2.9/extdemod.c`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/filter.c` & `quisk-4.2.9/filter.c`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/filter.h` & `quisk-4.2.9/filter.h`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/filters.h` & `quisk-4.2.9/filters.h`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/filters.py` & `quisk-4.2.9/filters.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/freedv.c` & `quisk-4.2.9/freedv.c`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/freedvpkg/README.txt` & `quisk-4.2.9/freedvpkg/README.txt`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/freedvpkg/libcodec2_32.dll` & `quisk-4.2.9/freedvpkg/libcodec2_32.dll`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/freedvpkg/libcodec2_32.so` & `quisk-4.2.9/freedvpkg/libcodec2_32.so`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/freedvpkg/libcodec2_64.dll` & `quisk-4.2.9/freedvpkg/libcodec2_64.dll`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/freedvpkg/libcodec2_64.so` & `quisk-4.2.9/freedvpkg/libcodec2_64.so`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/help.html` & `quisk-4.2.9/help.html`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/help_conf.html` & `quisk-4.2.9/help_conf.html`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/help_vna.html` & `quisk-4.2.9/help_vna.html`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/hermes/README.txt` & `quisk-4.2.9/hermes/README.txt`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/hermes/quisk_hardware.py` & `quisk-4.2.9/hermes/quisk_hardware.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/hermes/quisk_widgets.py` & `quisk-4.2.9/hermes/quisk_widgets.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/hiqsdr/quisk_conf.py` & `quisk-4.2.9/hiqsdr/quisk_conf.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/hiqsdr/quisk_hardware.py` & `quisk-4.2.9/hiqsdr/quisk_hardware.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/import_quisk_api.c` & `quisk-4.2.9/import_quisk_api.c`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/is_key_down.c` & `quisk-4.2.9/is_key_down.c`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/libfftw3-3.dll` & `quisk-4.2.9/libfftw3-3.dll`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/libgcc_s_dw2-1.dll` & `quisk-4.2.9/libgcc_s_dw2-1.dll`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/libusb.txt` & `quisk-4.2.9/libusb.txt`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/libwdsp.dll` & `quisk-4.2.9/libwdsp.dll`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/libwinpthread-1.dll` & `quisk-4.2.9/libwinpthread-1.dll`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/license.txt` & `quisk-4.2.9/license.txt`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/microphone.c` & `quisk-4.2.9/microphone.c`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/midi_handler.py` & `quisk-4.2.9/midi_handler.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/n2adr/.quisk_init.pkl` & `quisk-4.2.9/n2adr/.quisk_init.pkl`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/n2adr/conf2.py` & `quisk-4.2.9/n2adr/conf2.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/n2adr/conf4.py` & `quisk-4.2.9/n2adr/conf4.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/n2adr/conf6.py` & `quisk-4.2.9/n2adr/conf6.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/n2adr/hl2_hardware.py` & `quisk-4.2.9/n2adr/hl2_hardware.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/n2adr/quisk_conf.py` & `quisk-4.2.9/n2adr/quisk_conf.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/n2adr/quisk_conf_8600.py` & `quisk-4.2.9/n2adr/quisk_conf_8600.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/n2adr/quisk_hardware.py` & `quisk-4.2.9/n2adr/quisk_hardware.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/n2adr/quisk_widgets.py` & `quisk-4.2.9/n2adr/quisk_widgets.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/n2adr/scanner_widgets.py` & `quisk-4.2.9/n2adr/scanner_widgets.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/n2adr/startup.py` & `quisk-4.2.9/n2adr/startup.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/n2adr/station_hardware.py` & `quisk-4.2.9/n2adr/station_hardware.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/n2adr/uhf_conf.py` & `quisk-4.2.9/n2adr/uhf_conf.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/n2adr/uhf_hardware.old` & `quisk-4.2.9/n2adr/uhf_hardware.old`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/n2adr/uhf_hardware.py` & `quisk-4.2.9/n2adr/uhf_hardware.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/n2adr/uhf_widgets.py` & `quisk-4.2.9/n2adr/uhf_widgets.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/perseuspkg/build/import_quisk_api.o` & `quisk-4.2.9/perseuspkg/build/import_quisk_api.o`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/perseuspkg/perseus.c` & `quisk-4.2.9/perseuspkg/perseus.c`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/perseuspkg/quisk_hardware.py` & `quisk-4.2.9/perseuspkg/quisk_hardware.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/perseuspkg/quisk_widgets.py` & `quisk-4.2.9/perseuspkg/quisk_widgets.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/perseuspkg/setup.py` & `quisk-4.2.9/perseuspkg/setup.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/portaudio.py` & `quisk-4.2.9/portaudio.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/quisk.c` & `quisk-4.2.9/quisk.c`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/quisk.egg-info/PKG-INFO` & `quisk-4.2.9/quisk.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quisk
-Version: 4.2.8
+Version: 4.2.9
 Summary: QUISK is a Software Defined Radio (SDR) transceiver that can control various radio hardware.
 Home-page: http://james.ahlstrom.name/quisk/
 Author: James C. Ahlstrom
 Author-email: jahlstr@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 6 - Mature
```

### Comparing `quisk-4.2.8/quisk.egg-info/SOURCES.txt` & `quisk-4.2.9/quisk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/quisk.h` & `quisk-4.2.9/quisk.h`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/quisk.py` & `quisk-4.2.9/quisk.py`

 * *Files 1% similar despite different names*

```diff
@@ -604,26 +604,26 @@
     if length == 0:
       mode = self.app.mode
       code = self.Mo2CoKen.get(mode, 2)
       self.Write("%s%d;" % (cmd, code))
     elif length == 1:
       code = int(data, base=10)
       mode = self.Co2MoKen.get(code, 'USB')
-      self.app.OnBtnMode(None, mode)		# Set mode
+      self.app.modeButns.SetLabel(mode, True)		# Set mode
     else:
       self.Error(cmd, data)
   def ZZMD(self, cmd, data, length):	# the mode; USB, CW, etc.
     if length == 0:
       mode = self.app.mode
       code = self.Mo2CoFlex.get(mode, 1)
       self.Write("%s%02d;" % (cmd, code))
     elif length == 2:
       code = int(data, base=10)
       mode = self.Co2MoFlex.get(code, 'USB')
-      self.app.OnBtnMode(None, mode)	# Set mode
+      self.app.modeButns.SetLabel(mode, True)		# Set mode
     else:
       self.Error(cmd, data)
   def ZZMU(self, cmd, data, length):	# MultiRx on/off
     if length == 0:
       self.Write("%s0;" % cmd)
   def OI(self, cmd, data, length):      # return information
     self.ZZIF(cmd, data, length)
@@ -1062,28 +1062,28 @@
       self.Reply(0)
     elif mode == 'CWR':
       mode = 'CWL'
       self.Reply(0)
     else:
       self.ErrParam()
       return
-    self.app.OnBtnMode(None, mode)		# Set mode
+    self.app.modeButns.SetLabel(mode, True)		# Set mode
     if bw <= 0:		# use default bandwidth
       return
     # Choose button closest to requested bandwidth
     buttons = self.app.filterButns.GetButtons()
     Lab = buttons[0].GetLabel()
     diff = abs(int(Lab) - bw)
     for i in range(1, len(buttons) - 1):
       label = buttons[i].GetLabel()
       df = abs(int(label) - bw)
       if df < diff:
         Lab = label
         diff = df
-    self.app.OnBtnFilter(None, int(Lab))
+    self.app.filterButns.SetLabel(Lab, True)
   def GetVfo(self):
     self.Reply('VFO', self.vfo, 0)
   def SetVfo(self):
     name = self.GetParamName()
     if name == '?':	# send back supported parameters
       self.Reply2('Main', 0)
     else:
@@ -1836,15 +1836,15 @@
   def OnRightClickLabel(self, event):
     event.Skip()
     self.menurow = event.GetRow()
     if self.menurow >= 0:
       pos = event.GetPosition()
       self.PopupMenu(self.popupmenu, pos)
   def OnLeftClickLabel(self, event):
-    pass
+    self.OnRightClickLabel(event)
   def OnLeftDClick(self, event):		# Thanks to Christof, DJ4CM
     self.menurow = event.GetRow()
     if self.menurow >= 0:
       self.OnPopupTuneto(event)
   def OnPopupAppend(self, event):
     self.InsertRows(self.menurow + 1)
     self.SetCellEditor(self.menurow + 1, 2, wx.grid.GridCellChoiceEditor(self.mode_names, True))
@@ -1887,15 +1887,15 @@
     if self.changed:
       if self.timer.IsRunning():
         self.timer.Stop()
       self.WriteOut()
     application.ChangeRxTxFrequency(None, freq)
     mode = self.GetCellValue(self.menurow, 2)
     mode = mode.upper()
-    application.OnBtnMode(None, mode)
+    application.modeButns.SetLabel(mode, True)
     application.screenBtnGroup.SetLabel(conf.default_screen, do_cmd=True)
   def MakeRepeaterDict(self):
     self.RepeaterDict = {}
     for row in range(self.GetNumberRows()):
       offset = self.GetCellValue(row, 4)
       offset = offset.strip()
       if not offset:
@@ -2683,15 +2683,15 @@
       # tune to station
       if self.tunedStation >= self.nrStationInRange:
         self.tunedStation = 0      
       freq, symbol, name, mode, dscr = self.stationList[self.firstStationInRange+self.tunedStation]
       self.tunedStation += 1
       if mode != '': # information about mode available
         mode = mode.upper()
-        application.OnBtnMode(None, mode)
+        application.modeButns.SetLabel(mode, True)
       application.ChangeRxTxFrequency(None, freq)
   def OnMotion(self, event):
     mouse_x, mouse_y = event.GetPosition()
     x = (mouse_x - self.mouse_x)
     application.isTuning = False
     # show detailed station info
     if abs(self.lastStationX - mouse_x) > 30:
@@ -4475,15 +4475,15 @@
           self.accel_list.append(wx.AcceleratorEntry(wx.ACCEL_ALT, ord(button.char_shortcut), rid))
     else:	# Small screen
       for button in self.modeButns.GetButtons():	# mode buttons
         self.idName2Button[button.idName] = self.modeButns
       for button in self.bandBtnGroup.GetButtons():	# band buttons
         self.idName2Button[button.idName] = self.bandBtnGroup
     self.main_frame.SetAcceleratorTable(wx.AcceleratorTable(self.accel_list))
-    self.OnBtnMode(None, self.mode)
+    self.modeButns.SetLabel(self.mode, True)
   #  self.OnTestTimer(None)
     if hasattr(Hardware, 'post_open'):	# post_open() is called after open() and after sound is started
       Hardware.post_open()
     self.StartWsjtx()
     self.midiControls["Tune"]	= (None,		None)
     self.midiControls["Vol"]	= (self.sliderVol,	self.ChangeVolume)
     self.midiControls["STo"]	= (self.sliderSto,	self.ChangeSidetone)
@@ -5596,18 +5596,18 @@
         filtI.append(z.real)
         filtQ.append(z.imag)
       return filtI, filtQ
     return filtD, filtD
   def SetFilterByMode(self, mode):
     index = self.modeFilter[mode]
     try:
-      bw = int(self.filterButns.buttons[index].GetLabel())
+      Lab = self.filterButns.buttons[index].GetLabel()
     except:
-      bw = int(self.filterButns.buttons[0].GetLabel())
-    self.OnBtnFilter(None, bw)
+      Lab = self.filterButns.buttons[0].GetLabel()
+    self.filterButns.SetLabel(Lab, True)
   def GetFilterCenter(self, mode, bandwidth):
     if mode in ('CWU', 'CWL'):
       center = max(conf.cwTone, bandwidth // 2)
     elif mode in ('LSB', 'USB'):
       center = 300 + bandwidth // 2
     elif mode in ('AM',):
       center = 0
@@ -5671,28 +5671,30 @@
     self.multi_rx_screen.waterfall.pane1.filter_bandwidth = bw
     self.multi_rx_screen.waterfall.pane1.filter_center = center
     self.multi_rx_screen.waterfall.pane2.filter_mode = mode
     self.multi_rx_screen.waterfall.pane2.filter_bandwidth = bw
     self.multi_rx_screen.waterfall.pane2.filter_center = center
     if self.screen is self.filter_screen:
       self.screen.NewFilter()
-  def OnFreedvMenu(self, event, text=None, show_dlg=True):
-    if event:
-      idd = event.GetId()
-      text = self.freedv_menu.GetLabel(idd)
+  def OnFreedvMenu(self, event):
+    text = ''
+    for item in self.freedv_menu.GetMenuItems():
+      if item.IsChecked():
+        text = item.GetItemLabel()
+        break
     for mode, index in conf.freedv_modes:
       if mode == text:
         break
     else:
       print ("Failure in OnFreedvMenu")
       return
     mode = QS.freedv_set_options(mode=index)
     if mode == index:
       self.freedv_mode = text
-    elif show_dlg:		# change to new mode failed
+    elif not self.remote_control_slave:		# change to new mode failed
       self.freedv_menu_items[mode].Check(1)
       pos = (self.width//2, self.height//2)
       if index == 8:
         dlg = wx.MessageDialog(self.main_frame, "Quisk does not install %s. Please install a system-wide codec2." % text, "FreeDV Modes", wx.OK, pos)
       else:
         dlg = wx.MessageDialog(self.main_frame, "No codec2 support for " + text, "FreeDV Modes", wx.OK, pos)
       dlg.ShowModal()
@@ -6278,19 +6280,16 @@
         vfo = (tx_freq // 5000) * 5000 - 5000
         tune = tx_freq - vfo
         self.BandFromFreq(tx_freq)
       self.ChangeHwFrequency(tune, vfo, 'FreqEntry')
     if rx_freq and self.split_rxtx:		# Frequency must be on-screen
       tune = rx_freq - self.VFO
       self.ChangeHwFrequency(self.txFreq, self.VFO, 'FreqEntry', event=event, rx_freq=tune)
-  def OnBtnMode(self, event, mode=None):
-    if event is None:	# called by application
-      self.modeButns.SetLabel(mode)
-    else:		# called by button
-      mode = self.modeButns.GetLabel()
+  def OnBtnMode(self, event):
+    mode = self.modeButns.GetLabel()
     delta = 0	# Change frequency so switch between CW and SSB keeps tone constant
     if self.mode == 'USB':
       if mode in ('CWL', 'CWU'):
         delta = 1
     elif self.mode == 'LSB':
       if mode in ('CWL', 'CWU'):
         delta = -1
@@ -6351,15 +6350,15 @@
     frq = int(frq)
     for freq, band, vfo, txfreq, mode in self.memoryState:
       if freq == frq:
         break
     else:
       return
     if band == self.lastBand:	# leave band unchanged
-      self.OnBtnMode(None, mode)
+      self.modeButns.SetLabel(mode, True)
       self.ChangeHwFrequency(txfreq, vfo, 'FreqEntry')
     else:		# change to new band
       self.bandState[band] = (vfo, txfreq, mode)
       self.bandBtnGroup.SetLabel(band, do_cmd=True)
   def OnBtnMemSave(self, event):
     frq = self.VFO + self.txFreq
     for i in range(len(self.memoryState)):
@@ -6377,15 +6376,15 @@
     frq = self.VFO + self.txFreq
     for freq, band, vfo, txfreq, mode in self.memoryState:
       if freq > frq:
         break
     else:
       freq, band, vfo, txfreq, mode = self.memoryState[0]
     if band == self.lastBand:	# leave band unchanged
-      self.OnBtnMode(None, mode)
+      self.modeButns.SetLabel(mode, True)
       self.ChangeHwFrequency(txfreq, vfo, 'FreqEntry')
     else:		# change to new band
       self.bandState[band] = (vfo, txfreq, mode)
       self.bandBtnGroup.SetLabel(band, do_cmd=True)
   def OnBtnMemDelete(self, event):
     frq = self.VFO + self.txFreq
     for i in range(len(self.memoryState)):
@@ -6458,15 +6457,15 @@
       while freq - vfo <= -half + 1000:
         vfo -= 10000
       while freq - vfo >= +half - 5000:
         vfo += 10000
       tune = freq - vfo
     elif band == 'Time':
       vfo, tune, mode = conf.bandTime[btn.index]
-    self.OnBtnMode(None, mode)
+    self.modeButns.SetLabel(mode, True)
     self.txFreq = self.VFO = -1		# demand change
     self.ChangeBand(band)
     self.ChangeHwFrequency(tune, vfo, 'BtnBand', band=band)
     if band in ('Time', 'Audio') or conf.tx_level.get(band, 127) == 0:
       self.pttButton.Enable(False)
     else:
       self.pttButton.Enable(True)
@@ -6488,15 +6487,15 @@
       if f1 <= frequency <= f2:
         self.lastBand = band
         self.bandBtnGroup.SetLabel(band, do_cmd=False)
         try:
           vfo, tune, mode = self.bandState[band]
         except KeyError:
           vfo, tune, mode = (0, 0, 'LSB')
-        self.OnBtnMode(None, mode)
+        self.modeButns.SetLabel(mode, True)
         self.ChangeBand(band)
         break
   def ChangeBand(self, band):
     Hardware.ChangeBand(band)
     s, z = self.graphScaleZ.get(band, (conf.graph_y_scale, conf.graph_y_zero))
     self.waterfall.SetPane1(self.wfallGrScaleZ.get(band, (s, z)))
     self.waterfall.SetPane2(self.wfallScaleZ.get(band, (conf.waterfall_y_scale, conf.waterfall_y_zero)))
```

### Comparing `quisk-4.2.8/quisk_conf_defaults.py` & `quisk-4.2.9/quisk_conf_defaults.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/quisk_conf_kx3.py` & `quisk-4.2.9/quisk_conf_kx3.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/quisk_conf_model.py` & `quisk-4.2.9/quisk_conf_model.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/quisk_conf_openradio.py` & `quisk-4.2.9/quisk_conf_openradio.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/quisk_conf_sdr8600.py` & `quisk-4.2.9/quisk_conf_sdr8600.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/quisk_conf_sdriq.py` & `quisk-4.2.9/quisk_conf_sdriq.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/quisk_conf_win.py` & `quisk-4.2.9/quisk_conf_win.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/quisk_hardware_fixed.py` & `quisk-4.2.9/quisk_hardware_fixed.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/quisk_hardware_hamlib.py` & `quisk-4.2.9/quisk_hardware_hamlib.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,12 +146,12 @@
           if DEBUG: print('    Radio G mode', mode)
           if self.quisk_mode == self.radio_mode:
             if self.radio_mode != mode:		# The radio changed the mode
               self.radio_mode = mode
               self.quisk_mode = mode
               if mode in ('CW', 'CWR'):
                 mode = 'CWU'
-              self.application.OnBtnMode(None, mode)		# Set mode
+              self.application.modeButns.SetLabel(mode, True)		# Set mode
         else:
           if DEBUG: print('Unknown', reply)
       except:
         if DEBUG: traceback.print_exc()
```

### Comparing `quisk-4.2.8/quisk_hardware_hl2_oob.py` & `quisk-4.2.9/quisk_hardware_hl2_oob.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/quisk_hardware_model.py` & `quisk-4.2.9/quisk_hardware_model.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/quisk_hardware_sdr8600.py` & `quisk-4.2.9/quisk_hardware_sdr8600.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/quisk_hardware_sdriq.py` & `quisk-4.2.9/quisk_hardware_sdriq.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/quisk_utils.py` & `quisk-4.2.9/quisk_utils.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/quisk_vna.py` & `quisk-4.2.9/quisk_vna.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/quisk_wdsp.c` & `quisk-4.2.9/quisk_wdsp.c`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/quisk_wdsp.py` & `quisk-4.2.9/quisk_wdsp.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/quisk_widgets.py` & `quisk-4.2.9/quisk_widgets.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/sdriqpkg/quisk_hardware.py` & `quisk-4.2.9/sdriqpkg/quisk_hardware.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/sdriqpkg/sdriq.c` & `quisk-4.2.9/sdriqpkg/sdriq.c`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/sdriqpkg/sdriq.h` & `quisk-4.2.9/sdriqpkg/sdriq.h`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/sdrmicronpkg/quisk_hardware.py` & `quisk-4.2.9/sdrmicronpkg/quisk_hardware.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/setup.py` & `quisk-4.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 # This file is used to build the Linux and Mac versions of Quisk. Windows builds are not included.
 
 # You must define the version here.  A title string including
 # the version will be written to __init__.py and read by quisk.py.
 
-Version = '4.2.8'
+Version = '4.2.9'
 
 fp = open("__init__.py", "w")	# write title string
 fp.write("#Quisk version %s\n" % Version)
 fp.write("from .quisk import main\n")
 fp.close()
 
 sources = ['quisk.c', 'sound.c', 'is_key_down.c', 'microphone.c', 'utility.c',
```

### Comparing `quisk-4.2.8/soapypkg/build/import_quisk_api.o` & `quisk-4.2.9/soapypkg/build/import_quisk_api.o`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/soapypkg/build/temp.linux-x86_64-2.7/soapy.o` & `quisk-4.2.9/soapypkg/build/temp.linux-x86_64-2.7/soapy.o`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/soapypkg/build/temp.linux-x86_64-3.6/soapy.o` & `quisk-4.2.9/soapypkg/build/temp.linux-x86_64-3.6/soapy.o`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/soapypkg/build/temp.win32-2.7/import_quisk_api.o` & `quisk-4.2.9/soapypkg/build/temp.win32-2.7/import_quisk_api.o`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/soapypkg/quisk_hardware.py` & `quisk-4.2.9/soapypkg/quisk_hardware.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/soapypkg/setup.py` & `quisk-4.2.9/soapypkg/setup.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/soapypkg/soapy.c` & `quisk-4.2.9/soapypkg/soapy.c`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/softrock/hardware_net.py` & `quisk-4.2.9/softrock/hardware_net.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/softrock/hardware_usb.py` & `quisk-4.2.9/softrock/hardware_usb.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/softrock/widgets_tx.py` & `quisk-4.2.9/softrock/widgets_tx.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/softrock_tune_vfo.py` & `quisk-4.2.9/softrock_tune_vfo.py`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/sound.c` & `quisk-4.2.9/sound.c`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/sound_alsa.c` & `quisk-4.2.9/sound_alsa.c`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/sound_directx.c` & `quisk-4.2.9/sound_directx.c`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/sound_portaudio.c` & `quisk-4.2.9/sound_portaudio.c`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/sound_pulseaudio.c` & `quisk-4.2.9/sound_pulseaudio.c`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/sound_wasapi.c` & `quisk-4.2.9/sound_wasapi.c`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/utility.c` & `quisk-4.2.9/utility.c`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/windows.txt` & `quisk-4.2.9/windows.txt`

 * *Files identical despite different names*

### Comparing `quisk-4.2.8/winsound.txt` & `quisk-4.2.9/winsound.txt`

 * *Files identical despite different names*

