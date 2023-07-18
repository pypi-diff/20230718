# Comparing `tmp/vortexdm-2022.1.0.tar.gz` & `tmp/vortexdm-2023.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vortexdm-2022.1.0.tar", last modified: Tue Aug 16 23:03:41 2022, max compression
+gzip compressed data, was "vortexdm-2023.1.0.tar", last modified: Tue Jul 18 18:27:45 2023, max compression
```

## Comparing `vortexdm-2022.1.0.tar` & `vortexdm-2023.1.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2022-08-16 23:03:41.866632 vortexdm-2022.1.0/
--rw-rw-rw-   0        0        0    39587 2022-08-05 05:33:34.000000 vortexdm-2022.1.0/LICENSE.md
--rw-rw-rw-   0        0        0     9576 2022-08-16 23:03:41.866632 vortexdm-2022.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     8511 2022-08-16 22:35:41.000000 vortexdm-2022.1.0/README.md
--rw-rw-rw-   0        0        0       82 2022-08-16 22:14:11.000000 vortexdm-2022.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-08-16 23:03:41.867517 vortexdm-2022.1.0/setup.cfg
--rw-rw-rw-   0        0        0     2407 2022-08-16 22:57:43.000000 vortexdm-2022.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-08-16 23:03:41.851056 vortexdm-2022.1.0/vdm/
--rw-rw-rw-   0        0        0    20220 2022-08-05 07:34:53.000000 vortexdm-2022.1.0/vdm/VDM.py
--rw-rw-rw-   0        0        0       29 2022-05-23 05:13:41.000000 vortexdm-2022.1.0/vdm/__init__.py
--rw-rw-rw-   0        0        0      702 2022-08-05 05:44:46.000000 vortexdm-2022.1.0/vdm/__main__.py
--rw-rw-rw-   0        0        0      342 2022-08-05 05:48:38.000000 vortexdm-2022.1.0/vdm/about.py
--rw-rw-rw-   0        0        0    23853 2022-08-05 05:53:15.000000 vortexdm-2022.1.0/vdm/brain.py
--rw-rw-rw-   0        0        0     8677 2022-08-05 05:56:11.000000 vortexdm-2022.1.0/vdm/cmdview.py
--rw-rw-rw-   0        0        0    12725 2022-08-05 06:00:35.000000 vortexdm-2022.1.0/vdm/config.py
--rw-rw-rw-   0        0        0    62821 2022-08-05 06:04:56.000000 vortexdm-2022.1.0/vdm/controller.py
--rw-rw-rw-   0        0        0     1989 2022-08-05 06:05:45.000000 vortexdm-2022.1.0/vdm/dependency.py
--rw-rw-rw-   0        0        0    30034 2022-08-05 06:06:25.000000 vortexdm-2022.1.0/vdm/downloaditem.py
--rw-rw-rw-   0        0        0    41681 2022-08-05 07:19:14.000000 vortexdm-2022.1.0/vdm/iconsbase64.py
--rw-rw-rw-   0        0        0     6496 2022-08-05 07:20:25.000000 vortexdm-2022.1.0/vdm/model.py
--rw-rw-rw-   0        0        0     6996 2022-08-05 07:20:58.000000 vortexdm-2022.1.0/vdm/setting.py
--rw-rw-rw-   0        0        0     7044 2022-08-05 07:21:42.000000 vortexdm-2022.1.0/vdm/systray.py
--rw-rw-rw-   0        0        0    11308 2022-05-23 05:13:41.000000 vortexdm-2022.1.0/vdm/themes.py
--rw-rw-rw-   0        0        0   200466 2022-08-05 07:25:53.000000 vortexdm-2022.1.0/vdm/tkview.py
--rw-rw-rw-   0        0        0    10151 2022-08-16 20:43:28.000000 vortexdm-2022.1.0/vdm/update.py
--rw-rw-rw-   0        0        0    40394 2022-08-05 07:28:31.000000 vortexdm-2022.1.0/vdm/utils.py
--rw-rw-rw-   0        0        0       25 2022-08-05 07:35:26.000000 vortexdm-2022.1.0/vdm/version.py
--rw-rw-rw-   0        0        0    57154 2022-08-05 07:36:13.000000 vortexdm-2022.1.0/vdm/video.py
--rw-rw-rw-   0        0        0     1577 2022-08-05 07:36:33.000000 vortexdm-2022.1.0/vdm/view.py
--rw-rw-rw-   0        0        0    13667 2022-08-05 07:36:52.000000 vortexdm-2022.1.0/vdm/worker.py
-drwxrwxrwx   0        0        0        0 2022-08-16 23:03:41.865618 vortexdm-2022.1.0/vortexdm.egg-info/
--rw-rw-rw-   0        0        0     9576 2022-08-16 23:03:41.000000 vortexdm-2022.1.0/vortexdm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      563 2022-08-16 23:03:41.000000 vortexdm-2022.1.0/vortexdm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-16 23:03:41.000000 vortexdm-2022.1.0/vortexdm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2022-08-16 23:03:41.000000 vortexdm-2022.1.0/vortexdm.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      134 2022-08-16 23:03:41.000000 vortexdm-2022.1.0/vortexdm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2022-08-16 23:03:41.000000 vortexdm-2022.1.0/vortexdm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 18:27:45.150583 vortexdm-2023.1.0/
+-rw-rw-rw-   0        0        0    39587 2022-08-05 05:33:34.000000 vortexdm-2023.1.0/LICENSE.md
+-rw-rw-rw-   0        0        0     8330 2023-07-18 18:27:45.149585 vortexdm-2023.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7257 2023-07-14 06:42:54.000000 vortexdm-2023.1.0/README.md
+-rw-rw-rw-   0        0        0       82 2022-08-16 22:14:11.000000 vortexdm-2023.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-18 18:27:45.150583 vortexdm-2023.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     2375 2023-07-14 05:11:06.000000 vortexdm-2023.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 18:27:45.115581 vortexdm-2023.1.0/vortexdm/
+-rw-rw-rw-   0        0        0    20263 2023-07-14 07:07:08.000000 vortexdm-2023.1.0/vortexdm/VortexDM.py
+-rw-rw-rw-   0        0        0       29 2022-05-23 05:13:41.000000 vortexdm-2023.1.0/vortexdm/__init__.py
+-rw-rw-rw-   0        0        0      726 2023-07-14 07:01:15.000000 vortexdm-2023.1.0/vortexdm/__main__.py
+-rw-rw-rw-   0        0        0      354 2023-07-14 07:03:16.000000 vortexdm-2023.1.0/vortexdm/about.py
+-rw-rw-rw-   0        0        0    23858 2023-07-14 07:03:30.000000 vortexdm-2023.1.0/vortexdm/brain.py
+-rw-rw-rw-   0        0        0     8707 2023-07-14 07:03:38.000000 vortexdm-2023.1.0/vortexdm/cmdview.py
+-rw-rw-rw-   0        0        0    12740 2023-07-14 07:04:17.000000 vortexdm-2023.1.0/vortexdm/config.py
+-rw-rw-rw-   0        0        0    64248 2023-07-18 07:28:28.000000 vortexdm-2023.1.0/vortexdm/controller.py
+-rw-rw-rw-   0        0        0     1994 2023-07-14 07:04:40.000000 vortexdm-2023.1.0/vortexdm/dependency.py
+-rw-rw-rw-   0        0        0    30044 2023-07-14 07:04:48.000000 vortexdm-2023.1.0/vortexdm/downloaditem.py
+-rw-rw-rw-   0        0        0    42008 2023-07-14 07:04:57.000000 vortexdm-2023.1.0/vortexdm/iconsbase64.py
+-rw-rw-rw-   0        0        0     6501 2023-07-14 07:05:10.000000 vortexdm-2023.1.0/vortexdm/model.py
+-rw-rw-rw-   0        0        0     7001 2023-07-14 07:05:22.000000 vortexdm-2023.1.0/vortexdm/setting.py
+-rw-rw-rw-   0        0        0     7054 2023-07-14 07:05:31.000000 vortexdm-2023.1.0/vortexdm/systray.py
+-rw-rw-rw-   0        0        0    11635 2023-07-14 07:05:39.000000 vortexdm-2023.1.0/vortexdm/themes.py
+-rw-rw-rw-   0        0        0   200559 2023-07-14 07:05:52.000000 vortexdm-2023.1.0/vortexdm/tkview.py
+-rw-rw-rw-   0        0        0    10186 2023-07-14 07:06:10.000000 vortexdm-2023.1.0/vortexdm/update.py
+-rw-rw-rw-   0        0        0    40419 2023-07-14 07:06:23.000000 vortexdm-2023.1.0/vortexdm/utils.py
+-rw-rw-rw-   0        0        0       25 2023-07-14 07:06:38.000000 vortexdm-2023.1.0/vortexdm/version.py
+-rw-rw-rw-   0        0        0    57105 2023-07-18 07:44:21.000000 vortexdm-2023.1.0/vortexdm/video.py
+-rw-rw-rw-   0        0        0     1580 2023-07-14 07:06:59.000000 vortexdm-2023.1.0/vortexdm/view.py
+-rw-rw-rw-   0        0        0    13672 2023-07-14 07:07:17.000000 vortexdm-2023.1.0/vortexdm/worker.py
+drwxrwxrwx   0        0        0        0 2023-07-18 18:27:45.147588 vortexdm-2023.1.0/vortexdm.egg-info/
+-rw-rw-rw-   0        0        0     8330 2023-07-18 18:27:44.000000 vortexdm-2023.1.0/vortexdm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      678 2023-07-18 18:27:45.000000 vortexdm-2023.1.0/vortexdm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 18:27:44.000000 vortexdm-2023.1.0/vortexdm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-07-18 18:27:45.000000 vortexdm-2023.1.0/vortexdm.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      134 2023-07-18 18:27:45.000000 vortexdm-2023.1.0/vortexdm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-18 18:27:45.000000 vortexdm-2023.1.0/vortexdm.egg-info/top_level.txt
```

### Comparing `vortexdm-2022.1.0/LICENSE.md` & `vortexdm-2023.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `vortexdm-2022.1.0/PKG-INFO` & `vortexdm-2023.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,199 +1,178 @@
 Metadata-Version: 2.1
 Name: vortexdm
-Version: 2022.1.0
+Version: 2023.1.0
 Summary: Vortex Download Manager
-Home-page: https://github.com/Sixline/VDM 
+Home-page: https://github.com/Sixline/VortexDM 
 Author: Mahmoud Elshahat
 Maintainer: Sixline
-Project-URL: Source, https://github.com/Sixline/VDM
-Project-URL: Tracker, https://github.com/Sixline/VDM/issues
-Project-URL: Releases, https://github.com/Sixline/VDM/releases
-Keywords: vdm firedm internet download manager youtube hls pycurl curl youtube-dl tkinter
-Classifier: Programming Language :: Python :: 3.7
+Project-URL: Source, https://github.com/Sixline/VortexDM
+Project-URL: Tracker, https://github.com/Sixline/VortexDM/issues
+Project-URL: Releases, https://github.com/Sixline/VortexDM/releases
+Keywords: vortexdm vdm firedm internet download manager youtube hls pycurl curl youtube-dl tkinter
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-# Renaming the project to Vortex Download Manager and will carry on where FireDM 2022.2.5 left off. Original project, FireDM, by Mahmoud Elshahat. RIP
+![Logo](https://raw.githubusercontent.com/Sixline/VortexDM/main/icons/vortexdm.png)
+Vortex Download Manager (VortexDM) is an open-source Python Internet download manager with a high speed multi-connection engine. It downloads general files and videos. Developed in Python, based on "PycURL" and "youtube_dl".
 
-The original creator removed the project repository from Github but left it on PyPI. The latest version they published there, 2022.4.14, I believe was purposely sabotaged to not work and anybody who accepted the update in FireDM would be left with the broken version. ~~If you want to install from PyPI install 2022.2.5 and don't update. https://pypi.org/project/FireDM/2022.2.5~~ 2022.2.5 is now gone from PyPI.
+Original project, FireDM, by Mahmoud Elshahat.
 
-Homepage: https://github.com/Sixline/VDM
+Homepage: https://github.com/Sixline/VortexDM  
+PyPI Homepage: https://pypi.org/project/vortexdm
 
-![GitHub All Releases](https://img.shields.io/github/downloads/Sixline/VDM/total?color=orange&label=GitHub%20Releases)
-
-![GitHub issues](https://img.shields.io/github/issues-raw/Sixline/VDM?color=brightgreen) - ![GitHub closed issues](https://img.shields.io/github/issues-closed-raw/Sixline/VDM?color=blueviolet)
-
-![Logo](https://raw.githubusercontent.com/Sixline/VDM/main/icons/vdm.png)
-Vortex Download Manager (VDM) is an open-source python Internet download manager with a high speed multi-connection engine. It downloads general files and videos from youtube and tons of other streaming websites.
-
-Developed in Python, based on "LibCurl", and "youtube_dl".
+[![GitHub Issues](https://img.shields.io/github/issues-raw/Sixline/VortexDM?color=brightgreen)](https://github.com/Sixline/VortexDM/issues) - [![GitHub Closed Issues](https://img.shields.io/github/issues-closed-raw/Sixline/VortexDM?color=blueviolet)](https://github.com/Sixline/VortexDM/issues?q=is%3Aissue+is%3Aclosed)
 
 **Features**:
-* High download speeds based on LibCurl
+* High download speeds - based on PycURL
 * Multi-connection downloading
 * Automatic file segmentation
 * Automatic refresh for dead links
 * Resume uncompleted downloads
-* Support for Youtube, and a lot of other stream websites using youtube-dl to fetch info and libcurl to download media
-* Download entire video, playlist, or selected videos
+* Support for YouTube and a lot of other stream websites using youtube-dl to fetch info and PycURL to download media
+* Download entire videos, playlists, or selected videos
 * Download fragmented video streams and encrypted/nonencrypted HLS media streams
 * Watch videos while downloading *some videos will have no audio until they finish downloading*
 * Download video subtitles
 * Write video metadata to downloaded files
-* Checking for application updates
+* Built-in updater
 * Scheduled downloads
 * Re-using existing connections
 * Clipboard monitor
 * Proxy support (http, https, socks4, and socks5)
 * User/pass authentication, referee link, video thumbnail, and subtitles
 * Use custom cookie files
 * MD5 and SHA256 checksums
 * Custom GUI themes
 * Set download speed limit
 * Shell commands or computer shutdown on download completion
 * Control number of the concurrent downloads and maximum connections
 
-# How to use VDM:
-Running in command line: show help by typing `vdm -h`
+# How to use VortexDM:
+Running in command line: show help by typing `vortexdm -h`
 
-Running the GUI: Refer to the user guide at https://github.com/Sixline/VDM/blob/master/docs/user_guide.md
+Running the GUI: Refer to the user guide at https://github.com/Sixline/VortexDM/blob/master/docs/user_guide.md
 
-# Portable VDM versions:
+# Portable VortexDM Versions:
   
-Run VDM without any installation (recommended) 
- - **Windows portable version** ([Download!](https://github.com/Sixline/VDM/releases/latest)):  
-   available in .zip format.  
-   unzip, and run from VDM.exe, no installation required.
-   
- - **Linux portable version** ([Download!](https://github.com/Sixline/VDM/releases/latest)):   
-   available in .AppImage format.  
-   download file, then mark it as executable, and run it, no installation required,
-   Tested on Ubuntu.
-   note: ffmpeg is not included and must be installed separately
+Run VortexDM without any installation (recommended) 
+ - **Windows Portable Version** ([Download!](https://github.com/Sixline/VortexDM/releases/latest)):  
+   Available in .zip format. Built with 64-bit Python 3.11+ and will only work on 64-bit Windows 10+.  
+   Unzip and run VortexDM-GUI.exe, no installation required.
    
-   mark file as executable by right clicking the file> Properties> Permissions> Allow executing file as a program, or from terminal by `chmod +x VDM_xxx.AppImage`
-   
-   To check for ffmpeg use this command:
-   ```sh
-    which ffmpeg
-   
-    # expected output if installed
-    /usr/bin/ffmpeg
-   ```
+ - **Linux Portable Version**  
+  Removing this section for now as I am not familiar with building AppImages. Will revisit.
 
-   if ffmpeg is missing you can install it by `sudo apt install ffmpeg` on debian based or `sudo pacman -S ffmpeg` on Arch based distros.
+## Manually installing VortexDM with pip (Linux Only - Debian/Ubuntu Based Shown):
+1- Check python version (minimum version required is 3.8): `python3 --version`
 
-## Manually installing VDM with pip (Linux Only):
-1- check python version (minimum version required is 3.7): `python3 --version`
-
-2- install required packages first:<br>
-- Linux, ubuntu:<br>
+2- Install required packages:
 ```sh
 sudo apt install ffmpeg libcurl4-openssl-dev libssl-dev python3-pip python3-pil python3-pil.imagetk python3-tk python3-dbus gir1.2-appindicator3-0.1
 sudo apt install fonts-symbola fonts-linuxlibertine fonts-inconsolata fonts-emojione
 ```
 
-3- install Vortex Download Manager using pip:<br>
+3- Install Vortex Download Manager using pip:
 
 ```sh
 python3 -m pip install vortexdm --user --upgrade --no-cache
 ```
 
-## Running from source code inside virtual environment (Linux):
-1- check python version (minimum version required is 3.7): `python3 --version`
+## Running from source code inside a Python virtual environment (Linux Only - Debian/Ubuntu Based Shown):
+1- Check python version (minimum version required is 3.8): `python3 --version`
 
-2- install required packages first:
-- Linux, ubuntu:
+2- Install required packages:
 ```sh
 sudo apt install ffmpeg libcurl4-openssl-dev libssl-dev python3-pip python3-pil python3-pil.imagetk python3-tk python3-dbus gir1.2-appindicator3-0.1
 sudo apt install fonts-symbola fonts-linuxlibertine fonts-inconsolata fonts-emojione
 ```
 
-3- run below code to clone this repo, create virtual environment, install requirements, create launch script, and finally run VDM
+3- Run below code to do the following:  
+  * Clone this repo  
+  * Create Python virtual environment  
+  * Install the requirements  
+  * Create launch script  
+  * Run VortexDM
 
 ```sh
-git clone --depth 1 https://github.com/VDM/VDM.git
+git clone https://github.com/Sixline/VortexDM
 python3 -m venv ./.env
 source ./.env/bin/activate
-python3 -m pip install -r ./VDM/requirements.txt
+python3 -m pip install -r ./VortexDM/requirements.txt
 echo "source ./.env/bin/activate
-python3 ./VDM/vdm.py \$@
-" > vdm.sh
-chmod +x ./vdm.sh
-./vdm.sh
+python3 ./VortexDM/vortexdm.py \$@ " > vortexdm.sh
+chmod +x ./vortexdm.sh
+./vortexdm.sh
 ```
 
-> optionally create .desktop file and add VDM to your applications
+> Optionally create .desktop file and add VortexDM to your applications
 ```sh
-VDMLSPATH=$(realpath ./vdm.sh)
+VortexDMLSPATH=$(realpath ./vortexdm.sh)
 echo "[Desktop Entry]
-Name=Vortex Download Manager
-GenericName=VDM
+Name=VortexDM
+GenericName=VortexDM
 Comment=Vortex Download Manager
-Exec=$VDMLSPATH
-Icon=vdm
+Exec=$VortexDMLSPATH
+Icon=vortexdm
 Terminal=false
 Type=Application
 Categories=Network;
 Keywords=Internet;download
-" > VDM.desktop
-cp ./VDM.desktop ~/.local/share/applications/
+" > VortexDM.desktop
+cp ./VortexDM.desktop ~/.local/share/applications/
 mkdir -p ~/.local/share/icons/hicolor/48x48/apps/
-cp ./VDM/icons/vdm.png ~/.local/share/icons/hicolor/48x48/apps/vdm.png
+cp ./VortexDM/icons/vortexdm.png ~/.local/share/icons/hicolor/48x48/apps/vortexdm.png
 ```
 
 # Known Issues:
-- Linux X-server will raise an error if some fonts are missing especially emoji fonts - See Dependencies below
+- Linux X Server will raise an error if some fonts are missing, especially emoji fonts - See Dependencies below
 
-- Mac - Tkinter, as mentioned in "python.org" the Apple-supplied Tcl/Tk 8.5 has serious bugs that can cause application crashes. If you wish to use Tkinter, do not use the Apple-supplied Pythons. Instead, install and use a newer version of Python from python.org or a third-party distributor that supplies or links with a newer version of Tcl/Tk.
+- Mac - Tkinter - Can have issues depending on versions. See here: https://www.python.org/download/mac/tcltk
 
-- systray icon: depends on Gtk+3 and AppIndicator3 on linux, please refer to your distro guides on how to install these packages if you need systray to run properly
+- Systray Icon: Depends on GTK 3+ and AppIndicator3 on Linux. Install these packages if you need systray to run properly.
 
 # Dependencies:
-- Python 3.7+: Tested with Python 3.10 on Windows and Ubuntu Linux
-- tkinter
-- [ffmpeg](https://www.ffmpeg.org/) : for merging audio with youtube DASH videos "it will be installed automatically on windows"
-- Fonts: (Linux X-server will raise an error if some fonts are missing especially emoji fonts, below are the 
-recommended fonts to be installed
+- Python 3.8+: Tested with Python 3.11+ on Windows 10 and Ubuntu Linux
+- [Tkinter](https://docs.python.org/3/library/tkinter.html): standard Python interface to the Tcl/Tk GUI toolkit.
+- [FFmpeg](https://www.ffmpeg.org/): for merging audio with DASH videos.
+- Fonts: (Linux X Server will raise an error if some fonts are missing, especially emoji fonts. Below are the 
+recommended fonts to be installed.
 
     ```
     ttf-linux-libertine 
     ttf-inconsolata 
     ttf-emojione
     ttf-symbola
     noto-fonts
     ```
-- [pycurl](http://pycurl.io/docs/latest/index.html): is a Python interface to libcurl / curl as our download engine,
-- [youtube_dl](https://github.com/ytdl-org/youtube-dl): famous youtube downloader, limited use for meta information extraction only but videos are downloaded using pycurl
-- [yt_dlp](https://github.com/yt-dlp/yt-dlp): a fork of youtube-dlc which is inturn a fork of youtube-dl
-- [certifi](https://github.com/certifi/python-certifi): required by 'pycurl' for validating the trustworthiness of SSL certificates,
-- [plyer](https://github.com/kivy/plyer): for systray area notification.
-- [awesometkinter](https://github.com/Aboghazala/AwesomeTkinter): for application gui.
-- [pillow](https://python-pillow.org/): imaging library for python
-- [pystray](https://github.com/moses-palmer/pystray): for systray icon
+- [PycURL](http://pycurl.io/docs/latest/index.html): a Python interface to libcurl, the multiprotocol file transfer library. Used as the download engine.
+- [youtube_dl](https://github.com/ytdl-org/youtube-dl): Famous YouTube downloader, limited use for meta information extraction only but videos are downloaded using PycURL.
+- [yt_dlp](https://github.com/yt-dlp/yt-dlp): yt-dlp is a youtube-dl fork based on the now inactive youtube-dlc.
+- [Certifi](https://github.com/certifi/python-certifi): required by PycURL for validating the trustworthiness of SSL certificates.
+- [Plyer](https://github.com/kivy/plyer): for systray area notification.
+- [AwesomeTkinter](https://github.com/Aboghazala/AwesomeTkinter): for application GUI.
+- [Pillow](https://python-pillow.org): the friendly PIL fork. PIL is an acronym for Python Imaging Library.
+- [pystray](https://github.com/moses-palmer/pystray): for systray icon.
 
 **Note for PycURL:**
 For Windows users who wants to run from source or use pip:
 Unfortunately, PycURL removed binary versions for Windows and it now has to be built from source. See here: http://pycurl.io/docs/latest/install.html#windows
-Normal pip install i.e `python -m pip install pycurl` probably will fail on Windows, your best choice is to use the VDM standalone/portable exe version.
-
-For Linux users:
-There is no issue since most Linux distros have cURL preinstalled. PycURL will link with the libcurl library and get built without issues. Checked with python version 3.10.
+`python -m pip install pycurl` will fail on Windows, your best choice is to use the portable version.
 
 # How to contribute to this project:
-1- By testing the application and opening [new issues](https://github.com/Sixline/VDM/issues/new) for bugs, feature requests, or suggestions.
+1- By testing the application and opening [new issues](https://github.com/Sixline/VortexDM/issues/new) for bugs, feature requests, or suggestions.
 
-2- Check the [Developer Guidelines](https://github.com/Sixline/VDM/blob/master/docs/developer_guide.md).
+2- Check the [Developer Guidelines](https://github.com/Sixline/VortexDM/blob/master/docs/developer_guide.md).
 
-3- Check [open issues](https://github.com/Sixline/VDM/issues?q=is%3Aopen+is%3Aissue) and see if you can help.
+3- Check [open issues](https://github.com/Sixline/VortexDM/issues?q=is%3Aopen+is%3Aissue) and see if you can help.
 
 4- Fork this repo and make a pull request.
 
 # Contributors:
-Please check [contributors.md](https://github.com/Sixline/VDM/blob/master/contributors.md) for a list of contributors.
+Please check [contributors.md](https://github.com/Sixline/VortexDM/blob/master/contributors.md) for a list of contributors.
```

### Comparing `vortexdm-2022.1.0/README.md` & `vortexdm-2023.1.0/vortexdm.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,178 +1,178 @@
-# Renaming the project to Vortex Download Manager and will carry on where FireDM 2022.2.5 left off. Original project, FireDM, by Mahmoud Elshahat. RIP
-
-The original creator removed the project repository from Github but left it on PyPI. The latest version they published there, 2022.4.14, I believe was purposely sabotaged to not work and anybody who accepted the update in FireDM would be left with the broken version. ~~If you want to install from PyPI install 2022.2.5 and don't update. https://pypi.org/project/FireDM/2022.2.5~~ 2022.2.5 is now gone from PyPI.
-
-Homepage: https://github.com/Sixline/VDM
-
-![GitHub All Releases](https://img.shields.io/github/downloads/Sixline/VDM/total?color=orange&label=GitHub%20Releases)
-
-![GitHub issues](https://img.shields.io/github/issues-raw/Sixline/VDM?color=brightgreen) - ![GitHub closed issues](https://img.shields.io/github/issues-closed-raw/Sixline/VDM?color=blueviolet)
-
-![Logo](https://raw.githubusercontent.com/Sixline/VDM/main/icons/vdm.png)
-Vortex Download Manager (VDM) is an open-source python Internet download manager with a high speed multi-connection engine. It downloads general files and videos from youtube and tons of other streaming websites.
-
-Developed in Python, based on "LibCurl", and "youtube_dl".
-
-**Features**:
-* High download speeds based on LibCurl
-* Multi-connection downloading
-* Automatic file segmentation
-* Automatic refresh for dead links
-* Resume uncompleted downloads
-* Support for Youtube, and a lot of other stream websites using youtube-dl to fetch info and libcurl to download media
-* Download entire video, playlist, or selected videos
-* Download fragmented video streams and encrypted/nonencrypted HLS media streams
-* Watch videos while downloading *some videos will have no audio until they finish downloading*
-* Download video subtitles
-* Write video metadata to downloaded files
-* Checking for application updates
-* Scheduled downloads
-* Re-using existing connections
-* Clipboard monitor
-* Proxy support (http, https, socks4, and socks5)
-* User/pass authentication, referee link, video thumbnail, and subtitles
-* Use custom cookie files
-* MD5 and SHA256 checksums
-* Custom GUI themes
-* Set download speed limit
-* Shell commands or computer shutdown on download completion
-* Control number of the concurrent downloads and maximum connections
-
-# How to use VDM:
-Running in command line: show help by typing `vdm -h`
-
-Running the GUI: Refer to the user guide at https://github.com/Sixline/VDM/blob/master/docs/user_guide.md
-
-# Portable VDM versions:
-  
-Run VDM without any installation (recommended) 
- - **Windows portable version** ([Download!](https://github.com/Sixline/VDM/releases/latest)):  
-   available in .zip format.  
-   unzip, and run from VDM.exe, no installation required.
-   
- - **Linux portable version** ([Download!](https://github.com/Sixline/VDM/releases/latest)):   
-   available in .AppImage format.  
-   download file, then mark it as executable, and run it, no installation required,
-   Tested on Ubuntu.
-   note: ffmpeg is not included and must be installed separately
-   
-   mark file as executable by right clicking the file> Properties> Permissions> Allow executing file as a program, or from terminal by `chmod +x VDM_xxx.AppImage`
-   
-   To check for ffmpeg use this command:
-   ```sh
-    which ffmpeg
-   
-    # expected output if installed
-    /usr/bin/ffmpeg
-   ```
-
-   if ffmpeg is missing you can install it by `sudo apt install ffmpeg` on debian based or `sudo pacman -S ffmpeg` on Arch based distros.
-
-## Manually installing VDM with pip (Linux Only):
-1- check python version (minimum version required is 3.7): `python3 --version`
-
-2- install required packages first:<br>
-- Linux, ubuntu:<br>
-```sh
-sudo apt install ffmpeg libcurl4-openssl-dev libssl-dev python3-pip python3-pil python3-pil.imagetk python3-tk python3-dbus gir1.2-appindicator3-0.1
-sudo apt install fonts-symbola fonts-linuxlibertine fonts-inconsolata fonts-emojione
-```
-
-3- install Vortex Download Manager using pip:<br>
-
-```sh
-python3 -m pip install vortexdm --user --upgrade --no-cache
-```
-
-## Running from source code inside virtual environment (Linux):
-1- check python version (minimum version required is 3.7): `python3 --version`
-
-2- install required packages first:
-- Linux, ubuntu:
-```sh
-sudo apt install ffmpeg libcurl4-openssl-dev libssl-dev python3-pip python3-pil python3-pil.imagetk python3-tk python3-dbus gir1.2-appindicator3-0.1
-sudo apt install fonts-symbola fonts-linuxlibertine fonts-inconsolata fonts-emojione
-```
-
-3- run below code to clone this repo, create virtual environment, install requirements, create launch script, and finally run VDM
-
-```sh
-git clone --depth 1 https://github.com/VDM/VDM.git
-python3 -m venv ./.env
-source ./.env/bin/activate
-python3 -m pip install -r ./VDM/requirements.txt
-echo "source ./.env/bin/activate
-python3 ./VDM/vdm.py \$@
-" > vdm.sh
-chmod +x ./vdm.sh
-./vdm.sh
-```
-
-> optionally create .desktop file and add VDM to your applications
-```sh
-VDMLSPATH=$(realpath ./vdm.sh)
-echo "[Desktop Entry]
-Name=Vortex Download Manager
-GenericName=VDM
-Comment=Vortex Download Manager
-Exec=$VDMLSPATH
-Icon=vdm
-Terminal=false
-Type=Application
-Categories=Network;
-Keywords=Internet;download
-" > VDM.desktop
-cp ./VDM.desktop ~/.local/share/applications/
-mkdir -p ~/.local/share/icons/hicolor/48x48/apps/
-cp ./VDM/icons/vdm.png ~/.local/share/icons/hicolor/48x48/apps/vdm.png
-```
-
-# Known Issues:
-- Linux X-server will raise an error if some fonts are missing especially emoji fonts - See Dependencies below
-
-- Mac - Tkinter, as mentioned in "python.org" the Apple-supplied Tcl/Tk 8.5 has serious bugs that can cause application crashes. If you wish to use Tkinter, do not use the Apple-supplied Pythons. Instead, install and use a newer version of Python from python.org or a third-party distributor that supplies or links with a newer version of Tcl/Tk.
-
-- systray icon: depends on Gtk+3 and AppIndicator3 on linux, please refer to your distro guides on how to install these packages if you need systray to run properly
-
-# Dependencies:
-- Python 3.7+: Tested with Python 3.10 on Windows and Ubuntu Linux
-- tkinter
-- [ffmpeg](https://www.ffmpeg.org/) : for merging audio with youtube DASH videos "it will be installed automatically on windows"
-- Fonts: (Linux X-server will raise an error if some fonts are missing especially emoji fonts, below are the 
-recommended fonts to be installed
-
-    ```
-    ttf-linux-libertine 
-    ttf-inconsolata 
-    ttf-emojione
-    ttf-symbola
-    noto-fonts
-    ```
-- [pycurl](http://pycurl.io/docs/latest/index.html): is a Python interface to libcurl / curl as our download engine,
-- [youtube_dl](https://github.com/ytdl-org/youtube-dl): famous youtube downloader, limited use for meta information extraction only but videos are downloaded using pycurl
-- [yt_dlp](https://github.com/yt-dlp/yt-dlp): a fork of youtube-dlc which is inturn a fork of youtube-dl
-- [certifi](https://github.com/certifi/python-certifi): required by 'pycurl' for validating the trustworthiness of SSL certificates,
-- [plyer](https://github.com/kivy/plyer): for systray area notification.
-- [awesometkinter](https://github.com/Aboghazala/AwesomeTkinter): for application gui.
-- [pillow](https://python-pillow.org/): imaging library for python
-- [pystray](https://github.com/moses-palmer/pystray): for systray icon
-
-**Note for PycURL:**
-For Windows users who wants to run from source or use pip:
-Unfortunately, PycURL removed binary versions for Windows and it now has to be built from source. See here: http://pycurl.io/docs/latest/install.html#windows
-Normal pip install i.e `python -m pip install pycurl` probably will fail on Windows, your best choice is to use the VDM standalone/portable exe version.
-
-For Linux users:
-There is no issue since most Linux distros have cURL preinstalled. PycURL will link with the libcurl library and get built without issues. Checked with python version 3.10.
-
-# How to contribute to this project:
-1- By testing the application and opening [new issues](https://github.com/Sixline/VDM/issues/new) for bugs, feature requests, or suggestions.
-
-2- Check the [Developer Guidelines](https://github.com/Sixline/VDM/blob/master/docs/developer_guide.md).
-
-3- Check [open issues](https://github.com/Sixline/VDM/issues?q=is%3Aopen+is%3Aissue) and see if you can help.
-
-4- Fork this repo and make a pull request.
-
-# Contributors:
-Please check [contributors.md](https://github.com/Sixline/VDM/blob/master/contributors.md) for a list of contributors.
+Metadata-Version: 2.1
+Name: vortexdm
+Version: 2023.1.0
+Summary: Vortex Download Manager
+Home-page: https://github.com/Sixline/VortexDM 
+Author: Mahmoud Elshahat
+Maintainer: Sixline
+Project-URL: Source, https://github.com/Sixline/VortexDM
+Project-URL: Tracker, https://github.com/Sixline/VortexDM/issues
+Project-URL: Releases, https://github.com/Sixline/VortexDM/releases
+Keywords: vortexdm vdm firedm internet download manager youtube hls pycurl curl youtube-dl tkinter
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+![Logo](https://raw.githubusercontent.com/Sixline/VortexDM/main/icons/vortexdm.png)
+Vortex Download Manager (VortexDM) is an open-source Python Internet download manager with a high speed multi-connection engine. It downloads general files and videos. Developed in Python, based on "PycURL" and "youtube_dl".
+
+Original project, FireDM, by Mahmoud Elshahat.
+
+Homepage: https://github.com/Sixline/VortexDM  
+PyPI Homepage: https://pypi.org/project/vortexdm
+
+[![GitHub Issues](https://img.shields.io/github/issues-raw/Sixline/VortexDM?color=brightgreen)](https://github.com/Sixline/VortexDM/issues) - [![GitHub Closed Issues](https://img.shields.io/github/issues-closed-raw/Sixline/VortexDM?color=blueviolet)](https://github.com/Sixline/VortexDM/issues?q=is%3Aissue+is%3Aclosed)
+
+**Features**:
+* High download speeds - based on PycURL
+* Multi-connection downloading
+* Automatic file segmentation
+* Automatic refresh for dead links
+* Resume uncompleted downloads
+* Support for YouTube and a lot of other stream websites using youtube-dl to fetch info and PycURL to download media
+* Download entire videos, playlists, or selected videos
+* Download fragmented video streams and encrypted/nonencrypted HLS media streams
+* Watch videos while downloading *some videos will have no audio until they finish downloading*
+* Download video subtitles
+* Write video metadata to downloaded files
+* Built-in updater
+* Scheduled downloads
+* Re-using existing connections
+* Clipboard monitor
+* Proxy support (http, https, socks4, and socks5)
+* User/pass authentication, referee link, video thumbnail, and subtitles
+* Use custom cookie files
+* MD5 and SHA256 checksums
+* Custom GUI themes
+* Set download speed limit
+* Shell commands or computer shutdown on download completion
+* Control number of the concurrent downloads and maximum connections
+
+# How to use VortexDM:
+Running in command line: show help by typing `vortexdm -h`
+
+Running the GUI: Refer to the user guide at https://github.com/Sixline/VortexDM/blob/master/docs/user_guide.md
+
+# Portable VortexDM Versions:
+  
+Run VortexDM without any installation (recommended) 
+ - **Windows Portable Version** ([Download!](https://github.com/Sixline/VortexDM/releases/latest)):  
+   Available in .zip format. Built with 64-bit Python 3.11+ and will only work on 64-bit Windows 10+.  
+   Unzip and run VortexDM-GUI.exe, no installation required.
+   
+ - **Linux Portable Version**  
+  Removing this section for now as I am not familiar with building AppImages. Will revisit.
+
+## Manually installing VortexDM with pip (Linux Only - Debian/Ubuntu Based Shown):
+1- Check python version (minimum version required is 3.8): `python3 --version`
+
+2- Install required packages:
+```sh
+sudo apt install ffmpeg libcurl4-openssl-dev libssl-dev python3-pip python3-pil python3-pil.imagetk python3-tk python3-dbus gir1.2-appindicator3-0.1
+sudo apt install fonts-symbola fonts-linuxlibertine fonts-inconsolata fonts-emojione
+```
+
+3- Install Vortex Download Manager using pip:
+
+```sh
+python3 -m pip install vortexdm --user --upgrade --no-cache
+```
+
+## Running from source code inside a Python virtual environment (Linux Only - Debian/Ubuntu Based Shown):
+1- Check python version (minimum version required is 3.8): `python3 --version`
+
+2- Install required packages:
+```sh
+sudo apt install ffmpeg libcurl4-openssl-dev libssl-dev python3-pip python3-pil python3-pil.imagetk python3-tk python3-dbus gir1.2-appindicator3-0.1
+sudo apt install fonts-symbola fonts-linuxlibertine fonts-inconsolata fonts-emojione
+```
+
+3- Run below code to do the following:  
+  * Clone this repo  
+  * Create Python virtual environment  
+  * Install the requirements  
+  * Create launch script  
+  * Run VortexDM
+
+```sh
+git clone https://github.com/Sixline/VortexDM
+python3 -m venv ./.env
+source ./.env/bin/activate
+python3 -m pip install -r ./VortexDM/requirements.txt
+echo "source ./.env/bin/activate
+python3 ./VortexDM/vortexdm.py \$@ " > vortexdm.sh
+chmod +x ./vortexdm.sh
+./vortexdm.sh
+```
+
+> Optionally create .desktop file and add VortexDM to your applications
+```sh
+VortexDMLSPATH=$(realpath ./vortexdm.sh)
+echo "[Desktop Entry]
+Name=VortexDM
+GenericName=VortexDM
+Comment=Vortex Download Manager
+Exec=$VortexDMLSPATH
+Icon=vortexdm
+Terminal=false
+Type=Application
+Categories=Network;
+Keywords=Internet;download
+" > VortexDM.desktop
+cp ./VortexDM.desktop ~/.local/share/applications/
+mkdir -p ~/.local/share/icons/hicolor/48x48/apps/
+cp ./VortexDM/icons/vortexdm.png ~/.local/share/icons/hicolor/48x48/apps/vortexdm.png
+```
+
+# Known Issues:
+- Linux X Server will raise an error if some fonts are missing, especially emoji fonts - See Dependencies below
+
+- Mac - Tkinter - Can have issues depending on versions. See here: https://www.python.org/download/mac/tcltk
+
+- Systray Icon: Depends on GTK 3+ and AppIndicator3 on Linux. Install these packages if you need systray to run properly.
+
+# Dependencies:
+- Python 3.8+: Tested with Python 3.11+ on Windows 10 and Ubuntu Linux
+- [Tkinter](https://docs.python.org/3/library/tkinter.html): standard Python interface to the Tcl/Tk GUI toolkit.
+- [FFmpeg](https://www.ffmpeg.org/): for merging audio with DASH videos.
+- Fonts: (Linux X Server will raise an error if some fonts are missing, especially emoji fonts. Below are the 
+recommended fonts to be installed.
+
+    ```
+    ttf-linux-libertine 
+    ttf-inconsolata 
+    ttf-emojione
+    ttf-symbola
+    noto-fonts
+    ```
+- [PycURL](http://pycurl.io/docs/latest/index.html): a Python interface to libcurl, the multiprotocol file transfer library. Used as the download engine.
+- [youtube_dl](https://github.com/ytdl-org/youtube-dl): Famous YouTube downloader, limited use for meta information extraction only but videos are downloaded using PycURL.
+- [yt_dlp](https://github.com/yt-dlp/yt-dlp): yt-dlp is a youtube-dl fork based on the now inactive youtube-dlc.
+- [Certifi](https://github.com/certifi/python-certifi): required by PycURL for validating the trustworthiness of SSL certificates.
+- [Plyer](https://github.com/kivy/plyer): for systray area notification.
+- [AwesomeTkinter](https://github.com/Aboghazala/AwesomeTkinter): for application GUI.
+- [Pillow](https://python-pillow.org): the friendly PIL fork. PIL is an acronym for Python Imaging Library.
+- [pystray](https://github.com/moses-palmer/pystray): for systray icon.
+
+**Note for PycURL:**
+For Windows users who wants to run from source or use pip:
+Unfortunately, PycURL removed binary versions for Windows and it now has to be built from source. See here: http://pycurl.io/docs/latest/install.html#windows
+`python -m pip install pycurl` will fail on Windows, your best choice is to use the portable version.
+
+# How to contribute to this project:
+1- By testing the application and opening [new issues](https://github.com/Sixline/VortexDM/issues/new) for bugs, feature requests, or suggestions.
+
+2- Check the [Developer Guidelines](https://github.com/Sixline/VortexDM/blob/master/docs/developer_guide.md).
+
+3- Check [open issues](https://github.com/Sixline/VortexDM/issues?q=is%3Aopen+is%3Aissue) and see if you can help.
+
+4- Fork this repo and make a pull request.
+
+# Contributors:
+Please check [contributors.md](https://github.com/Sixline/VortexDM/blob/master/contributors.md) for a list of contributors.
```

### Comparing `vortexdm-2022.1.0/setup.py` & `vortexdm-2023.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """
-    Vortex Download Manager (VDM)
+    Vortex Download Manager (VortexDM)
 
-    Multi-connection internet download manager, based on "LibCurl", and "youtube_dl". Original project, FireDM, by Mahmoud Elshahat.
-    :copyright: (c) 2022 by Sixline
+    A multi-connection internet download manager, based on "PycURL" and "youtube_dl". Original project, FireDM, by Mahmoud Elshahat.
+    :copyright: (c) 2023 by Sixline
     :copyright: (c) 2019-2021 by Mahmoud Elshahat.
     :license: GNU GPLv3, see LICENSE.md for more details.
 """
 
 import os
 import setuptools
 
 # get current directory
 path = os.path.realpath(os.path.abspath(__file__))
 current_directory = os.path.dirname(path)
 
 # get version
 version = {}
-with open(f"{current_directory}/vdm/version.py") as f:
+with open(f"{current_directory}/vortexdm/version.py") as f:
     exec(f.read(), version)  # then we can use it as: version['__version__']
 
 # get long description from readme
 with open(f"{current_directory}/README.md", "r") as fh:
     long_description = fh.read()
 
 try:
@@ -29,38 +29,37 @@
 except:
     requirements = ['plyer', 'certifi', 'youtube_dl', 'yt_dlp', 'pycurl', 'pillow >= 6.0.0', 'pystray',
                     'awesometkinter >= 2021.3.19']
 
 setuptools.setup(
     name="vortexdm",
     version=version['__version__'],
-    scripts=[],  # ['VDM.py'], no need since added an entry_points
+    scripts=[],  # ['VortexDM.py'], no need since added an entry_points
     author="Mahmoud Elshahat",
     maintainer="Sixline",
     description="Vortex Download Manager",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/Sixline/VDM ",
+    url="https://github.com/Sixline/VortexDM ",
     packages=setuptools.find_packages(),
-    keywords="vdm firedm internet download manager youtube hls pycurl curl youtube-dl tkinter",
+    keywords="vortexdm vdm firedm internet download manager youtube hls pycurl curl youtube-dl tkinter",
     project_urls={
-        'Source': 'https://github.com/Sixline/VDM',
-        'Tracker': 'https://github.com/Sixline/VDM/issues',
-        'Releases': 'https://github.com/Sixline/VDM/releases',
-#        'Screenshots': 'https://github.com/firedm/FireDM/issues/13#issuecomment-689337428'
+        'Source': 'https://github.com/Sixline/VortexDM',
+        'Tracker': 'https://github.com/Sixline/VortexDM/issues',
+        'Releases': 'https://github.com/Sixline/VortexDM/releases',
     },
     install_requires=requirements,
     entry_points={
         # our executable: "exe file on windows for example"
         'console_scripts': [
-            'vdm = vdm.VDM:main',
+            'vortexdm = vortexdm.VortexDM:main',
         ]},
     classifiers=[
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.7',
+    python_requires='>=3.8',
 )
```

### Comparing `vortexdm-2022.1.0/vdm/VDM.py` & `vortexdm-2023.1.0/vortexdm/VortexDM.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 """
-    Vortex Download Manager (VDM)
+    Vortex Download Manager (VortexDM)
 
-    Multi-connection internet download manager, based on "LibCurl", and "youtube_dl". Original project, FireDM, by Mahmoud Elshahat.
-    :copyright: (c) 2022 by Sixline
+    A multi-connection internet download manager, based on "PycURL" and "youtube_dl". Original project, FireDM, by Mahmoud Elshahat.
+    :copyright: (c) 2023 by Sixline
     :copyright: (c) 2019-2021 by Mahmoud Elshahat.
     :license: GNU GPLv3, see LICENSE.md for more details.
 
     Module description:
         This is main application module
 """
 
@@ -15,22 +15,22 @@
 import os
 import subprocess
 import sys
 import argparse
 import re
 import signal
 
-# This code should stay on top to handle relative imports in case of direct call of VDM.py
+# This code should stay on top to handle relative imports in case of direct call of VortexDM.py
 if __package__ is None:
     path = os.path.realpath(os.path.abspath(__file__))
     sys.path.insert(0, os.path.dirname(path))
     sys.path.insert(0, os.path.dirname(os.path.dirname(path)))
     
-    __package__ = 'vdm'
-    import vdm
+    __package__ = 'vortexdm'
+    import vortexdm
 
 
 # local modules
 from . import config, setting
 from .controller import Controller
 from .tkview import MainWindow
 from .cmdview import CmdView
@@ -41,19 +41,20 @@
 
 def pars_args(arguments):
     """parse arguments vector
     Args:
         arguments(list): list contains arguments, could be sys.argv[1:] i.e. without script name
     """
 
-    description = """Vortex Download Manager (VDM) is an open-source python Internet download manager
-        with a high speed multi-connection engine. It downloads general files and videos from youtube 
-        and tons of other streaming websites. 
-        Developed in Python, based on "LibCurl", "youtube_dl", and "Tkinter". 
-        Source: https://github.com/Sixline/VDM """
+    description = """Vortex Download Manager (VortexDM) - An open-source Python 
+        Internet download manager with a high speed multi-connection engine. It 
+        downloads general files and videos. 
+        Developed in Python, based on "PycURL" and "youtube_dl".
+        GNU GPLv3, see LICENSE.md for more details. 
+        Source: https://github.com/Sixline/VortexDM"""
 
     def iterable(txt):
         # process iterable in arguments, e.g. tuple or list,
         # example --window=(600,300)
         return re.findall(r'\d+', txt)
 
     def int_iterable(txt):
@@ -65,19 +66,19 @@
     # region cmdline arguments
     # some args' names are taken from youtube-dl, reference:
     # https://github.com/ytdl-org/youtube-dl/blob/master/youtube_dl/options.py
     # Note: we should use "default=argparse.SUPPRESS" to discard option if not used by user,
     # and prevent default value overwrite in config module
 
     parser = argparse.ArgumentParser(
-        prog='vdm',
+        prog='vortexdm',
         description=description,
         epilog='copyright: (c) 2022 Vortex Download Manager. license: GNU GPLv3, see LICENSE.md file for more details.'
                'Original project, FireDM, by Mahmoud Elshahat'
-               'Isuues: https://github.com/Sixline/VDM/issues',
+               'Isuues: https://github.com/Sixline/VortexDM/issues',
         usage='\n'
               '%(prog)s [OPTIONS] URL1 URL2 URL3 \n'
               'example: %(prog)s "https://somesite.com/somevideo" "https://somesite.com/anothervideo"\n'
               'Note: to run %(prog)s in GUI(Graphical User Interface) mode, use "--gui" option along with other '
               'arguments, or start %(prog)s without any arguments.',
         add_help=False
     )
@@ -91,29 +92,29 @@
     general = parser.add_argument_group(title='General options')
     general.add_argument(
         '-h', '--help',
         action='help',
         help='show this help message and exit')
     general.add_argument(
         '-v', '--version',
-        action='version', version='VDM version: ' + __version__,
+        action='version', version='VortexDM Version: ' + __version__,
         help='Print program version and exit')
     general.add_argument(
         '--show-settings',
         action='store_true', default=argparse.SUPPRESS,
         help='show current application settings and their current values and exit')
     general.add_argument(
         '--edit-config', dest='edit_config',
         type=str, metavar='EDITOR', default=argparse.SUPPRESS,
         action='store', nargs='?', const='nano',  # const if use argument without value
         help='Edit config file, you should specify your text editor executable, otherwise "nano" will be used')
     general.add_argument(
         '--ignore-config', dest='ignore_config', default=argparse.SUPPRESS,
         action='store_true',
-        help='Do not load settings from config file. in ~/.config/VDM/ or (APPDATA/VDM/ on Windows)')
+        help='Do not load settings from config file. in ~/.config/VortexDM/ or (APPDATA/VortexDM/ on Windows)')
     general.add_argument(
         '--dlist', dest='ignore_dlist',
         action='store_false', default=argparse.SUPPRESS,
         help='load/save "download list" from/to  d-list config file. '
              'default="False in cmdline mode and True in GUI mode"')
     general.add_argument(
         '--ignore-dlist', dest='ignore_dlist',
@@ -241,15 +242,15 @@
         help='Don\'t calculate checksums')
 
     # -------------------------------------------------------------------------------------Application Update Options---
     appupdate = parser.add_argument_group(title='Application Update Options')
     appupdate.add_argument(
         '--update',
         action='store_true', dest='update_self', default=argparse.SUPPRESS,
-        help='Update this Application and video libraries to latest version.')
+        help='Update this application and video libraries to latest version.')
 
     # -------------------------------------------------------------------------------------Downloader Options-----------
     downloader = parser.add_argument_group(title='Downloader Options')
     downloader.add_argument(
         '-R', '--retries', dest='refresh_url_retries',
         type=int, metavar='RETRIES', default=argparse.SUPPRESS,
         help=f'Number of retries to download a file, default="{config.refresh_url_retries}".')
```

### Comparing `vortexdm-2022.1.0/vdm/__main__.py` & `vortexdm-2023.1.0/vortexdm/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #!/usr/bin/env python3
 """
-    Vortex Download Manager (VDM)
+    Vortex Download Manager (VortexDM)
 
-    Multi-connection internet download manager, based on "LibCurl", and "youtube_dl". Original project, FireDM, by Mahmoud Elshahat.
-    :copyright: (c) 2022 by Sixline
+    A multi-connection internet download manager, based on "PycURL" and "youtube_dl". Original project, FireDM, by Mahmoud Elshahat.
+    :copyright: (c) 2023 by Sixline
     :copyright: (c) 2019-2021 by Mahmoud Elshahat.
     :license: GNU GPLv3, see LICENSE.md for more details.
 """
 # main module executed when run command
-# python -m vdm
+# python -m vortexdm
 
 import sys
 
 if __package__ is None and not hasattr(sys, 'frozen'):
     # direct call of __main__.py
     import os.path
     path = os.path.realpath(os.path.abspath(__file__))
     sys.path.insert(0, os.path.dirname(os.path.dirname(path)))
 
-from vdm import VDM
+from vortexdm import VortexDM
 
 if __name__ == '__main__':
-    VDM.main()
+    VortexDM.main()
```

### Comparing `vortexdm-2022.1.0/vdm/brain.py` & `vortexdm-2023.1.0/vortexdm/brain.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
-    Vortex Download Manager (VDM)
+    Vortex Download Manager (VortexDM)
 
-    Multi-connection internet download manager, based on "LibCurl", and "youtube_dl". Original project, FireDM, by Mahmoud Elshahat.
-    :copyright: (c) 2022 by Sixline
+    A multi-connection internet download manager, based on "PycURL" and "youtube_dl". Original project, FireDM, by Mahmoud Elshahat.
+    :copyright: (c) 2023 by Sixline
     :copyright: (c) 2019-2021 by Mahmoud Elshahat.
     :license: GNU GPLv3, see LICENSE.md for more details.
 """
 import os
 import time
 from threading import Thread
 from queue import Queue
```

### Comparing `vortexdm-2022.1.0/vdm/cmdview.py` & `vortexdm-2023.1.0/vortexdm/cmdview.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
-    Vortex Download Manager (VDM)
+    Vortex Download Manager (VortexDM)
 
-    Multi-connection internet download manager, based on "LibCurl", and "youtube_dl". Original project, FireDM, by Mahmoud Elshahat.
-    :copyright: (c) 2022 by Sixline
+    A multi-connection internet download manager, based on "PycURL" and "youtube_dl". Original project, FireDM, by Mahmoud Elshahat.
+    :copyright: (c) 2023 by Sixline
     :copyright: (c) 2019-2021 by Mahmoud Elshahat.
     :license: GNU GPLv3, see LICENSE.md for more details.
 
     Module description:
         This is a command line / Terminal view, as a layer between user and controller
         it must inherit from IView and implement all its abstract methods, see view.py
         currently it runs in interactive mode and not suitable for automated jobs.
@@ -17,20 +17,20 @@
 import sys
 import shutil
 from queue import Queue
 from threading import Event
 from collections import namedtuple
 
 if not __package__:
-    __package__ = 'vdm'
+    __package__ = 'vortexdm'
 
-from vdm.view import IView
-from vdm import utils
-from vdm.utils import format_bytes, format_seconds
-from vdm import config
+from vortexdm.view import IView
+from vortexdm import utils
+from vortexdm.utils import format_bytes, format_seconds
+from vortexdm import config
 
 
 def write(s, end=''):
     sys.stdout.write(s + end)
     sys.stdout.flush()
```

### Comparing `vortexdm-2022.1.0/vdm/config.py` & `vortexdm-2023.1.0/vortexdm/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
-    Vortex Download Manager (VDM)
+    Vortex Download Manager (VortexDM)
 
-    Multi-connection internet download manager, based on "LibCurl", and "youtube_dl". Original project, FireDM, by Mahmoud Elshahat.
-    :copyright: (c) 2022 by Sixline
+    A multi-connection internet download manager, based on "PycURL" and "youtube_dl". Original project, FireDM, by Mahmoud Elshahat.
+    :copyright: (c) 2023 by Sixline
     :copyright: (c) 2019-2021 by Mahmoud Elshahat.
     :license: GNU GPLv3, see LICENSE.md for more details.
 """
 
 from queue import Queue
 import os
 import sys
@@ -27,28 +27,28 @@
     'video_title_template', 'ffmpeg_actual_path'
 ]
 
 # ----------------------------------------------------------------------------------------General ----------------------
 # CONSTANTS
 APP_NAME = 'Vortex Download Manager'
 APP_VERSION = __version__
-APP_TITLE = f'{APP_NAME} version {APP_VERSION} .. an open-source download manager'
+APP_TITLE = f'{APP_NAME} Version {APP_VERSION} .. an open-source download manager'
 
 # minimum segment size used in auto-segmentation process, refer to brain.py>thread_manager.
 SEGMENT_SIZE = 1024 * 100  # 100 KB
 
-APP_URL = 'https://github.com/Sixline/VDM'
-LATEST_RELEASE_URL = 'https://github.com/Sixline/VDM/releases/latest'
+APP_URL = 'https://github.com/Sixline/VortexDM'
+LATEST_RELEASE_URL = 'https://github.com/Sixline/VortexDM/releases/latest'
 
 FROZEN = getattr(sys, "frozen", False)  # check if app is being compiled by cx_freeze
 
 operating_system = platform.system()  # current operating system  ('Windows', 'Linux', 'Darwin')
 
 # Example output: Os: Linux - Platform: Linux-5.11.0-7614-generic-x86_64-with-glibc2.32 - Machine: x86_64
-operating_system_info = f"Os: {platform.system()} - Platform: {platform.platform()} - Machine: {platform.machine()}"
+operating_system_info = f"OS: {platform.system()} - Platform: {platform.platform()} - Machine: {platform.machine()}"
 
 try:
     import distro
 
     # Example output: Distribution: ('Pop!_OS', '20.10', 'groovy')
     operating_system_info += f"\nDistribution: {distro.linux_distribution(full_distribution_name=True)}"
 except:
```

### Comparing `vortexdm-2022.1.0/vdm/controller.py` & `vortexdm-2023.1.0/vortexdm/controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
-    Vortex Download Manager (VDM)
+    Vortex Download Manager (VortexDM)
 
-    Multi-connection internet download manager, based on "LibCurl", and "youtube_dl". Original project, FireDM, by Mahmoud Elshahat.
-    :copyright: (c) 2022 by Sixline
+    A multi-connection internet download manager, based on "PycURL" and "youtube_dl". Original project, FireDM, by Mahmoud Elshahat.
+    :copyright: (c) 2023 by Sixline
     :copyright: (c) 2019-2021 by Mahmoud Elshahat.
     :license: GNU GPLv3, see LICENSE.md for more details.
 
     module description:
         This is the controller module as a part of MVC design, which will replace the old application design
         in attempt to isolate logic from gui / view
         old design has gui and logic mixed together
@@ -34,15 +34,14 @@
 from . import config
 from .config import Status, MediaType
 from .brain import brain
 from . import video
 from .video import get_media_info, process_video
 from .model import ObservableDownloadItem, ObservableVideo
 
-
 def set_option(**kwargs):
     """set global setting option(s) in config.py"""
     try:
         config.__dict__.update(kwargs)
         # log('Settings:', kwargs)
     except:
         pass
@@ -102,21 +101,21 @@
         cmd = f'"{config.ffmpeg_actual_path}" -version'
         error, out = run_command(cmd, verbose=False, striplines=False)
         if not error:
             try:
                 # ffmpeg version 4.3.2-0+deb11u1ubuntu1 Copyright (c) 2000-2021 the FFmpeg developers
                 match = re.match(r'ffmpeg version (.*?) Copyright', out, re.IGNORECASE)
                 config.ffmpeg_version = match.groups()[0]
-                msg += f', version: {config.ffmpeg_version}'
+                msg += f', Version: {config.ffmpeg_version}'
             except:
                 pass
         log(msg, log_level=2)
         return True
     else:
-        log(f'can not find ffmpeg!!, install it, or add executable location to PATH, or copy executable to ',
+        log(f'Can not find ffmpeg! Install it, add executable location to PATH, or copy executable to ',
             config.global_sett_folder, 'or', config.current_directory)
 
 
 def write_timestamp(d):
     """write server timestamp to downloaded file
 
     try to figure out the timestamp of the remote file, and if available make
@@ -197,28 +196,28 @@
         log('controller._download_thumbnail()> error:', e)
         if config.test_mode:
             raise e
 
 
 def log_runtime_info():
     """Print useful information about the system"""
-    log('-' * 20, 'VDM', '-' * 20)
+    log('-' * 20, 'VortexDM', '-' * 20)
 
     if config.isappimage:
         release_type = 'AppImage'
     elif config.FROZEN:
         release_type = 'Frozen'
     else:
         release_type = 'Non-Frozen'
 
-    log('Starting VDM version:', config.APP_VERSION, release_type)
-    log('operating system:', config.operating_system_info)
-    log('Python version:', sys.version)
-    log('current working directory:', config.current_directory)
-    log(f'FFMPEG: {config.ffmpeg_actual_path}, version: {config.ffmpeg_version}')
+    log('Starting VortexDM Version:', config.APP_VERSION, release_type)
+    log('Operating System:', config.operating_system_info)
+    log('Python Version:', sys.version)
+    log('Current working directory:', config.current_directory)
+    log(f'FFmpeg: {config.ffmpeg_actual_path}, Version: {config.ffmpeg_version}')
 
 
 def create_video_playlist(url, ytdloptions=None, interrupt=False):
     """Process url and build video object(s) and return a video playlist"""
 
     log('creating video playlist', log_level=2)
     playlist = []
@@ -786,25 +785,25 @@
 
                 if not silent and config.operating_system == 'Windows':
                     res = self.get_user_response(popup_id=2)
                     if res == 'Download':
                         # download ffmpeg from github
                         self._download_ffmpeg()
                 else:
-                    log('FFMPEG is missing', start='', showpopup=showpopup)
+                    log('FFmpeg is missing.', start='', showpopup=showpopup)
 
                 return False
 
         # in case of missing download folder value will fallback to current download folder
         folder = d.folder or config.download_folder
 
         # validate destination folder for existence and permissions
         try:
             # write test file to download folder
-            test_file_path = os.path.join(folder, 'test_file_.VDM')
+            test_file_path = os.path.join(folder, 'test_file_.VortexDM')
             # skip test in case test_file already created by another thread
             if not os.path.isfile(test_file_path):
                 with open(test_file_path, 'w') as f:
                     f.write('0')
                 delete_file(test_file_path)
 
             # update download item
@@ -1013,36 +1012,60 @@
     def _download_ffmpeg(self, destination=config.sett_folder):
         """download ffmpeg.exe for windows os
 
         Args:
             destination (str): download folder
 
         """
+        import shutil
+        import time
+        import platform
 
         # set download folder
         config.ffmpeg_download_folder = destination
 
         # first check windows 32 or 64
-        import platform
         # ends with 86 for 32 bit and 64 for 64 bit i.e. Win7-64: AMD64 and Vista-32: x86
         if platform.machine().endswith('64'):
             # 64 bit link
-            url = 'https://github.com/Sixline/VDM/releases/download/extra/ffmpeg_64bit.exe'
+            url = 'https://github.com/BtbN/FFmpeg-Builds/releases/download/latest/ffmpeg-master-latest-win64-gpl.zip'
         else:
-            # 32 bit link
-            url = 'https://github.com/Sixline/VDM/releases/download/extra/ffmpeg_32bit.exe'
+            # 32 bit - BtbN doesn't auto-build a 32-bit version.
+            log('BtbN doesn\'t auto-build a 32-bit version of FFmpeg.exe. You will need to source a version yourself. :(', showpopup=True)
+            return
 
-        log('downloading: ', url)
+        log('Downloading ffmpeg, please wait for it to complete.', showpopup=True)
+        log('Downloading: ', url,)
 
         # create a download object, will save ffmpeg in setting folder
         d = ObservableDownloadItem(url=url, folder=config.ffmpeg_download_folder)
         d.update(url)
-        d.name = 'ffmpeg.exe'
+        d.name = 'ffmpeg-master-latest-win64-gpl.zip'
+
+        self.download(d, silent=False)
+
+        ffmpeg_zip_path = os.path.join(config.ffmpeg_download_folder, 'ffmpeg-master-latest-win64-gpl.zip')
 
-        self.download(d, silent=True)
+        # check if downloaded zip file exists
+        while not os.path.isfile(ffmpeg_zip_path):
+            log('Waiting for download to complete...')
+            time.sleep(3)
+
+        # extract zip, move ffmpeg.exe from extracted folder, delete zip file and extracted folder
+        
+        log('Download done! Extracting and moving ffmpeg.exe...')
+        
+        ffmpeg_extract_path = os.path.join(config.ffmpeg_download_folder, 'ffmpeg-master-latest-win64-gpl')
+        ffmpeg_path = os.path.join(ffmpeg_extract_path, 'ffmpeg-master-latest-win64-gpl', 'bin', 'ffmpeg.exe')
+        zip_extract(z_fp=ffmpeg_zip_path, extract_folder=ffmpeg_extract_path)
+        shutil.move(ffmpeg_path, os.path.join(config.ffmpeg_download_folder, 'ffmpeg.exe'))
+        log('Cleaning up...')
+        delete_folder(ffmpeg_extract_path, verbose=True)
+        delete_file(ffmpeg_zip_path, verbose=True)
+        log('ffmpeg.exe downloaded! Retry your download.', showpopup=True)
 
     def autodownload(self, url, **kwargs):
         """download file automatically without user intervention
         for video files it should download best quality, for video playlist, it will download first video
         """
 
         stream_options = kwargs.setdefault('stream_options', {})
@@ -1094,15 +1117,15 @@
             time.sleep(0.5)
 
     # endregion
 
     # region Application update
     @threaded
     def check_for_update(self, signal_id=None, wait=False, timeout=30, **kwargs):
-        """check for newer version of VDM, youtube-dl, and yt_dlp
+        """check for newer version of VortexDM, youtube-dl, and yt_dlp
         Args:
             signal_id(any): signal a view when this function done
             wait(bool): wait for youtube-dl and ytdlp to load
             timeout(int): timeout for above wait in seconds
         """
 
         # parse youtube-dl and yt_dlp versions manually (if importing still in progress)
@@ -1111,22 +1134,22 @@
 
         if not config.yt_dlp_version:
             config.yt_dlp_version = get_pkg_version('yt_dlp')
 
         if wait:
             c = 1
             while config.youtube_dl_version is None or config.yt_dlp_version is None:
-                log('\ryoutube-dl and ytdlp still loading, please wait', '.' * c, end='')
+                log('\ryoutube-dl and yt_dlp still loading, please wait', '.' * c, end='')
                 c += 1
                 if c > timeout:
                     break
                 time.sleep(1)
             log()
 
-        info = {'vdm': {'current_version': config.APP_VERSION, 'latest_version': None},
+        info = {'vortexdm': {'current_version': config.APP_VERSION, 'latest_version': None},
                 'youtube_dl': {'current_version': config.youtube_dl_version, 'latest_version': None},
                 'yt_dlp': {'current_version': config.yt_dlp_version, 'latest_version': None},
                 'awesometkinter': {'current_version': config.atk_version, 'latest_version': None},
                 }
 
         def fetch_pypi(pkg):
             pkg_info = info[pkg]
@@ -1144,15 +1167,15 @@
             t.start()
             time.sleep(0.1)
 
         for t in threads:
             t.join()
 
         # update
-        msg = 'Check for update Status:\n\n'
+        msg = 'Update Status:\n\n'
         new_pkgs = []
         for pkg in pkgs:
             pkg_info = info[pkg]
             current_version = pkg_info['current_version']
             latest_version = pkg_info['latest_version']
 
             if current_version is None:
@@ -1165,36 +1188,36 @@
             else:
                 msg += f'    {pkg}: up to date!\n\n'
 
         if new_pkgs:
             msg += 'Do you want to update now? \n'
             options = ['Update', 'Cancel']
 
-            # show update notes for vdm
-            if 'vdm' in new_pkgs:
-                log('getting VDM changelog ....')
+            # show update notes for vortexdm
+            if 'vortexdm' in new_pkgs:
+                log('getting VortexDM changelog ....')
 
                 # download change log file
-                url = 'https://github.com/Sixline/VDM/raw/master/ChangeLog.txt'
+                url = 'https://github.com/Sixline/VortexDM/raw/master/ChangeLog.txt'
                 changelog = download(url, verbose=False)
 
                 # verify server didn't send html page
                 if changelog and '<!DOCTYPE html>' not in changelog:
                     msg += '\n\n\n'
-                    msg += 'VDM Change Log:\n'
+                    msg += 'VortexDM Change Log:\n'
                     msg += changelog
 
             res = self.get_user_response(msg, options)
             if res == options[0]:
 
                 # check write permission
-                tf = update.get_target_folder('vdm')
+                tf = update.get_target_folder('vortexdm')
                 if tf and not check_write_permission(tf):
                     log('Permission error:',
-                        'Run VDM as admin to install updates', showpopup=True)
+                        'Run VortexDM as admin to install updates', showpopup=True)
                     return
 
                 # start updating modules
                 done_pkgs = {}
                 for pkg in new_pkgs:
                     pkg_info = info[pkg]
                     latest_version, url = pkg_info['latest_version'], pkg_info['url']
@@ -1226,44 +1249,44 @@
             self._update_view(command='signal', signal_id=signal_id)
 
         today = date.today()
         config.last_update_check = (today.year, today.month, today.day)
 
     @threaded
     def auto_check_for_update(self):
-        """auto check for vdm update"""
+        """auto check for vortexdm update"""
         if config.check_for_update and not config.disable_update_feature:
             today = date.today()
 
             if update.parse_version(config.APP_VERSION) > update.parse_version(config.updater_version):
                 config.last_update_check = (today.year, today.month, today.day)
                 config.updater_version = config.APP_VERSION
-                # log('Running newer VDM version, reset last_update_check')
+                # log('Running newer VortexDM version, reset last_update_check')
 
             else:
                 try:
                     last_check = date(*config.last_update_check)
                 except:
                     last_check = today
                     config.last_update_check = (today.year, today.month, today.day)
 
                 delta = today - last_check
                 if delta.days >= config.update_frequency:
-                    res = self.get_user_response(f'Check for VDM update?\nLast check was {delta.days} days ago',
+                    res = self.get_user_response(f'Check for VortexDM update?\nLast check was {delta.days} days ago',
                                                  options=['Ok', 'Cancel'])
                     if res == 'Ok':
                         self.check_for_update()
 
     def rollback_pkg_update(self, pkg):
         try:
             # check write permission
             tf = update.get_target_folder(pkg)
             if tf and not check_write_permission(tf):
                 log('Permission error:',
-                    'Run VDM as admin to rollback updates', showpopup=True)
+                    'Run VortexDM as admin to rollback updates', showpopup=True)
                 return
 
             run_thread(update.rollback_pkg_update, pkg, daemon=True)
         except Exception as e:
             log(f'failed to restore {pkg}:', e)
 
     # endregion
```

### Comparing `vortexdm-2022.1.0/vdm/dependency.py` & `vortexdm-2023.1.0/vortexdm/dependency.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 """
-    Vortex Download Manager (VDM)
+    Vortex Download Manager (VortexDM)
 
-    Multi-connection internet download manager, based on "LibCurl", and "youtube_dl". Original project, FireDM, by Mahmoud Elshahat.
-    :copyright: (c) 2022 by Sixline
+    A multi-connection internet download manager, based on "PycURL" and "youtube_dl". Original project, FireDM, by Mahmoud Elshahat.
+    :copyright: (c) 2023 by Sixline
     :copyright: (c) 2019-2021 by Mahmoud Elshahat.
     :license: GNU GPLv3, see LICENSE.md for more details.
 """
 
 # The purpose of this module is checking and auto installing dependencies
 import sys
 import subprocess
```

### Comparing `vortexdm-2022.1.0/vdm/downloaditem.py` & `vortexdm-2023.1.0/vortexdm/downloaditem.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
-    Vortex Download Manager (VDM)
+    Vortex Download Manager (VortexDM)
 
-    Multi-connection internet download manager, based on "LibCurl", and "youtube_dl". Original project, FireDM, by Mahmoud Elshahat.
-    :copyright: (c) 2022 by Sixline
+    A multi-connection internet download manager, based on "PycURL" and "youtube_dl". Original project, FireDM, by Mahmoud Elshahat.
+    :copyright: (c) 2023 by Sixline
     :copyright: (c) 2019-2021 by Mahmoud Elshahat.
     :license: GNU GPLv3, see LICENSE.md for more details.
 """
 
 # Download Item Class
 
 import os
@@ -398,15 +398,15 @@
         self._name = validate_file_name(new_value)
 
         self.title, self.extension = os.path.splitext(self._name)
 
     @property
     def temp_folder(self):
         fp = self.alternative_temp_folder if os.path.isdir(self.alternative_temp_folder) else self.folder
-        name = f'vdm_{self.uid}'
+        name = f'vortexdm_{self.uid}'
         return os.path.join(fp, name)
 
     @property
     def target_file(self):
         """return file name including path"""
         return os.path.join(self.folder, self.name)
```

### Comparing `vortexdm-2022.1.0/vdm/iconsbase64.py` & `vortexdm-2023.1.0/vortexdm/iconsbase64.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+"""
+    Vortex Download Manager (VortexDM)
+
+    A multi-connection internet download manager, based on "PycURL" and "youtube_dl". Original project, FireDM, by Mahmoud Elshahat.
+    :copyright: (c) 2023 by Sixline
+    :copyright: (c) 2019-2021 by Mahmoud Elshahat.
+    :license: GNU GPLv3, see LICENSE.md for more details.
+"""
+
 # this module includes base64 data for all icons
 
 # APP_ICON 48x48 pixel VDM logo
 APP_ICON = b'iVBORw0KGgoAAAANSUhEUgAAADAAAAAwCAYAAABXAvmHAAAACXBIWXMAAAHRAAAB0QEMkUzzAAAA\nGXRFWHRTb2Z0d2FyZQB3d3cuaW5rc2NhcGUub3Jnm+48GgAAAAx0RVh0QXV0aG9yAGVybmVzPTIL\nhQAAAGp0RVh0RGVzY3JpcHRpb24AYXJ0aXN0aWMsIGFydGlzdGljLCBjbGlwIGFydCwgY2xpcGFy\ndCwgZmxvd2VyLCBmbG93ZXIsIGltYWdlLCBtZWRpYSwgcG5nLCBwdWJsaWMgZG9tYWluLCBzdmcs\nIKhTTBoAAAAhdEVYdENyZWF0aW9uIFRpbWUAMjAwNy0wNC0zMFQwMzo1Mjo1NDY2JWUAAAA6dEVY\ndFNvdXJjZQBodHRwOi8vb3BlbmNsaXBhcnQub3JnL2RldGFpbC80MjIxL3NwaXJhbGUtYnktZXJu\nZXM7OisKAAAAWHRFWHRDb3B5cmlnaHQAQ0MwIFB1YmxpYyBEb21haW4gRGVkaWNhdGlvbiBodHRw\nOi8vY3JlYXRpdmVjb21tb25zLm9yZy9wdWJsaWNkb21haW4vemVyby8xLjAvxuO9+QAAEFVJREFU\naIG9Wml0VVWW/vY59943ZyQJJGFICIOMggEEtUSkZFBslEJL0CrBstV2oKtkuSznVV3l2Nrl1FgO\nBWUpWrQDSDkjhSBqMQQSUBnEMAYIIWR4053O7h/3PYyPF4029l7rrrtW3j77fN/Z59w9nBAz4/9D\nLupHfasKAsW7Wpz46zvsncwcPxl26ccmsOC84MzRPbSbq/JodEADCQKaEmw2J1AXtd0Nmw7ximtX\nJJYxs/tD7H9vAtdUh3pM68MzX9qR+OuLdXysM72rh1P59KrgY6cWy+lSMAkiCAIEACm8RxcETQB7\n27h+d4v70iv19PiT66KHfhQCRCRfnx66ZVy5mB+10HbdsvYh7x7iWDbdB38SOHdcT/HnkqDoxQAI\ngCCACJBEkOQR0IhhSIIuCIYEjiZU05oG9/6ZSxOPcBeBaV1RumM09az5RXjR0CKaYLqEt7407+wM\n/P1nB2aPKxdPBSSFW01Okf+ahCSGJECTBF0AmsswBMNWgCDqdna59uCfpwTjABZ0Bdt3euC/J4ZG\nnV8lXygJUv+ky/jsqNp45oux0cysMnXvGhu85IxyWuiTCKagg8EQRAAzpPC2UXOSG2MOr25LuhsP\n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\n'
 
 # 32x30 pixels black
 home_icon = b'iVBORw0KGgoAAAANSUhEUgAAACAAAAAeCAYAAABNChwpAAAACXBIWXMAAAd0AAAHdAHxbc2KAAAA\nGXRFWHRTb2Z0d2FyZQB3d3cuaW5rc2NhcGUub3Jnm+48GgAAAfpJREFUSInVlj1LW1EYx383L6aD\nFPwCXQKi30KwBedOxaUUh0opCkYUt3boKmpoqJLWNGIbLSUR3yYlcwf7CTpUEIeAk+JgXjrcc+Dw\n5Nzk5PbG0gf+Q56X8/uf3JdzIVw8BqrAtVIVmAi5Vs/xGqgDLaEmkBG9Y8ApUAAeRgGft4Clloz+\nX0b+TT/gP5Rk/q2auTVyK1HDD4CU0qGlvix+r0YJ31dgHSmV63Rp1sLA5ywLHQEPLL0DQLmDgWyv\n8IxlkYoCAXjAO/zr7Rkm9gIMvO8FPmNZoGzA48Bno7YuTNj+iS+u8Cn8Z9oc/g4kA+BaH4GY6kmq\nGdmz2A3+AmiIoW8OcJuJOLBt6VkIgj+3wHeAhCNc65NhIgHsinoTeCXhk7S/Xr8a8JgjXGtTmCiJ\nekNtGICnwJ1oKBlwD/8mc4XbTMSBoqjXgWcANVEoqgG983wIuFZemNgS9RrATyNRMOAesPEXcNsj\nKu+jM4A08AH/2dduPSAXAVwrZ5iIAbP4Z0OagMhGCNdyPgum+wDXeilhMZkARl2dhogRFwOeJRdV\ntK2dcGkS0QJOAmrjXebbNhzGQBN4ElBrOMx3dnTfYTPQ6iOv8V8YaP5rA5d9NPDbpWkIuCD4bVbv\nMCs/aEydA4OuToeBY+BKyfxY6cXADf6RWwEe2Qb+AP3yZGXPWUKPAAAAAElFTkSuQmCC\n'
```

### Comparing `vortexdm-2022.1.0/vdm/model.py` & `vortexdm-2023.1.0/vortexdm/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
-    Vortex Download Manager (VDM)
+    Vortex Download Manager (VortexDM)
 
-    Multi-connection internet download manager, based on "LibCurl", and "youtube_dl". Original project, FireDM, by Mahmoud Elshahat.
-    :copyright: (c) 2022 by Sixline
+    A multi-connection internet download manager, based on "PycURL" and "youtube_dl". Original project, FireDM, by Mahmoud Elshahat.
+    :copyright: (c) 2023 by Sixline
     :copyright: (c) 2019-2021 by Mahmoud Elshahat.
     :license: GNU GPLv3, see LICENSE.md for more details.
 
     Module description:
         this module contains an observables data models
 """
 import os
```

### Comparing `vortexdm-2022.1.0/vdm/setting.py` & `vortexdm-2023.1.0/vortexdm/setting.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
-    Vortex Download Manager (VDM)
+    Vortex Download Manager (VortexDM)
 
-    Multi-connection internet download manager, based on "LibCurl", and "youtube_dl". Original project, FireDM, by Mahmoud Elshahat.
-    :copyright: (c) 2022 by Sixline
+    A multi-connection internet download manager, based on "PycURL" and "youtube_dl". Original project, FireDM, by Mahmoud Elshahat.
+    :copyright: (c) 2023 by Sixline
     :copyright: (c) 2019-2021 by Mahmoud Elshahat.
     :license: GNU GPLv3, see LICENSE.md for more details.
 """
 
 import os
 import json
 import shutil
```

### Comparing `vortexdm-2022.1.0/vdm/systray.py` & `vortexdm-2023.1.0/vortexdm/systray.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
-    Vortex Download Manager (VDM)
+    Vortex Download Manager (VortexDM)
 
-    Multi-connection internet download manager, based on "LibCurl", and "youtube_dl". Original project, FireDM, by Mahmoud Elshahat.
-    :copyright: (c) 2022 by Sixline
+    A multi-connection internet download manager, based on "PycURL" and "youtube_dl". Original project, FireDM, by Mahmoud Elshahat.
+    :copyright: (c) 2023 by Sixline
     :copyright: (c) 2019-2021 by Mahmoud Elshahat.
     :license: GNU GPLv3, see LICENSE.md for more details.
 
     Module description:
         system tray icon based on GTK and pystray, tested on windows and Manjaro using GTK 3.0
 """
 
@@ -63,15 +63,15 @@
         if config.operating_system == 'Linux':
             try:
                 import gi
                 gi.require_version('Gtk', '3.0')
                 from gi.repository import Gtk
                 self.Gtk = Gtk
 
-                # delete previous icon file (it might contains an icon file for old VDM versions)
+                # delete previous icon file (it might contains an icon file for old VortexDM versions)
                 delete_file(self.tray_icon_path)
 
                 # save file to settings folder
                 self.tray_icon.save(self.tray_icon_path, format='png')
 
                 # creating menu
                 menu = Gtk.Menu()
```

### Comparing `vortexdm-2022.1.0/vdm/themes.py` & `vortexdm-2023.1.0/vortexdm/themes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+"""
+    Vortex Download Manager (VortexDM)
+
+    A multi-connection internet download manager, based on "PycURL" and "youtube_dl". Original project, FireDM, by Mahmoud Elshahat.
+    :copyright: (c) 2023 by Sixline
+    :copyright: (c) 2019-2021 by Mahmoud Elshahat.
+    :license: GNU GPLv3, see LICENSE.md for more details.
+"""
+
 import awesometkinter as atk
 
 # main colors
 MAIN_BG = "#1c1c21"
 MAIN_FG = "white"
 
 # side frame colors
```

### Comparing `vortexdm-2022.1.0/vdm/tkview.py` & `vortexdm-2023.1.0/vortexdm/tkview.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
-    Vortex Download Manager (VDM)
+    Vortex Download Manager (VortexDM)
 
-    Multi-connection internet download manager, based on "LibCurl", and "youtube_dl". Original project, FireDM, by Mahmoud Elshahat.
-    :copyright: (c) 2022 by Sixline
+    A multi-connection internet download manager, based on "PycURL" and "youtube_dl". Original project, FireDM, by Mahmoud Elshahat.
+    :copyright: (c) 2023 by Sixline
     :copyright: (c) 2019-2021 by Mahmoud Elshahat.
     :license: GNU GPLv3, see LICENSE.md for more details.
 
     Module description:
         Main application gui design by tkinter
 """
 import datetime
@@ -27,16 +27,16 @@
 import signal
 
 if __package__ is None:
     path = os.path.realpath(os.path.abspath(__file__))
     sys.path.insert(0, os.path.dirname(path))
     sys.path.insert(0, os.path.dirname(os.path.dirname(path)))
 
-    __package__ = 'vdm'
-    import vdm
+    __package__ = 'vortexdm'
+    import vortexdm
 
 from .view import IView
 from .controller import Controller, set_option, get_option, log_runtime_info
 from .utils import *
 from . import config
 from .config import BULK, COMPACT, MIX
 from . import iconsbase64
@@ -1061,15 +1061,15 @@
         kdialog: command line tool for kde file chooser
         gtk: use Gtk.FileChooserDialog directly thru python, "will not use", since sometimes it will raise
              error: Gdk-Message: Fatal IO error 0 (Success) on X server :1, and application will crash
     """
     def __init__(self, foldersonly=False):
         self.use = 'TK'  #, 'zenity', or 'kdialog'
         self.foldersonly = foldersonly
-        self.title = 'VDM - ' 
+        self.title = 'VortexDM - ' 
         self.title += 'Select a folder' if self.foldersonly else 'Select a file'
         if config.operating_system == 'Linux':
             # looking for zenity
             error, zenity_path = run_command('which zenity', verbose=False)
             if os.path.isfile(zenity_path):
                 self.use = 'zenity'
             else:
@@ -3160,15 +3160,15 @@
             if config.operating_system in ('Windows', 'Darwin'):
                 self.root.wm_state('zoomed')
             else:
                 self.root.attributes('-zoomed', True)
 
         # prevent window resize to zero
         self.root.minsize(750, 455)
-        self.root.title(f'VDM ver.{config.APP_VERSION}')
+        self.root.title(f'VortexDM - {config.APP_VERSION}')
         self.main_frame = None
 
         # set window icon
         global app_icon_img, popup_icon_img
         app_icon_img = atk.create_image(b64=APP_ICON, size=48)
         popup_icon_img = atk.create_image(b64=APP_ICON, size=22)
 
@@ -3178,15 +3178,15 @@
         self.load_user_themes()
 
         # select tkinter theme required for things to be right on windows,
         # only 'alt', 'default', and 'classic' works fine on windows 10
         s = ttk.Style()
         s.theme_use('default')
 
-        # apply VDM theme
+        # apply VortexDM theme
         self.apply_theme(config.current_theme)
 
         self.create_main_widgets()
 
         # bind window close
         self.root.protocol("WM_DELETE_WINDOW", self.close)
 
@@ -3210,19 +3210,19 @@
 
         # number vs callback, e.g. ask controller to update youtube-dl sending any identifier e.g. "500",
         # when controller finishes this job it will send a signal with same number "500", then tkview will call
         # the associated callback
         self.post_processors = {}
 
     def ibus_workaround(self):
-        # because of ibus bug, VDM take longer time to load with every run as time goes on, same as 
+        # because of ibus bug, VortexDM take longer time to load with every run as time goes on, same as 
         # any tkinter application.
-        # workaround is to kill ibus-x11 then restart ibus again after VDM finish loading
+        # workaround is to kill ibus-x11 then restart ibus again after VortexDM finish loading
         # reported bug at https://github.com/ibus/ibus/issues/2324
-        # however this workaround makes VDM loads faster, ibus will still affect gui performance when 
+        # however this workaround makes VortexDM loads faster, ibus will still affect gui performance when 
         # it gets restarted again.
         # hope they fix this bug as soon as possible
         p = subprocess.Popen(['ps', '-A'], stdout=subprocess.PIPE, universal_newlines=True)
         output, error = p.communicate()
         if error: return
 
         for line in output.splitlines():
@@ -3938,15 +3938,15 @@
         CheckOption(tab, 'Write thumbnail image to disk', key='download_thumbnail').pack(anchor='w')
 
         tk.Label(tab, text='Select action to run after "ALL" download items are completed:', bg=bg,
                  fg=fg).pack(anchor='w', padx=5)
 
         CheckEntryOption(tab, ' Run command:  ', entry_key='on_completion_command').pack(anchor='w', fill='x',
                                                                                          expand=True, padx=(0, 5))
-        CheckOption(tab, ' Exit VDM', key='on_completion_exit').pack(anchor='w', fill='x', expand=True, padx=(0, 5))
+        CheckOption(tab, ' Exit VortexDM', key='on_completion_exit').pack(anchor='w', fill='x', expand=True, padx=(0, 5))
         CheckOption(tab, ' Shutdown computer', key='shutdown_pc').pack(anchor='w', fill='x', expand=True, padx=(0, 5))
 
         separator()
 
         # ------------------------------------------------------------------------------------Downloader options--------
         heading('Downloader options:')
         LabeledEntryOption(tab, 'Concurrent downloads (1 ~ 100): ', entry_key='max_concurrent_downloads',
@@ -4044,30 +4044,30 @@
 
         CheckEntryOption(update_frame, 'Check for update every: ', entry_key='update_frequency', width=4,
                          justify='center',
                          check_key='check_for_update', get_text_validator=lambda x: int(x) if int(x) > 0 else 7) \
             .grid(row=0, column=1, sticky='w')
         tk.Label(update_frame, bg=bg, fg=fg, text='days', padx=5).grid(row=0, column=2, sticky='w')
 
-        # VDM update
-        self.vdm_update_note = tk.StringVar()
-        self.vdm_update_note.set(f'VDM version: {config.APP_VERSION}')
-        lbl(self.vdm_update_note).grid(row=1, column=1, sticky='w', pady=20, padx=20)
+        # VortexDM update
+        self.vortexdm_update_note = tk.StringVar()
+        self.vortexdm_update_note.set(f'VortexDM Version: {config.APP_VERSION}')
+        lbl(self.vortexdm_update_note).grid(row=1, column=1, sticky='w', pady=20, padx=20)
 
         # youtube-dl and yt_dlp
         self.youtube_dl_update_note = tk.StringVar()
-        self.youtube_dl_update_note.set(f'youtube-dl version: {config.youtube_dl_version}')
+        self.youtube_dl_update_note.set(f'youtube-dl Version: {config.youtube_dl_version}')
         lbl(self.youtube_dl_update_note).grid(row=2, column=1, sticky='w', pady=(0, 20), padx=20)
 
         self.yt_dlp_update_note = tk.StringVar()
-        self.yt_dlp_update_note.set(f'yt_dlp version: {config.yt_dlp_version}')
+        self.yt_dlp_update_note.set(f'yt_dlp Version: {config.yt_dlp_version}')
         lbl(self.yt_dlp_update_note).grid(row=3, column=1, sticky='w', pady=(0, 20), padx=20)
 
         if config.FROZEN or config.isappimage:
-            for i, pkg in enumerate(('vdm', 'youtube_dl', 'yt_dlp')):
+            for i, pkg in enumerate(('vortexdm', 'youtube_dl', 'yt_dlp')):
                 Button(update_frame, text='Rollback', command=lambda x=pkg: self.rollback_pkg_update(x),
                        tooltip=f'Restore Previous {pkg} Version',
                        image=imgs['undo_icon']).grid(row=i + 1, column=3, sticky='w', pady=5)
 
         Button(update_frame, text='Check for updates', compound='left',
                command=self.check_for_update).grid(row=3, column=4, padx=20)
 
@@ -4792,16 +4792,16 @@
                 else:
                     self.response_q.put(data)
                 time.sleep(0.01)
 
     def update_youtube_dl_info(self):
         """write youtube-dl and yt_dlp version once it gets imported"""
 
-        self.youtube_dl_update_note.set(f'youtube-dl version: {config.youtube_dl_version or "Loading ... "}')
-        self.yt_dlp_update_note.set(f'yt_dlp version: {config.yt_dlp_version or "Loading ... "}')
+        self.youtube_dl_update_note.set(f'youtube-dl Version: {config.youtube_dl_version or "Loading ... "}')
+        self.yt_dlp_update_note.set(f'yt_dlp Version: {config.yt_dlp_version or "Loading ... "}')
 
         if not all((config.youtube_dl_version, config.yt_dlp_version)):
             self.root.after(1000, self.update_youtube_dl_info)
 
     def rollback_pkg_update(self, pkg):
         """restore previous package version e.g. youtube-dl and yt_dlp"""
         response = self.popup(f'Delete last {pkg} update and restore previous version?', buttons=['Ok', 'Cancel'])
@@ -4826,18 +4826,18 @@
         config.log_callbacks.append(self.log_callback)
         config.log_popup_callback = self.log_popup
 
         # log runtime info
         log_runtime_info()
 
         # log extra pkgs info
-        log('Tkinter version:', self.root.call("info", "patchlevel"))
-        log('AwesomeTkinter version:', atk_version)
-        log('Pillow version:', PIL.__version__)
-        log('PyCUrl version:', pycurl.version)
+        log('Tkinter Version:', self.root.call("info", "patchlevel"))
+        log('AwesomeTkinter Version:', atk_version)
+        log('Pillow Version:', PIL.__version__)
+        log('PycURL Version:', pycurl.version)
         log()
 
         # get download items
         self.controller.get_d_list()
 
         # start url monitor thread
         run_thread(url_watchdog, self.root, daemon=True)
@@ -4891,19 +4891,19 @@
             dp = DatePicker(self.root, title='Schedule Download Item')
             if dp.selected_date:
                 for item in selected_items:
                     self.controller.schedule_start(uid=item.uid, target_date=dp.selected_date)
 
     @ignore_calls_when_busy
     def show_about_notes(self):
-        res = self.popup(about_notes, buttons=['Home', 'Help!', 'Close'], title='About VDM')
+        res = self.popup(about_notes, buttons=['Home', 'Help!', 'Close'], title='About VortexDM')
         if res == 'Help!':
-            open_webpage('https://github.com/Sixline/VDM/blob/master/docs/user_guide.md')
+            open_webpage('https://github.com/Sixline/VortexDM/blob/master/docs/user_guide.md')
         elif res == 'Home':
-            open_webpage('https://github.com/Sixline/VDM')
+            open_webpage('https://github.com/Sixline/VortexDM')
 
         free_callback(self.show_about_notes)
 
     @ignore_calls_when_busy
     def check_for_update(self):
         log('\n\nstart Checking for update ....')
         self.select_tab('Log')
```

### Comparing `vortexdm-2022.1.0/vdm/update.py` & `vortexdm-2023.1.0/vortexdm/update.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
-    Vortex Download Manager (VDM)
+    Vortex Download Manager (VortexDM)
 
-    Multi-connection internet download manager, based on "LibCurl", and "youtube_dl". Original project, FireDM, by Mahmoud Elshahat.
-    :copyright: (c) 2022 by Sixline
+    A multi-connection internet download manager, based on "PycURL" and "youtube_dl". Original project, FireDM, by Mahmoud Elshahat.
+    :copyright: (c) 2023 by Sixline
     :copyright: (c) 2019-2021 by Mahmoud Elshahat.
     :license: GNU GPLv3, see LICENSE.md for more details.
 """
 
 # todo: change docstring to google format and clean unused code
 # check and update application
 
@@ -33,43 +33,43 @@
     """open browser window with latest release url on github for frozen application or source code url"""
     url = config.LATEST_RELEASE_URL if config.FROZEN else config.APP_URL
     webbrowser.open_new(url)
 
 
 def check_for_new_version():
     """
-    Check for new VDM version
+    Check for new VortexDM version
 
     Return:
         changelog text or None
 
     """
 
     latest_version = '0'
     changelog = None
 
     try:
         if config.FROZEN:
             # use github API to get latest version
-            url = 'https://api.github.com/repos/Sixline/VDM/releases/latest'
+            url = 'https://api.github.com/repos/Sixline/VortexDM/releases/latest'
             contents = download(url, verbose=False)
 
             if contents:
                 j = json.loads(contents)
                 latest_version = j.get('tag_name', '0')
 
         else:
             # check pypi version
             latest_version, _ = get_pkg_latest_version('vortexdm')
 
         if parse_version(latest_version) > parse_version(config.APP_VERSION):
             log('Found new version:', str(latest_version))
 
             # download change log file
-            url = 'https://github.com/Sixline/VDM/raw/master/ChangeLog.txt'
+            url = 'https://github.com/Sixline/VortexDM/raw/master/ChangeLog.txt'
             changelog = download(url, verbose=False)
     except Exception as e:
         log('check_for_new_version()> error:', e)
 
     return changelog
 
 
@@ -85,15 +85,15 @@
                     <link>https://pypi.org/project/youtube-dl/2020.12.14/</link>
                     <description>YouTube video downloader</description>
                     <author>dstftw@gmail.com</author>
                     <pubDate>Sun, 13 Dec 2020 17:59:21 GMT</pubDate>
                     </item>
 
     2- json, (slower and bigger file), send all info for the package
-        url pattern: f'https://pypi.org/pypi/{pkg}/json' e.g.    https://pypi.org/pypi/vdm/json
+        url pattern: f'https://pypi.org/pypi/{pkg}/json' e.g.    https://pypi.org/pypi/vortexdm/json
         received json will be a dict with:
         keys = 'info', 'last_serial', 'releases', 'urls'
         releases = {'release_version': [{dict for wheel file}, {dict for tar file}], ...}
         dict for wheel file = {"filename":"yt_dlp-2020.10.24.post6-py2.py3-none-any.whl", 'url': 'file url'}
         dict for tar file = {"filename":"yt_dlp-2020.10.24.post6.tar.gz", 'url': 'file url'}
 
 
@@ -105,15 +105,15 @@
         2-tuple(str, str): latest_version, and download url (for wheel file) if available
     """
 
     # download json info
     url = f'https://pypi.org/pypi/{pkg}/json' if fetch_url else f'https://pypi.org/rss/project/{pkg}/releases.xml'
 
     # get BytesIO object
-    log(f'check for {pkg} latest version on pypi.org...')
+    log(f'Checking for the latest version of {pkg} on pypi.org...')
     contents = download(url, verbose=False)
     latest_version = None
     url = None
 
     if contents:
         # rss feed
         if not fetch_url:
```

### Comparing `vortexdm-2022.1.0/vdm/utils.py` & `vortexdm-2023.1.0/vortexdm/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
-    Vortex Download Manager (VDM)
+    Vortex Download Manager (VortexDM)
 
-    Multi-connection internet download manager, based on "LibCurl", and "youtube_dl". Original project, FireDM, by Mahmoud Elshahat.
-    :copyright: (c) 2022 by Sixline
+    A multi-connection internet download manager, based on "PycURL" and "youtube_dl". Original project, FireDM, by Mahmoud Elshahat.
+    :copyright: (c) 2023 by Sixline
     :copyright: (c) 2019-2021 by Mahmoud Elshahat.
     :license: GNU GPLv3, see LICENSE.md for more details.
 """
 import datetime
 import os
 import io
 import hashlib
@@ -28,15 +28,15 @@
 
 # 3rd party
 try:
     import pycurl
 except:
     print('pycurl not found')
 
-__package__ = 'vdm'
+__package__ = 'vortexdm'
 
 from . import config
 
 
 def threaded(func):
     """a decorator to run any function / method in a thread
     you can pass threaded=False option when calling the decorated function if you need to disable threadding"""
@@ -878,15 +878,15 @@
 def is_pkg_exist(pkg_name):
     """
     return True if pkg exist in sys.path and can be imported
 
     Args:
         pkg_name(str): package name, spaces will be stripped
 
-    >>> is_pkg_exist('   vdm  ')
+    >>> is_pkg_exist('   vortexdm  ')
     True
     >>> is_pkg_exist('blahx123456789x')
     False
     """
     pkg_name = pkg_name.strip()
     if importlib.util.find_spec(pkg_name) is not None:
         return True
@@ -1212,15 +1212,15 @@
                 text = f.read()
                 match = re.search(rb'\d+\.\d+\.\d+', text)
                 version = match.group().decode('utf-8')
         except:
             pass
 
     if not version:
-        # parse .dist-info folder e.g: youtube_dl-2021.5.16.dist-info or VDM-2021.2.9.dist-info
+        # parse .dist-info folder e.g: youtube_dl-2021.5.16.dist-info or VortexDM-2021.2.9.dist-info
         try:
             parent_folder = os.path.dirname(pkg_path)
             pkg_name = os.path.basename(pkg_path)
 
             for folder_name in os.listdir(parent_folder):
                 match = re.match(pkg_name + r'-(.*?)\.dist-info', folder_name, re.IGNORECASE)
                 if match:
@@ -1278,15 +1278,15 @@
 def check_write_permission(target_folder, create_dirs=True):
     """check target folder for write permission"""
 
     try:
         if create_dirs:
             os.makedirs(target_folder, exist_ok=True)
 
-        fn = 'vdm-testfile'
+        fn = 'vortexdm-testfile'
         existing_names = os.listdir(target_folder)
         if fn in existing_names:
             fn = auto_rename(fn, existing_names)
 
         fp = os.path.join(target_folder, fn)
 
         with open(fp, 'w') as f:
```

### Comparing `vortexdm-2022.1.0/vdm/video.py` & `vortexdm-2023.1.0/vortexdm/video.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
-    Vortex Download Manager (VDM)
+    Vortex Download Manager (VortexDM)
 
-    Multi-connection internet download manager, based on "LibCurl", and "youtube_dl". Original project, FireDM, by Mahmoud Elshahat.
-    :copyright: (c) 2022 by Sixline
+    A multi-connection internet download manager, based on "PycURL" and "youtube_dl". Original project, FireDM, by Mahmoud Elshahat.
+    :copyright: (c) 2023 by Sixline
     :copyright: (c) 2019-2021 by Mahmoud Elshahat.
     :license: GNU GPLv3, see LICENSE.md for more details.
 """
 import copy
 import os
 import re
 import time
@@ -80,15 +80,15 @@
     # subtitle
     # ydl_opts['listsubtitles'] = True  # this is has a problem with playlist
     # ydl_opts['allsubtitles'] = True  # has no effect
     ydl_opts['writesubtitles'] = True
     ydl_opts['writeautomaticsub'] = True
 
     # if config.log_level >= 3:
-        # ydl_opts['verbose'] = True  # it make problem with Frozen VDM, extractor doesn't work
+        # ydl_opts['verbose'] = True  # it make problem with Frozen VortexDM, extractor doesn't work
     # elif config.log_level <= 1:
     #     ydl_opts['quiet'] = True  # it doesn't work
 
     return ydl_opts
 
 
 class Video(DownloadItem):
@@ -550,15 +550,14 @@
         self.fragment_base_url = stream_info.get('fragment_base_url', None)
         self.fragments = stream_info.get('fragments', None)
 
         # protocol
         self.protocol = stream_info.get('protocol', '')
 
         # calculate some values
-        self.rawbitrate = stream_info.get('abr', 0) * 1024
         self._mediatype = None
         self.resolution = f'{self.width}x{self.height}' if (self.width and self.height) else ''
 
         # ignore fragmented streams, and hls (m3u8), the size coming from headers is not correct
         if self.fragments or 'm3u8' in self.protocol:
             self.size = 0
 
@@ -725,15 +724,15 @@
         else:
             import youtube_dl
 
         config.youtube_dl_version = youtube_dl.version.__version__
 
         # calculate loading time
         load_time = time.time() - start
-        log(f'youtube_dl version: {config.youtube_dl_version}, load_time= {int(load_time)} seconds', log_level=2)
+        log(f'youtube_dl Version: {config.youtube_dl_version}, load_time= {int(load_time)} seconds', log_level=2)
 
         # get a random user agent and update headers
         if not config.custom_user_agent:
             config.http_headers['User-Agent'] = youtube_dl.utils.random_user_agent()
 
         # set default extractor
         if config.active_video_extractor == 'youtube_dl':
@@ -752,15 +751,15 @@
         else:
             import yt_dlp
 
         config.yt_dlp_version = yt_dlp.version.__version__
 
         # calculate loading time
         load_time = time.time() - start
-        log(f'yt_dlp version: {config.yt_dlp_version}, load_time= {int(load_time)} seconds', log_level=2)
+        log(f'yt_dlp Version: {config.yt_dlp_version}, load_time= {int(load_time)} seconds', log_level=2)
 
         # set default extractor
         if config.active_video_extractor == 'yt_dlp':
             set_default_extractor('yt_dlp')
 
         load_user_extractors(engine=yt_dlp)
```

### Comparing `vortexdm-2022.1.0/vdm/view.py` & `vortexdm-2023.1.0/vortexdm/view.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 """
-    Vortex Download Manager (VDM)
+    Vortex Download Manager (VortexDM)
 
-    Multi-connection internet download manager, based on "LibCurl", and "youtube_dl". Original project, FireDM, by Mahmoud Elshahat.
-    :copyright: (c) 2022 by Sixline
+    A multi-connection internet download manager, based on "PycURL" and "youtube_dl". Original project, FireDM, by Mahmoud Elshahat.
+    :copyright: (c) 2023 by Sixline
     :copyright: (c) 2019-2021 by Mahmoud Elshahat.
     :license: GNU GPLv3, see LICENSE.md for more details.
 
     Module description:
         An interface for All views / GUIs
 """
 
-
 from abc import ABC, abstractmethod
 
-
 class IView(ABC):
     @abstractmethod
     def run(self):
         """run view mainloop if any"""
         pass
 
     @abstractmethod
```

### Comparing `vortexdm-2022.1.0/vdm/worker.py` & `vortexdm-2023.1.0/vortexdm/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
-    Vortex Download Manager (VDM)
+    Vortex Download Manager (VortexDM)
 
-    Multi-connection internet download manager, based on "LibCurl", and "youtube_dl". Original project, FireDM, by Mahmoud Elshahat.
-    :copyright: (c) 2022 by Sixline
+    A multi-connection internet download manager, based on "PycURL" and "youtube_dl". Original project, FireDM, by Mahmoud Elshahat.
+    :copyright: (c) 2023 by Sixline
     :copyright: (c) 2019-2021 by Mahmoud Elshahat.
     :license: GNU GPLv3, see LICENSE.md for more details.
 """
 
 # worker class
 
 # todo: change docstring to google format and clean unused code
```

