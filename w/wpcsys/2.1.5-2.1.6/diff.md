# Comparing `tmp/wpcsys-2.1.5.tar.gz` & `tmp/wpcsys-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wpcsys-2.1.5.tar", last modified: Mon Jul 17 04:03:42 2023, max compression
+gzip compressed data, was "wpcsys-2.1.6.tar", last modified: Tue Jul 18 05:46:27 2023, max compression
```

## Comparing `wpcsys-2.1.5.tar` & `wpcsys-2.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 04:03:42.133986 wpcsys-2.1.5/
--rw-rw-rw-   0        0        0     1091 2022-10-03 09:42:47.000000 wpcsys-2.1.5/LICENSE
--rw-rw-rw-   0        0        0       64 2022-11-04 05:05:00.000000 wpcsys-2.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0    10221 2023-07-17 04:03:42.125985 wpcsys-2.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     9160 2023-07-14 09:03:31.000000 wpcsys-2.1.5/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-17 04:03:42.133986 wpcsys-2.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1985 2022-11-23 08:57:09.000000 wpcsys-2.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 04:03:42.069066 wpcsys-2.1.5/wpcsys/
--rw-rw-rw-   0        0        0        0 2022-10-06 03:03:31.000000 wpcsys-2.1.5/wpcsys/__init__.py
--rw-rw-rw-   0        0        0  1292959 2023-02-08 04:26:34.000000 wpcsys-2.1.5/wpcsys/libusb-1.0.dll
--rw-rw-rw-   0        0        0  7552000 2023-07-17 03:59:27.000000 wpcsys-2.1.5/wpcsys/pywpc.cp310-win_amd64.pyd
--rw-rw-rw-   0        0        0  8136704 2023-07-17 04:03:09.000000 wpcsys-2.1.5/wpcsys/pywpc.cp38-win_amd64.pyd
--rw-rw-rw-   0        0        0  8145920 2023-07-17 04:02:02.000000 wpcsys-2.1.5/wpcsys/pywpc.cp39-win_amd64.pyd
-drwxrwxrwx   0        0        0        0 2023-07-17 04:03:42.122985 wpcsys-2.1.5/wpcsys.egg-info/
--rw-rw-rw-   0        0        0    10221 2023-07-17 04:03:41.000000 wpcsys-2.1.5/wpcsys.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2023-07-17 04:03:41.000000 wpcsys-2.1.5/wpcsys.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 04:03:41.000000 wpcsys-2.1.5/wpcsys.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      152 2023-07-17 04:03:41.000000 wpcsys-2.1.5/wpcsys.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-17 04:03:41.000000 wpcsys-2.1.5/wpcsys.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 05:46:27.656314 wpcsys-2.1.6/
+-rw-rw-rw-   0        0        0     1091 2022-10-03 09:42:47.000000 wpcsys-2.1.6/LICENSE
+-rw-rw-rw-   0        0        0       64 2022-11-04 05:05:00.000000 wpcsys-2.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0    10446 2023-07-18 05:46:27.647318 wpcsys-2.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     9385 2023-07-17 09:03:28.000000 wpcsys-2.1.6/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-18 05:46:27.656314 wpcsys-2.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1985 2022-11-23 08:57:09.000000 wpcsys-2.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 05:46:27.592525 wpcsys-2.1.6/wpcsys/
+-rw-rw-rw-   0        0        0        0 2022-10-06 03:03:31.000000 wpcsys-2.1.6/wpcsys/__init__.py
+-rw-rw-rw-   0        0        0  1292959 2023-02-08 04:26:34.000000 wpcsys-2.1.6/wpcsys/libusb-1.0.dll
+-rw-rw-rw-   0        0        0  7585280 2023-07-18 05:42:14.000000 wpcsys-2.1.6/wpcsys/pywpc.cp310-win_amd64.pyd
+-rw-rw-rw-   0        0        0  8171520 2023-07-18 05:43:53.000000 wpcsys-2.1.6/wpcsys/pywpc.cp38-win_amd64.pyd
+-rw-rw-rw-   0        0        0  8180224 2023-07-18 05:43:11.000000 wpcsys-2.1.6/wpcsys/pywpc.cp39-win_amd64.pyd
+drwxrwxrwx   0        0        0        0 2023-07-18 05:46:27.645338 wpcsys-2.1.6/wpcsys.egg-info/
+-rw-rw-rw-   0        0        0    10446 2023-07-18 05:46:27.000000 wpcsys-2.1.6/wpcsys.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2023-07-18 05:46:27.000000 wpcsys-2.1.6/wpcsys.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 05:46:27.000000 wpcsys-2.1.6/wpcsys.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      152 2023-07-18 05:46:27.000000 wpcsys-2.1.6/wpcsys.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-18 05:46:27.000000 wpcsys-2.1.6/wpcsys.egg-info/top_level.txt
```

### Comparing `wpcsys-2.1.5/LICENSE` & `wpcsys-2.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wpcsys-2.1.5/PKG-INFO` & `wpcsys-2.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wpcsys
-Version: 2.1.5
+Version: 2.1.6
 Summary: WPC Python driver APIs, the easiest way to Control & Data Acquisition (DAQ)
 Home-page: https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release
 Author: chunglee_people, Chieh-An Lin
 Author-email: wu@wpc.com.tw
 License: MIT
 Keywords: wpc,daq,driver,usb,ethernet,wifi,data acquisition
 Classifier: Development Status :: 5 - Production/Stable
@@ -34,15 +34,15 @@
 
 Asynchronous mode means that processes run independently of each other and don't wait for the completion of the previous process. Instead, each process runs on its own, without blocking the execution of other processes.
 
 In general, synchronous mode is easier to understand and debug, while asynchronous mode is more scalable and allows for greater concurrency.
 
 Some API functions in the `pywpc` package may not compatible with earlier versions of WPC DAQ firmware.
 To update device firmware to the latest version, please use WPC Device Manager and `LabVIEW Run-time engine <https://drive.google.com/file/d/1Uj6r65KhNxvuApiqrMkZp-NWyq-Eek-k/view>`_.
-You can download WPC Device Manager by `latest release <https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release/releases/tag/v2.1.5>`_ or visit `WPC Systems Ltd. official website <http://www.wpc.com.tw/>`_.
+You can download WPC Device Manager by `latest release <https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release/releases/tag/v2.1.6>`_ or visit `WPC Systems Ltd. official website <http://www.wpc.com.tw/>`_.
 
 +-------------------+-----------------------------------------------------------------------------------+
 |                   | Link                                                                              |
 +===================+===================================================================================+
 | WPC official site | http://www.wpc.com.tw/                                                            |
 +-------------------+-----------------------------------------------------------------------------------+
 | GitHub            | https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release                      |
@@ -88,15 +88,15 @@
 -----------
 **Easy, fast, and just works!**
 
    >>> from wpcsys import pywpc
    >>> pywpc.PKG_NAME
    pywpc
    >>> pywpc.HANDLE_LIST
-   ['DeviceFinder', 'WifiDAQE3A', 'WifiDAQF4A', 'STEM', 'EMotion', 'EDrive_ST', 'EthanA', 'EthanD', 'EthanL', 'EthanO', 'USBDAQF1D', 'USBDAQF1DSNK', 'USBDAQF1AD', 'USBDAQF1AOD', 'USBDAQF1TD', 'USBDAQF1RD', 'USBDAQF1CD']
+   ['DeviceFinder', 'WifiDAQE3A', 'WifiDAQF4A', 'STEM', 'EMotion', 'EDrive_ST', 'EthanA', 'EthanD', 'EthanI', 'EthanL', 'EthanO', 'EthanT', 'USBDAQF1D', 'USBDAQF1DSNK', 'USBDAQF1AD', 'USBDAQF1AOD', 'USBDAQF1TD', 'USBDAQF1RD', 'USBDAQF1CD']
 
 Install and Upgrade
 -------------------
 
 - Install
 
 .. code-block:: shell
@@ -130,18 +130,22 @@
 
 Ethernet based DAQ card
 
 - Ethan-A
 
 - Ethan-D
 
+- Ethan-I
+
 - Ethan-L
 
 - Ethan-O
 
+- Ethan-T
+
 USB interface DAQ card
 
 - USB-DAQ-F1-D (Digital)
 
 - USB-DAQ-F1-DSNK (24V Digital)
 
 - USB-DAQ-F1-AD (Digital + AI)
@@ -182,31 +186,33 @@
 +----------------+------+------+------+------+
 
 In the `STEM` product, the values 1, 2, and 4 are used to represent the slots in the AIO.
 Additionally, the DIO ports 0 to 1 are assigned to slot 1, while ports 2 to 3 are assigned to slot 2.
 
 - Ethan & Wifi series
 
-+----------------+-----+-----+----+----+
-| Product/module |AI   |AO   |DI  |DO  |
-+----------------+-----+-----+----+----+
-| Emotion        |     |     |    |    |
-+----------------+-----+-----+----+----+
-| Ethan-A        |0    |     |    |    |
-+----------------+-----+-----+----+----+
-| Ethan-D        |     |     |1   |0   |
-+----------------+-----+-----+----+----+
-| Ethan-L        |     |     |    |0   |
-+----------------+-----+-----+----+----+
-| Ethan-O        |     | 0   |    |    |
-+----------------+-----+-----+----+----+
-| Wifi-DAQ-E3-A  |0    |     |    |    |
-+----------------+-----+-----+----+----+
-| Wifi-DAQ-F4-A  |0    |     |    |    |
-+----------------+-----+-----+----+----+
++----------------+-----+-----+----+----+----+
+| Product/module |AI   |AO   |DI  |DO  |TC  |
++----------------+-----+-----+----+----+----+
+| Ethan-A        |0    |     |    |    |    |
++----------------+-----+-----+----+----+----+
+| Ethan-D        |     |     |1   |0   |    |
++----------------+-----+-----+----+----+----+
+| Ethan-I        |0    |     |    |    |    |
++----------------+-----+-----+----+----+----+
+| Ethan-L        |     |     |    |0   |    |
++----------------+-----+-----+----+----+----+
+| Ethan-O        |     | 0   |    |    |    |
++----------------+-----+-----+----+----+----+
+| Ethan-T        |     |     |    |    | 1  |
++----------------+-----+-----+----+----+----+
+| Wifi-DAQ-E3-A  |0    |     |    |    |    |
++----------------+-----+-----+----+----+----+
+| Wifi-DAQ-F4-A  |0    |     |    |    |    |
++----------------+-----+-----+----+----+----+
 
 - USB series
 
 +----------------+-----+-----+----+----+----+-----+-----+-----+----+---+
 | Product/module |AI   |AO   |DI  |DO  |CAN |UART |SPI  |I2C  |RTD |TC |
 +----------------+-----+-----+----+----+----+-----+-----+-----+----+---+
 | USB-DAQ-F1-D   |     |     |0~3 |0~3 |    |1, 2 |1, 2 |1, 2 |    |   |
```

### Comparing `wpcsys-2.1.5/README.rst` & `wpcsys-2.1.6/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 Asynchronous mode means that processes run independently of each other and don't wait for the completion of the previous process. Instead, each process runs on its own, without blocking the execution of other processes.
 
 In general, synchronous mode is easier to understand and debug, while asynchronous mode is more scalable and allows for greater concurrency.
 
 Some API functions in the `pywpc` package may not compatible with earlier versions of WPC DAQ firmware.
 To update device firmware to the latest version, please use WPC Device Manager and `LabVIEW Run-time engine <https://drive.google.com/file/d/1Uj6r65KhNxvuApiqrMkZp-NWyq-Eek-k/view>`_.
-You can download WPC Device Manager by `latest release <https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release/releases/tag/v2.1.5>`_ or visit `WPC Systems Ltd. official website <http://www.wpc.com.tw/>`_.
+You can download WPC Device Manager by `latest release <https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release/releases/tag/v2.1.6>`_ or visit `WPC Systems Ltd. official website <http://www.wpc.com.tw/>`_.
 
 +-------------------+-----------------------------------------------------------------------------------+
 |                   | Link                                                                              |
 +===================+===================================================================================+
 | WPC official site | http://www.wpc.com.tw/                                                            |
 +-------------------+-----------------------------------------------------------------------------------+
 | GitHub            | https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release                      |
@@ -64,15 +64,15 @@
 -----------
 **Easy, fast, and just works!**
 
    >>> from wpcsys import pywpc
    >>> pywpc.PKG_NAME
    pywpc
    >>> pywpc.HANDLE_LIST
-   ['DeviceFinder', 'WifiDAQE3A', 'WifiDAQF4A', 'STEM', 'EMotion', 'EDrive_ST', 'EthanA', 'EthanD', 'EthanL', 'EthanO', 'USBDAQF1D', 'USBDAQF1DSNK', 'USBDAQF1AD', 'USBDAQF1AOD', 'USBDAQF1TD', 'USBDAQF1RD', 'USBDAQF1CD']
+   ['DeviceFinder', 'WifiDAQE3A', 'WifiDAQF4A', 'STEM', 'EMotion', 'EDrive_ST', 'EthanA', 'EthanD', 'EthanI', 'EthanL', 'EthanO', 'EthanT', 'USBDAQF1D', 'USBDAQF1DSNK', 'USBDAQF1AD', 'USBDAQF1AOD', 'USBDAQF1TD', 'USBDAQF1RD', 'USBDAQF1CD']
 
 Install and Upgrade
 -------------------
 
 - Install
 
 .. code-block:: shell
@@ -106,18 +106,22 @@
 
 Ethernet based DAQ card
 
 - Ethan-A
 
 - Ethan-D
 
+- Ethan-I
+
 - Ethan-L
 
 - Ethan-O
 
+- Ethan-T
+
 USB interface DAQ card
 
 - USB-DAQ-F1-D (Digital)
 
 - USB-DAQ-F1-DSNK (24V Digital)
 
 - USB-DAQ-F1-AD (Digital + AI)
@@ -158,31 +162,33 @@
 +----------------+------+------+------+------+
 
 In the `STEM` product, the values 1, 2, and 4 are used to represent the slots in the AIO.
 Additionally, the DIO ports 0 to 1 are assigned to slot 1, while ports 2 to 3 are assigned to slot 2.
 
 - Ethan & Wifi series
 
-+----------------+-----+-----+----+----+
-| Product/module |AI   |AO   |DI  |DO  |
-+----------------+-----+-----+----+----+
-| Emotion        |     |     |    |    |
-+----------------+-----+-----+----+----+
-| Ethan-A        |0    |     |    |    |
-+----------------+-----+-----+----+----+
-| Ethan-D        |     |     |1   |0   |
-+----------------+-----+-----+----+----+
-| Ethan-L        |     |     |    |0   |
-+----------------+-----+-----+----+----+
-| Ethan-O        |     | 0   |    |    |
-+----------------+-----+-----+----+----+
-| Wifi-DAQ-E3-A  |0    |     |    |    |
-+----------------+-----+-----+----+----+
-| Wifi-DAQ-F4-A  |0    |     |    |    |
-+----------------+-----+-----+----+----+
++----------------+-----+-----+----+----+----+
+| Product/module |AI   |AO   |DI  |DO  |TC  |
++----------------+-----+-----+----+----+----+
+| Ethan-A        |0    |     |    |    |    |
++----------------+-----+-----+----+----+----+
+| Ethan-D        |     |     |1   |0   |    |
++----------------+-----+-----+----+----+----+
+| Ethan-I        |0    |     |    |    |    |
++----------------+-----+-----+----+----+----+
+| Ethan-L        |     |     |    |0   |    |
++----------------+-----+-----+----+----+----+
+| Ethan-O        |     | 0   |    |    |    |
++----------------+-----+-----+----+----+----+
+| Ethan-T        |     |     |    |    | 1  |
++----------------+-----+-----+----+----+----+
+| Wifi-DAQ-E3-A  |0    |     |    |    |    |
++----------------+-----+-----+----+----+----+
+| Wifi-DAQ-F4-A  |0    |     |    |    |    |
++----------------+-----+-----+----+----+----+
 
 - USB series
 
 +----------------+-----+-----+----+----+----+-----+-----+-----+----+---+
 | Product/module |AI   |AO   |DI  |DO  |CAN |UART |SPI  |I2C  |RTD |TC |
 +----------------+-----+-----+----+----+----+-----+-----+-----+----+---+
 | USB-DAQ-F1-D   |     |     |0~3 |0~3 |    |1, 2 |1, 2 |1, 2 |    |   |
```

### Comparing `wpcsys-2.1.5/setup.py` & `wpcsys-2.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `wpcsys-2.1.5/wpcsys/libusb-1.0.dll` & `wpcsys-2.1.6/wpcsys/libusb-1.0.dll`

 * *Files identical despite different names*

### Comparing `wpcsys-2.1.5/wpcsys.egg-info/PKG-INFO` & `wpcsys-2.1.6/wpcsys.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wpcsys
-Version: 2.1.5
+Version: 2.1.6
 Summary: WPC Python driver APIs, the easiest way to Control & Data Acquisition (DAQ)
 Home-page: https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release
 Author: chunglee_people, Chieh-An Lin
 Author-email: wu@wpc.com.tw
 License: MIT
 Keywords: wpc,daq,driver,usb,ethernet,wifi,data acquisition
 Classifier: Development Status :: 5 - Production/Stable
@@ -34,15 +34,15 @@
 
 Asynchronous mode means that processes run independently of each other and don't wait for the completion of the previous process. Instead, each process runs on its own, without blocking the execution of other processes.
 
 In general, synchronous mode is easier to understand and debug, while asynchronous mode is more scalable and allows for greater concurrency.
 
 Some API functions in the `pywpc` package may not compatible with earlier versions of WPC DAQ firmware.
 To update device firmware to the latest version, please use WPC Device Manager and `LabVIEW Run-time engine <https://drive.google.com/file/d/1Uj6r65KhNxvuApiqrMkZp-NWyq-Eek-k/view>`_.
-You can download WPC Device Manager by `latest release <https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release/releases/tag/v2.1.5>`_ or visit `WPC Systems Ltd. official website <http://www.wpc.com.tw/>`_.
+You can download WPC Device Manager by `latest release <https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release/releases/tag/v2.1.6>`_ or visit `WPC Systems Ltd. official website <http://www.wpc.com.tw/>`_.
 
 +-------------------+-----------------------------------------------------------------------------------+
 |                   | Link                                                                              |
 +===================+===================================================================================+
 | WPC official site | http://www.wpc.com.tw/                                                            |
 +-------------------+-----------------------------------------------------------------------------------+
 | GitHub            | https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release                      |
@@ -88,15 +88,15 @@
 -----------
 **Easy, fast, and just works!**
 
    >>> from wpcsys import pywpc
    >>> pywpc.PKG_NAME
    pywpc
    >>> pywpc.HANDLE_LIST
-   ['DeviceFinder', 'WifiDAQE3A', 'WifiDAQF4A', 'STEM', 'EMotion', 'EDrive_ST', 'EthanA', 'EthanD', 'EthanL', 'EthanO', 'USBDAQF1D', 'USBDAQF1DSNK', 'USBDAQF1AD', 'USBDAQF1AOD', 'USBDAQF1TD', 'USBDAQF1RD', 'USBDAQF1CD']
+   ['DeviceFinder', 'WifiDAQE3A', 'WifiDAQF4A', 'STEM', 'EMotion', 'EDrive_ST', 'EthanA', 'EthanD', 'EthanI', 'EthanL', 'EthanO', 'EthanT', 'USBDAQF1D', 'USBDAQF1DSNK', 'USBDAQF1AD', 'USBDAQF1AOD', 'USBDAQF1TD', 'USBDAQF1RD', 'USBDAQF1CD']
 
 Install and Upgrade
 -------------------
 
 - Install
 
 .. code-block:: shell
@@ -130,18 +130,22 @@
 
 Ethernet based DAQ card
 
 - Ethan-A
 
 - Ethan-D
 
+- Ethan-I
+
 - Ethan-L
 
 - Ethan-O
 
+- Ethan-T
+
 USB interface DAQ card
 
 - USB-DAQ-F1-D (Digital)
 
 - USB-DAQ-F1-DSNK (24V Digital)
 
 - USB-DAQ-F1-AD (Digital + AI)
@@ -182,31 +186,33 @@
 +----------------+------+------+------+------+
 
 In the `STEM` product, the values 1, 2, and 4 are used to represent the slots in the AIO.
 Additionally, the DIO ports 0 to 1 are assigned to slot 1, while ports 2 to 3 are assigned to slot 2.
 
 - Ethan & Wifi series
 
-+----------------+-----+-----+----+----+
-| Product/module |AI   |AO   |DI  |DO  |
-+----------------+-----+-----+----+----+
-| Emotion        |     |     |    |    |
-+----------------+-----+-----+----+----+
-| Ethan-A        |0    |     |    |    |
-+----------------+-----+-----+----+----+
-| Ethan-D        |     |     |1   |0   |
-+----------------+-----+-----+----+----+
-| Ethan-L        |     |     |    |0   |
-+----------------+-----+-----+----+----+
-| Ethan-O        |     | 0   |    |    |
-+----------------+-----+-----+----+----+
-| Wifi-DAQ-E3-A  |0    |     |    |    |
-+----------------+-----+-----+----+----+
-| Wifi-DAQ-F4-A  |0    |     |    |    |
-+----------------+-----+-----+----+----+
++----------------+-----+-----+----+----+----+
+| Product/module |AI   |AO   |DI  |DO  |TC  |
++----------------+-----+-----+----+----+----+
+| Ethan-A        |0    |     |    |    |    |
++----------------+-----+-----+----+----+----+
+| Ethan-D        |     |     |1   |0   |    |
++----------------+-----+-----+----+----+----+
+| Ethan-I        |0    |     |    |    |    |
++----------------+-----+-----+----+----+----+
+| Ethan-L        |     |     |    |0   |    |
++----------------+-----+-----+----+----+----+
+| Ethan-O        |     | 0   |    |    |    |
++----------------+-----+-----+----+----+----+
+| Ethan-T        |     |     |    |    | 1  |
++----------------+-----+-----+----+----+----+
+| Wifi-DAQ-E3-A  |0    |     |    |    |    |
++----------------+-----+-----+----+----+----+
+| Wifi-DAQ-F4-A  |0    |     |    |    |    |
++----------------+-----+-----+----+----+----+
 
 - USB series
 
 +----------------+-----+-----+----+----+----+-----+-----+-----+----+---+
 | Product/module |AI   |AO   |DI  |DO  |CAN |UART |SPI  |I2C  |RTD |TC |
 +----------------+-----+-----+----+----+----+-----+-----+-----+----+---+
 | USB-DAQ-F1-D   |     |     |0~3 |0~3 |    |1, 2 |1, 2 |1, 2 |    |   |
```

