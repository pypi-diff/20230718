# Comparing `tmp/stego-lsb-1.4.4.tar.gz` & `tmp/stego-lsb-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stego-lsb-1.4.4.tar", last modified: Wed Jul  5 19:39:17 2023, max compression
+gzip compressed data, was "stego-lsb-1.5.0.tar", last modified: Tue Jul 18 01:17:21 2023, max compression
```

## Comparing `stego-lsb-1.4.4.tar` & `stego-lsb-1.5.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-07-05 19:39:17.687523 stego-lsb-1.4.4/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      130 2022-06-05 03:00:51.000000 stego-lsb-1.4.4/AUTHORS.md
--rw-r--r--   0 ryan      (1000) ryan      (1000)     1077 2020-05-10 23:35:29.000000 stego-lsb-1.4.4/LICENSE.md
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     8788 2023-07-05 19:39:17.687523 stego-lsb-1.4.4/PKG-INFO
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     7968 2022-10-14 19:21:15.000000 stego-lsb-1.4.4/README.md
--rw-r--r--   0 ryan      (1000) ryan      (1000)       67 2023-07-05 19:39:17.687523 stego-lsb-1.4.4/setup.cfg
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     1481 2023-07-05 19:38:31.000000 stego-lsb-1.4.4/setup.py
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-07-05 19:39:17.687523 stego-lsb-1.4.4/stego_lsb/
--rwxrwxr-x   0 ryan      (1000) ryan      (1000)     7671 2023-02-08 00:44:44.000000 stego-lsb-1.4.4/stego_lsb/LSBSteg.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     1504 2023-02-07 02:21:16.000000 stego-lsb-1.4.4/stego_lsb/StegDetect.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     3951 2023-02-07 02:21:16.000000 stego-lsb-1.4.4/stego_lsb/WavSteg.py
--rw-r--r--   0 ryan      (1000) ryan      (1000)        0 2020-05-10 23:35:29.000000 stego-lsb-1.4.4/stego_lsb/__init__.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     6927 2023-02-07 02:21:16.000000 stego-lsb-1.4.4/stego_lsb/bit_manipulation.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     4483 2023-02-07 02:21:16.000000 stego-lsb-1.4.4/stego_lsb/cli.py
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-07-05 19:39:17.687523 stego-lsb-1.4.4/stego_lsb.egg-info/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     8788 2023-07-05 19:39:17.000000 stego-lsb-1.4.4/stego_lsb.egg-info/PKG-INFO
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      492 2023-07-05 19:39:17.000000 stego-lsb-1.4.4/stego_lsb.egg-info/SOURCES.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)        1 2023-07-05 19:39:17.000000 stego-lsb-1.4.4/stego_lsb.egg-info/dependency_links.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)       48 2023-07-05 19:39:17.000000 stego-lsb-1.4.4/stego_lsb.egg-info/entry_points.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)        1 2023-04-17 19:48:52.000000 stego-lsb-1.4.4/stego_lsb.egg-info/not-zip-safe
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      144 2023-07-05 19:39:17.000000 stego-lsb-1.4.4/stego_lsb.egg-info/requires.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)       10 2023-07-05 19:39:17.000000 stego-lsb-1.4.4/stego_lsb.egg-info/top_level.txt
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-07-05 19:39:17.687523 stego-lsb-1.4.4/tests/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     2215 2023-02-08 00:44:44.000000 stego-lsb-1.4.4/tests/test_bit_manipulation.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     2890 2023-02-08 00:44:44.000000 stego-lsb-1.4.4/tests/test_lsbsteg.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     3786 2023-02-08 00:44:44.000000 stego-lsb-1.4.4/tests/test_wavsteg.py
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-07-18 01:17:21.699273 stego-lsb-1.5.0/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      130 2022-06-05 03:00:51.000000 stego-lsb-1.5.0/AUTHORS.md
+-rw-r--r--   0 ryan      (1000) ryan      (1000)     1077 2020-05-10 23:35:29.000000 stego-lsb-1.5.0/LICENSE.md
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     8663 2023-07-18 01:17:21.699273 stego-lsb-1.5.0/PKG-INFO
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     7843 2023-07-18 00:12:47.000000 stego-lsb-1.5.0/README.md
+-rw-r--r--   0 ryan      (1000) ryan      (1000)       67 2023-07-18 01:17:21.699273 stego-lsb-1.5.0/setup.cfg
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1580 2023-07-18 00:12:47.000000 stego-lsb-1.5.0/setup.py
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-07-18 01:17:21.699273 stego-lsb-1.5.0/stego_lsb/
+-rwxrwxr-x   0 ryan      (1000) ryan      (1000)     8095 2023-07-18 01:01:17.000000 stego-lsb-1.5.0/stego_lsb/LSBSteg.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1451 2023-07-18 01:00:24.000000 stego-lsb-1.5.0/stego_lsb/StegDetect.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     3986 2023-07-18 01:00:24.000000 stego-lsb-1.5.0/stego_lsb/WavSteg.py
+-rw-r--r--   0 ryan      (1000) ryan      (1000)        0 2020-05-10 23:35:29.000000 stego-lsb-1.5.0/stego_lsb/__init__.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     6647 2023-07-18 00:12:47.000000 stego-lsb-1.5.0/stego_lsb/bit_manipulation.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     4285 2023-07-18 00:12:47.000000 stego-lsb-1.5.0/stego_lsb/cli.py
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-07-18 01:17:21.699273 stego-lsb-1.5.0/stego_lsb.egg-info/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     8663 2023-07-18 01:17:21.000000 stego-lsb-1.5.0/stego_lsb.egg-info/PKG-INFO
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      492 2023-07-18 01:17:21.000000 stego-lsb-1.5.0/stego_lsb.egg-info/SOURCES.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)        1 2023-07-18 01:17:21.000000 stego-lsb-1.5.0/stego_lsb.egg-info/dependency_links.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)       48 2023-07-18 01:17:21.000000 stego-lsb-1.5.0/stego_lsb.egg-info/entry_points.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)        1 2023-07-18 01:17:21.000000 stego-lsb-1.5.0/stego_lsb.egg-info/not-zip-safe
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      130 2023-07-18 01:17:21.000000 stego-lsb-1.5.0/stego_lsb.egg-info/requires.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)       10 2023-07-18 01:17:21.000000 stego-lsb-1.5.0/stego_lsb.egg-info/top_level.txt
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-07-18 01:17:21.699273 stego-lsb-1.5.0/tests/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     2069 2023-07-18 00:12:47.000000 stego-lsb-1.5.0/tests/test_bit_manipulation.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     3766 2023-07-18 01:00:24.000000 stego-lsb-1.5.0/tests/test_lsbsteg.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     3521 2023-07-18 01:00:24.000000 stego-lsb-1.5.0/tests/test_wavsteg.py
```

### Comparing `stego-lsb-1.4.4/LICENSE.md` & `stego-lsb-1.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `stego-lsb-1.4.4/PKG-INFO` & `stego-lsb-1.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stego-lsb
-Version: 1.4.4
+Version: 1.5.0
 Summary: stego lsb
 Home-page: https://github.com/ragibson/Steganography
 Author: Ryan Gibson
 Author-email: ryanalexandergibson@gmail.com
 License: MIT
 Keywords: stego lsb
 Classifier: Development Status :: 4 - Beta
@@ -23,35 +23,36 @@
 License-File: AUTHORS.md
 
 # Steganography
 
 ![Steganography illustration](readme_illustration.png)
 
 # Table of Contents
-  * [Installation](#Installation)
-  * [Byte Sequence Manipulation](#ByteSequenceManipulation)
-  * [WavSteg](#WavSteg)
-  * [LSBSteg](#LSBSteg)
-  * [StegDetect](#StegDetect)
 
-<a name = "Installation"></a>
+* [Installation](#installation)
+* [Byte Sequence Manipulation](#byte-sequence-manipulation)
+* [WavSteg](#wavsteg)
+* [LSBSteg](#lsbsteg)
+* [StegDetect](#stegdetect)
+
 ## Installation
+
 This project is on [PyPI](https://pypi.org/project/stego-lsb/) and can be
 installed with
 
     pip install stego-lsb
 
 Alternatively, you can install it from this repository directly:
 
     git clone https://github.com/ragibson/Steganography
     cd Steganography
     python3 setup.py install
 
-<a name = "ByteSequenceManipulation"></a>
 ## Byte Sequence Manipulation
+
 bit_manipulation provides the ability to (quickly) interleave the bytes of a
 payload directly in the least significant bits of a carrier byte sequence.
 
 Specifically, it contains four primary functions:
 
     # Interleave the bytes of payload into the num_lsb LSBs of carrier.
     lsb_interleave_bytes(carrier, payload, num_lsb, truncate=False)
@@ -78,23 +79,24 @@
     | 4      | 112.4  MB/s  | 105.9  MB/s  |
     | 5      | 135.9  MB/s  | 129.8  MB/s  |
     | 6      | 159.9  MB/s  | 152.4  MB/s  |
     | 7      | 181.7  MB/s  | 174.6  MB/s  |
     | 8      | 372.8  MB/s  | 1121.8 MB/s  |
     ----------------------------------------
 
-<a name = "WavSteg"></a>
 ## WavSteg
+
 WavSteg uses least significant bit steganography to hide a file in the samples
 of a .wav file.
 
 For each sample in the audio file, we overwrite the least significant bits with
 the data from our file.
 
 ### How to use
+
 WavSteg requires Python 3
 
 Run WavSteg with the following command line arguments:
 
     Command Line Arguments:
      -h, --hide               To hide data in a sound file
      -r, --recover            To recover data from a sound file
@@ -108,14 +110,15 @@
 Example:
 
     $ stegolsb wavsteg -h -i sound.wav -s file.txt -o sound_steg.wav -n 1
     # OR
     $ stegolsb wavsteg -r -i sound_steg.wav -o output.txt -n 1 -b 1000
 
 ### Hiding Data
+
 Hiding data uses the arguments -h, -i, -s, -o, and -n.
 
 The following command would hide the contents of file.txt into sound.wav and
 save the result as sound_steg.wav. The command also outputs how many bytes have
 been used out of a theoretical maximum.
 
 Example:
@@ -126,38 +129,40 @@
     5589889 bytes hidden           in 0.24s
     Output wav written             in 0.03s
 
 If you attempt to hide too much data, WavSteg will print the minimum number of
 LSBs required to hide your data.
 
 ### Recovering Data
+
 Recovering data uses the arguments -r, -i, -o, -n, and -b
 
 The following command would recover the hidden data from sound_steg.wav and
 save it as output.txt. This requires the size in bytes of the hidden data to
 be accurate or the result may be too short or contain extraneous data.
 
 Example:
 
     $ stegolsb wavsteg -r -i sound_steg.wav -o output.txt -n 2 -b 5589889
     Files read                     in 0.02s
     Recovered 5589889 bytes        in 0.18s
     Written output file            in 0.00s
 
-<a name = "LSBSteg"></a>
 ## LSBSteg
+
 LSBSteg uses least significant bit steganography to hide a file in the color
 information of an RGB image (.bmp or .png).
 
-For each color channel (R,G,B) in each pixel of the image, we overwrite the
-least significant bits of the color value with the data from our file.
-In order to make recovering this data easier, we also hide the file size
+For each color channel (e.g., R, G, and B) in each pixel of the image, we
+overwrite the least significant bits of the color value with the data from our
+file. In order to make recovering this data easier, we also hide the file size
 of our input file in the first few color channels of the image.
 
 ### How to use
+
 You need Python 3 and Pillow, a fork of the Python Imaging Library (PIL).
 
 Run LSBSteg with the following command line arguments:
 
     Command Line Arguments:
      -h, --hide                      To hide data in an image file
      -r, --recover                   To recover data from an image file
@@ -175,56 +180,61 @@
     $ stegolsb steglsb -a -i input_image.png -s input_file.zip -n 2
     # OR
     $ stegolsb steglsb -h -i input_image.png -s input_file.zip -o steg.png -n 2 -c 1
     # OR
     $ stegolsb steglsb -r -i steg.png -o output_file.zip -n 2
 
 ### Analyzing
-Before hiding data in an image, it can useful to see how much data can be
+
+Before hiding data in an image, it can be useful to see how much data can be
 hidden. The following command will achieve this, producing output similar to
 
     $ stegolsb steglsb -a -i input_image.png -s input_file.zip -n 2
-    Image resolution: (2000, 1100)
+    Image resolution: (2000, 1100, 3)
     Using 2 LSBs, we can hide:     1650000 B
     Size of input file:            1566763 B
     File size tag:                 3 B
 
 ### Hiding Data
+
 The following command will hide data in the input image and write the result to
 the steganographed image, producing output similar to
 
     $ stegolsb steglsb -h -i input_image.png -s input_file.zip -o steg.png -n 2 -c 1
     Files read                     in 0.26s
     1566763 bytes hidden           in 0.31s
     Image overwritten              in 0.27s
 
 ### Recovering Data
+
 The following command will recover data from the steganographed image and write
 the result to the output file, producing output similar to
 
     $ stegolsb steglsb -r -i steg.png -o output_file.zip -n 2
     Files read                     in 0.30s
     1566763 bytes recovered        in 0.28s
     Output file written            in 0.00s
 
-<a name = "StegDetect"></a>
 ## StegDetect
+
 StegDetect provides one method for detecting simple steganography in images.
 
 ### How to Use
+
 You need Python 3 and Pillow, a fork of the Python Imaging Library (PIL).
 
 Run StegDetect with the following command line arguments:
 
     Command Line Arguments:
      -i, --input TEXT         Path to an image
      -n, --lsb-count INTEGER  How many LSBs to display  [default: 2]
      --help                   Show this message and exit.
 
 ### Showing the Least Significant Bits of an Image
+
 We sum the least significant n bits of the RGB color channels for each pixel
 and normalize the result to the range 0-255. This value is then applied to each
 color channel for the pixel. Where n is the number of least significant bits to
 show, the following command will save the resulting image, appending "_nLSBs"
 to the file name, and will produce output similar to the following:
 
     $ stegolsb stegdetect -i input_image.png -n 2
```

### Comparing `stego-lsb-1.4.4/README.md` & `stego-lsb-1.5.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 # Steganography
 
 ![Steganography illustration](readme_illustration.png)
 
 # Table of Contents
-  * [Installation](#Installation)
-  * [Byte Sequence Manipulation](#ByteSequenceManipulation)
-  * [WavSteg](#WavSteg)
-  * [LSBSteg](#LSBSteg)
-  * [StegDetect](#StegDetect)
 
-<a name = "Installation"></a>
+* [Installation](#installation)
+* [Byte Sequence Manipulation](#byte-sequence-manipulation)
+* [WavSteg](#wavsteg)
+* [LSBSteg](#lsbsteg)
+* [StegDetect](#stegdetect)
+
 ## Installation
+
 This project is on [PyPI](https://pypi.org/project/stego-lsb/) and can be
 installed with
 
     pip install stego-lsb
 
 Alternatively, you can install it from this repository directly:
 
     git clone https://github.com/ragibson/Steganography
     cd Steganography
     python3 setup.py install
 
-<a name = "ByteSequenceManipulation"></a>
 ## Byte Sequence Manipulation
+
 bit_manipulation provides the ability to (quickly) interleave the bytes of a
 payload directly in the least significant bits of a carrier byte sequence.
 
 Specifically, it contains four primary functions:
 
     # Interleave the bytes of payload into the num_lsb LSBs of carrier.
     lsb_interleave_bytes(carrier, payload, num_lsb, truncate=False)
@@ -54,23 +55,24 @@
     | 4      | 112.4  MB/s  | 105.9  MB/s  |
     | 5      | 135.9  MB/s  | 129.8  MB/s  |
     | 6      | 159.9  MB/s  | 152.4  MB/s  |
     | 7      | 181.7  MB/s  | 174.6  MB/s  |
     | 8      | 372.8  MB/s  | 1121.8 MB/s  |
     ----------------------------------------
 
-<a name = "WavSteg"></a>
 ## WavSteg
+
 WavSteg uses least significant bit steganography to hide a file in the samples
 of a .wav file.
 
 For each sample in the audio file, we overwrite the least significant bits with
 the data from our file.
 
 ### How to use
+
 WavSteg requires Python 3
 
 Run WavSteg with the following command line arguments:
 
     Command Line Arguments:
      -h, --hide               To hide data in a sound file
      -r, --recover            To recover data from a sound file
@@ -84,14 +86,15 @@
 Example:
 
     $ stegolsb wavsteg -h -i sound.wav -s file.txt -o sound_steg.wav -n 1
     # OR
     $ stegolsb wavsteg -r -i sound_steg.wav -o output.txt -n 1 -b 1000
 
 ### Hiding Data
+
 Hiding data uses the arguments -h, -i, -s, -o, and -n.
 
 The following command would hide the contents of file.txt into sound.wav and
 save the result as sound_steg.wav. The command also outputs how many bytes have
 been used out of a theoretical maximum.
 
 Example:
@@ -102,38 +105,40 @@
     5589889 bytes hidden           in 0.24s
     Output wav written             in 0.03s
 
 If you attempt to hide too much data, WavSteg will print the minimum number of
 LSBs required to hide your data.
 
 ### Recovering Data
+
 Recovering data uses the arguments -r, -i, -o, -n, and -b
 
 The following command would recover the hidden data from sound_steg.wav and
 save it as output.txt. This requires the size in bytes of the hidden data to
 be accurate or the result may be too short or contain extraneous data.
 
 Example:
 
     $ stegolsb wavsteg -r -i sound_steg.wav -o output.txt -n 2 -b 5589889
     Files read                     in 0.02s
     Recovered 5589889 bytes        in 0.18s
     Written output file            in 0.00s
 
-<a name = "LSBSteg"></a>
 ## LSBSteg
+
 LSBSteg uses least significant bit steganography to hide a file in the color
 information of an RGB image (.bmp or .png).
 
-For each color channel (R,G,B) in each pixel of the image, we overwrite the
-least significant bits of the color value with the data from our file.
-In order to make recovering this data easier, we also hide the file size
+For each color channel (e.g., R, G, and B) in each pixel of the image, we
+overwrite the least significant bits of the color value with the data from our
+file. In order to make recovering this data easier, we also hide the file size
 of our input file in the first few color channels of the image.
 
 ### How to use
+
 You need Python 3 and Pillow, a fork of the Python Imaging Library (PIL).
 
 Run LSBSteg with the following command line arguments:
 
     Command Line Arguments:
      -h, --hide                      To hide data in an image file
      -r, --recover                   To recover data from an image file
@@ -151,56 +156,61 @@
     $ stegolsb steglsb -a -i input_image.png -s input_file.zip -n 2
     # OR
     $ stegolsb steglsb -h -i input_image.png -s input_file.zip -o steg.png -n 2 -c 1
     # OR
     $ stegolsb steglsb -r -i steg.png -o output_file.zip -n 2
 
 ### Analyzing
-Before hiding data in an image, it can useful to see how much data can be
+
+Before hiding data in an image, it can be useful to see how much data can be
 hidden. The following command will achieve this, producing output similar to
 
     $ stegolsb steglsb -a -i input_image.png -s input_file.zip -n 2
-    Image resolution: (2000, 1100)
+    Image resolution: (2000, 1100, 3)
     Using 2 LSBs, we can hide:     1650000 B
     Size of input file:            1566763 B
     File size tag:                 3 B
 
 ### Hiding Data
+
 The following command will hide data in the input image and write the result to
 the steganographed image, producing output similar to
 
     $ stegolsb steglsb -h -i input_image.png -s input_file.zip -o steg.png -n 2 -c 1
     Files read                     in 0.26s
     1566763 bytes hidden           in 0.31s
     Image overwritten              in 0.27s
 
 ### Recovering Data
+
 The following command will recover data from the steganographed image and write
 the result to the output file, producing output similar to
 
     $ stegolsb steglsb -r -i steg.png -o output_file.zip -n 2
     Files read                     in 0.30s
     1566763 bytes recovered        in 0.28s
     Output file written            in 0.00s
 
-<a name = "StegDetect"></a>
 ## StegDetect
+
 StegDetect provides one method for detecting simple steganography in images.
 
 ### How to Use
+
 You need Python 3 and Pillow, a fork of the Python Imaging Library (PIL).
 
 Run StegDetect with the following command line arguments:
 
     Command Line Arguments:
      -i, --input TEXT         Path to an image
      -n, --lsb-count INTEGER  How many LSBs to display  [default: 2]
      --help                   Show this message and exit.
 
 ### Showing the Least Significant Bits of an Image
+
 We sum the least significant n bits of the RGB color channels for each pixel
 and normalize the result to the range 0-255. This value is then applied to each
 color channel for the pixel. Where n is the number of least significant bits to
 show, the following command will save the resulting image, appending "_nLSBs"
 to the file name, and will produce output similar to the following:
 
     $ stegolsb stegdetect -i input_image.png -n 2
```

### Comparing `stego-lsb-1.4.4/setup.py` & `stego-lsb-1.5.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 # -*- coding: utf-8 -*-
 from setuptools import find_packages, setup
 
 with open("README.md") as readme_file:
     readme = readme_file.read()
 
 requirements = [
-    "Pillow>=5.3.0",
-    "numpy>=1.15.4,<1.25.0; python_version>='3.8' and python_version<'3.9'",
-    "numpy>=1.15.4; python_version>='3.9'",
-    "Click>=7.0",
+    # TODO: remove Click restriction after release of 8.1.6 or merge of
+    #  https://github.com/pallets/click/pull/2565
+    "Click<8.1.4", "Pillow", "numpy; python_version>='3.9'",
+    "numpy>=1.15.4,<1.25.0; python_version>='3.8' and python_version<'3.9'"
 ]
 
 setup(
     author="Ryan Gibson",
     author_email="ryanalexandergibson@gmail.com",
     name="stego-lsb",
-    version="1.4.4",
+    version="1.5.0",
     description="stego lsb",
     keywords="stego lsb",
     license="MIT",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/ragibson/Steganography",
     install_requires=requirements,
```

### Comparing `stego-lsb-1.4.4/stego_lsb/StegDetect.py` & `stego-lsb-1.5.0/stego_lsb/StegDetect.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,38 +12,32 @@
 """
 from PIL import Image
 from time import time
 from typing import cast, Tuple, Iterable
 import logging
 import os
 
-
 log = logging.getLogger(__name__)
 
 
 def show_lsb(image_path: str, n: int) -> None:
     """Shows the n least significant bits of image"""
     if image_path is None:
         raise ValueError("StegDetect requires an input image file path")
 
     start = time()
-    image = Image.open(image_path)
-
-    # Used to set everything but the least significant n bits to 0 when
-    # using bitwise AND on an integer
-    mask = (1 << n) - 1
-
-    image_data = cast(Iterable[Tuple[int, int, int]], image.getdata())
-    color_data = [
-        (255 * ((rgb[0] & mask) + (rgb[1] & mask) + (rgb[2] & mask)) // (3 * mask),) * 3
-        for rgb in image_data
-    ]
-
-    # TODO: image.putdata() appears to have buggy typing?
-    image.putdata(color_data)  # type: ignore
-    log.debug(f"Runtime: {time() - start:.2f}s")
-    file_name, file_extension = os.path.splitext(image_path)
-    image.save(file_name + "_{}LSBs".format(n) + file_extension)
-
-
-if __name__ == "__main__":
-    show_lsb("/home/ryan/Desktop/featured-improve-test-taking.png", 1)
+    with Image.open(image_path) as image:
+        # Used to set everything but the least significant n bits to 0 when
+        # using bitwise AND on an integer
+        mask = (1 << n) - 1
+
+        image_data = cast(Iterable[Tuple[int, int, int]], image.getdata())
+        color_data = [
+            (255 * ((rgb[0] & mask) + (rgb[1] & mask) + (rgb[2] & mask)) // (3 * mask),) * 3
+            for rgb in image_data
+        ]
+
+        # TODO: image.putdata() appears to have buggy typing?
+        image.putdata(color_data)  # type: ignore
+        log.debug(f"Runtime: {time() - start:.2f}s")
+        file_name, file_extension = os.path.splitext(image_path)
+        image.save(f"{file_name}_{n}LSBs{file_extension}")
```

### Comparing `stego-lsb-1.4.4/stego_lsb/WavSteg.py` & `stego-lsb-1.5.0/stego_lsb/WavSteg.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,102 +12,86 @@
 from stego_lsb.bit_manipulation import lsb_deinterleave_bytes, lsb_interleave_bytes
 from time import time
 import logging
 import math
 import os
 import wave
 
-
 log = logging.getLogger(__name__)
 
 
 def hide_data(sound_path: str, file_path: str, output_path: str, num_lsb: int) -> None:
     """Hide data from the file at file_path in the sound file at sound_path"""
     if sound_path is None:
         raise ValueError("WavSteg hiding requires an input sound file path")
     if file_path is None:
         raise ValueError("WavSteg hiding requires a secret file path")
     if output_path is None:
         raise ValueError("WavSteg hiding requires an output sound file path")
 
-    sound = wave.open(sound_path, "r")
-
-    params = sound.getparams()
-    num_channels = sound.getnchannels()
-    sample_width = sound.getsampwidth()
-    num_frames = sound.getnframes()
-    num_samples = num_frames * num_channels
-
-    # We can hide up to num_lsb bits in each sample of the sound file
-    max_bytes_to_hide = (num_samples * num_lsb) // 8
-    file_size = os.stat(file_path).st_size
-
-    log.debug(f"Using {num_lsb} LSBs, we can hide {max_bytes_to_hide} bytes")
-
-    start = time()
-    sound_frames = sound.readframes(num_frames)
-    with open(file_path, "rb") as file:
-        data = file.read()
-    log.debug("Files read".ljust(30) + f" in {time() - start:.2f}s")
-
-    if file_size > max_bytes_to_hide:
-        required_lsb = math.ceil(file_size * 8 / num_samples)
-        raise ValueError(
-            "Input file too large to hide, "
-            f"requires {required_lsb} LSBs, using {num_lsb}"
-        )
-
-    if sample_width != 1 and sample_width != 2:
-        # Python's wave module doesn't support higher sample widths
-        raise ValueError("File has an unsupported bit-depth")
-
-    start = time()
-    sound_frames = lsb_interleave_bytes(
-        sound_frames, data, num_lsb, byte_depth=sample_width
-    )
-    log.debug(f"{file_size} bytes hidden".ljust(30) + f" in {time() - start:.2f}s")
-
-    start = time()
-    sound_steg = wave.open(output_path, "w")
-    sound_steg.setparams(params)
-    sound_steg.writeframes(sound_frames)
-    sound_steg.close()
-    log.debug("Output wav written".ljust(30) + f" in {time() - start:.2f}s")
+    with wave.open(sound_path, "r") as sound:
+        params = sound.getparams()
+        num_channels = sound.getnchannels()
+        sample_width = sound.getsampwidth()
+        num_frames = sound.getnframes()
+        num_samples = num_frames * num_channels
+
+        # We can hide up to num_lsb bits in each sample of the sound file
+        max_bytes_to_hide = (num_samples * num_lsb) // 8
+        file_size = os.stat(file_path).st_size
+
+        log.debug(f"Using {num_lsb} LSBs, we can hide {max_bytes_to_hide} bytes")
+
+        start = time()
+        sound_frames = sound.readframes(num_frames)
+        with open(file_path, "rb") as file:
+            data = file.read()
+        log.debug(f"{'Files read':<30} in {time() - start:.2f}s")
+
+        if file_size > max_bytes_to_hide:
+            required_lsb = math.ceil(file_size * 8 / num_samples)
+            raise ValueError(f"Input file too large to hide, requires {required_lsb} LSBs, using {num_lsb}")
+
+        if sample_width != 1 and sample_width != 2:
+            # Python's wave module doesn't support higher sample widths
+            raise ValueError("File has an unsupported bit-depth")
+
+        start = time()
+        sound_frames = lsb_interleave_bytes(sound_frames, data, num_lsb, byte_depth=sample_width)
+        log.debug(f"{f'{file_size} bytes hidden':<30} in {time() - start:.2f}s")
+
+        start = time()
+        with wave.open(output_path, "w") as sound_steg:
+            sound_steg.setparams(params)
+            sound_steg.writeframes(sound_frames)
+        log.debug(f"{'Output wav written':<30} in {time() - start:.2f}s")
 
 
-def recover_data(
-    sound_path: str, output_path: str, num_lsb: int, bytes_to_recover: int
-) -> None:
+def recover_data(sound_path: str, output_path: str, num_lsb: int, bytes_to_recover: int) -> None:
     """Recover data from the file at sound_path to the file at output_path"""
     if sound_path is None:
         raise ValueError("WavSteg recovery requires an input sound file path")
     if output_path is None:
         raise ValueError("WavSteg recovery requires an output file path")
     if bytes_to_recover is None:
         raise ValueError("WavSteg recovery requires the number of bytes to recover")
 
     start = time()
-    sound = wave.open(sound_path, "r")
-
-    # num_channels = sound.getnchannels()
-    sample_width = sound.getsampwidth()
-    num_frames = sound.getnframes()
-    sound_frames = sound.readframes(num_frames)
-    log.debug("Files read".ljust(30) + f" in {time() - start:.2f}s")
-
-    if sample_width != 1 and sample_width != 2:
-        # Python's wave module doesn't support higher sample widths
-        raise ValueError("File has an unsupported bit-depth")
-
-    start = time()
-    data = lsb_deinterleave_bytes(
-        sound_frames, 8 * bytes_to_recover, num_lsb, byte_depth=sample_width
-    )
-    log.debug(
-        f"Recovered {bytes_to_recover} bytes".ljust(30) + f" in {time() - start:.2f}s"
-    )
-
-    start = time()
-    output_file = open(output_path, "wb+")
-    output_file.write(bytes(data))
-    output_file.close()
-    log.debug("Written output file".ljust(30) + f" in {time() - start:.2f}s")
+    with wave.open(sound_path, "r") as sound:
+        # num_channels = sound.getnchannels()
+        sample_width = sound.getsampwidth()
+        num_frames = sound.getnframes()
+        sound_frames = sound.readframes(num_frames)
+        log.debug(f"{'Files read':<30} in {time() - start:.2f}s")
+
+        if sample_width != 1 and sample_width != 2:
+            # Python's wave module doesn't support higher sample widths
+            raise ValueError("File has an unsupported bit-depth")
+
+        start = time()
+        data = lsb_deinterleave_bytes(sound_frames, 8 * bytes_to_recover, num_lsb, byte_depth=sample_width)
+        log.debug(f"{f'Recovered {bytes_to_recover} bytes':<30} in {time() - start:.2f}s")
+
+        start = time()
+        with open(output_path, "wb+") as output_file:
+            output_file.write(bytes(data))
+        log.debug(f"{'Written output file':<30} in {time() - start:.2f}s")
```

### Comparing `stego-lsb-1.4.4/stego_lsb/bit_manipulation.py` & `stego-lsb-1.5.0/stego_lsb/bit_manipulation.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,133 +29,104 @@
 byte_depth_to_dtype = {1: np.uint8, 2: np.uint16, 4: np.uint32, 8: np.uint64}
 
 
 def roundup(x: float, base: int = 1) -> int:
     return int(ceil(x / base)) * base
 
 
-def lsb_interleave_bytes(
-    carrier: bytes,
-    payload: bytes,
-    num_lsb: int,
-    truncate: bool = False,
-    byte_depth: int = 1,
-) -> bytes:
+def lsb_interleave_bytes(carrier: bytes, payload: bytes, num_lsb: int, truncate: bool = False,
+                         byte_depth: int = 1) -> bytes:
     """
     Interleave the bytes of payload into the num_lsb LSBs of carrier.
 
     :param carrier: carrier bytes
     :param payload: payload bytes
     :param num_lsb: number of least significant bits to use
     :param truncate: if True, will only return the interleaved part
     :param byte_depth: byte depth of carrier values
     :return: The interleaved bytes
     """
 
     plen = len(payload)
     payload_bits = np.zeros(shape=(plen, 8), dtype=np.uint8)
-    payload_bits[:plen, :] = np.unpackbits(
-        np.frombuffer(payload, dtype=np.uint8, count=plen)
-    ).reshape(plen, 8)
+    payload_bits[:plen, :] = np.unpackbits(np.frombuffer(payload, dtype=np.uint8, count=plen)).reshape(plen, 8)
 
     bit_height = roundup(plen * 8 / num_lsb)
     payload_bits.resize(bit_height * num_lsb)
 
     carrier_dtype = byte_depth_to_dtype[byte_depth]
-    carrier_bits = np.unpackbits(
-        np.frombuffer(carrier, dtype=carrier_dtype, count=bit_height).view(np.uint8)
-    ).reshape(bit_height, 8 * byte_depth)
-
-    carrier_bits[:, 8 * byte_depth - num_lsb : 8 * byte_depth] = payload_bits.reshape(
-        bit_height, num_lsb
-    )
+    carrier_bits = np.unpackbits(np.frombuffer(carrier, dtype=carrier_dtype, count=bit_height).view(np.uint8)
+                                 ).reshape(bit_height, 8 * byte_depth)
+
+    carrier_bits[:, 8 * byte_depth - num_lsb: 8 * byte_depth] = payload_bits.reshape(bit_height, num_lsb)
 
     ret = np.packbits(carrier_bits).tobytes()
-    return ret if truncate else ret + carrier[byte_depth * bit_height :]
+    return ret if truncate else ret + carrier[byte_depth * bit_height:]
 
 
-def lsb_deinterleave_bytes(
-    carrier: bytes, num_bits: int, num_lsb: int, byte_depth: int = 1
-) -> bytes:
+def lsb_deinterleave_bytes(carrier: bytes, num_bits: int, num_lsb: int, byte_depth: int = 1) -> bytes:
     """
     Deinterleave num_bits bits from the num_lsb LSBs of carrier.
 
     :param carrier: carrier bytes
     :param num_bits: number of num_bits to retrieve
     :param num_lsb: number of least significant bits to use
     :param byte_depth: byte depth of carrier values
     :return: The deinterleaved bytes
     """
 
     plen = roundup(num_bits / num_lsb)
     carrier_dtype = byte_depth_to_dtype[byte_depth]
-    payload_bits = np.unpackbits(
-        np.frombuffer(carrier, dtype=carrier_dtype, count=plen).view(np.uint8)
-    ).reshape(plen, 8 * byte_depth)[:, 8 * byte_depth - num_lsb : 8 * byte_depth]
+    payload_bits = np.unpackbits(np.frombuffer(carrier, dtype=carrier_dtype, count=plen).view(np.uint8)
+                                 ).reshape(plen, 8 * byte_depth)[:, 8 * byte_depth - num_lsb: 8 * byte_depth]
     return np.packbits(payload_bits).tobytes()[: num_bits // 8]
 
 
-def lsb_interleave_list(
-    carrier: List[np.uint8], payload: bytes, num_lsb: int
-) -> List[np.uint8]:
+def lsb_interleave_list(carrier: List[np.uint8], payload: bytes, num_lsb: int) -> List[np.uint8]:
     """Runs lsb_interleave_bytes with a List[uint8] carrier.
 
     This is slower than working with bytes directly, but is often
     unavoidable if working with libraries that require using lists."""
     bit_height = roundup(8 * len(payload) / num_lsb)
     carrier_bytes = np.array(carrier[:bit_height], dtype=np.uint8).tobytes()
     interleaved = lsb_interleave_bytes(carrier_bytes, payload, num_lsb, truncate=True)
     carrier[:bit_height] = np.frombuffer(interleaved, dtype=np.uint8).tolist()
     return carrier
 
 
-def lsb_deinterleave_list(
-    carrier: List[np.uint8], num_bits: int, num_lsb: int
-) -> bytes:
+def lsb_deinterleave_list(carrier: List[np.uint8], num_bits: int, num_lsb: int) -> bytes:
     """Runs lsb_deinterleave_bytes with a List[uint8] carrier.
 
     This is slower than working with bytes directly, but is often
     unavoidable if working with libraries that require using lists."""
     plen = roundup(num_bits / num_lsb)
     carrier_bytes = np.array(carrier[:plen], dtype=np.uint8).tobytes()
     deinterleaved = lsb_deinterleave_bytes(carrier_bytes, num_bits, num_lsb)
     return deinterleaved
 
 
-def test(carrier_len: int = 10**7, payload_len: int = 10**6) -> bool:
+def test(carrier_len: int = 10 ** 7, payload_len: int = 10 ** 6) -> bool:
     """Runs consistency tests with a random carrier and payload of byte
     lengths carrier_len and payload_len, respectively."""
 
     def print_results(e_rates: List[str], d_rates: List[str]) -> None:
         print("\n" + "-" * 40)
-        row_fmt = "| {:<7}| {:<13}| {:<13}|"
-        print(row_fmt.format("# LSBs", "Encode Rate", "Decode rate"))
+        print(f"| {'# LSBs':<7}| {'Encode Rate':<13}| {'Decode rate':<13}|")
         for n, e, d in zip(range(1, 9), e_rates[1:], d_rates[1:]):
-            print(row_fmt.format(n, e, d))
+            print(f"| {n:<7}| {e:<13}| {d:<13}|")
         print("-" * 40)
 
     current_progress = 0
 
     def progress() -> None:
         nonlocal current_progress
-        print(
-            "\rProgress: ["
-            + "#" * current_progress
-            + "-" * (32 - current_progress)
-            + "]",
-            end="",
-            flush=True,
-        )
+        print(f"\rProgress: [{'#' * current_progress}{'-' * (32 - current_progress)}]", end="", flush=True)
         current_progress += 1
 
-    print(
-        "Testing {:.1f} MB payload -> {:.1f} MB carrier...".format(
-            payload_len / 1e6, carrier_len / 1e6
-        )
-    )
+    print(f"Testing {payload_len / 1e6:.1f} MB payload -> {carrier_len / 1e6:.1f} MB carrier...")
     progress()
 
     carrier = os.urandom(carrier_len)
     payload = os.urandom(payload_len)
     encode_rates = [""] * 9
     decode_rates = [""] * 9
 
@@ -164,35 +135,28 @@
         encoded = lsb_interleave_bytes(carrier, payload, num_lsb)
         progress()
         decoded = lsb_deinterleave_bytes(encoded, 8 * payload_len, num_lsb)
         progress()
 
         # truncated LSB interleavings
         encode_time = time()
-        truncated_encode = lsb_interleave_bytes(
-            carrier, payload, num_lsb, truncate=True
-        )
+        truncated_encode = lsb_interleave_bytes(carrier, payload, num_lsb, truncate=True)
         encode_time = time() - encode_time
         progress()
+
         decode_time = time()
-        truncated_decode = lsb_deinterleave_bytes(
-            truncated_encode, 8 * payload_len, num_lsb
-        )
+        truncated_decode = lsb_deinterleave_bytes(truncated_encode, 8 * payload_len, num_lsb)
         decode_time = time() - decode_time
         progress()
 
-        encode_rates[num_lsb] = "{:<6.1f} MB/s".format(
-            (payload_len / 1e6) / encode_time
-        )
-        decode_rates[num_lsb] = "{:<6.1f} MB/s".format(
-            (payload_len / 1e6) / decode_time
-        )
+        encode_rates[num_lsb] = f"{(payload_len / 1e6) / encode_time:<6.1f} MB/s"
+        decode_rates[num_lsb] = f"{(payload_len / 1e6) / decode_time:<6.1f} MB/s"
 
         if decoded != payload or truncated_decode != payload:
-            print("\nTest failed at {} LSBs!".format(num_lsb))
+            print(f"\nTest failed at {num_lsb} LSBs!")
             return False
 
     print_results(encode_rates, decode_rates)
     return True
 
 
 if __name__ == "__main__":
```

### Comparing `stego-lsb-1.4.4/stego_lsb/cli.py` & `stego-lsb-1.5.0/stego_lsb/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -29,58 +29,26 @@
 @click.version_option()
 def main() -> None:
     """Console script for stegolsb."""
 
 
 @main.command(context_settings=dict(max_content_width=120))
 @click.option("--hide", "-h", is_flag=True, help="To hide data in an image file")
-@click.option(
-    "--recover", "-r", is_flag=True, help="To recover data from an image file"
-)
-@click.option(
-    "--analyze",
-    "-a",
-    is_flag=True,
-    default=False,
-    show_default=True,
-    help="Print how much data can be hidden within an image",
-)
-@click.option(
-    "--input", "-i", "input_fp", help="Path to an bitmap (.bmp or .png) image"
-)
+@click.option("--recover", "-r", is_flag=True, help="To recover data from an image file")
+@click.option("--analyze", "-a", is_flag=True, default=False, show_default=True,
+              help="Print how much data can be hidden within an image")
+@click.option("--input", "-i", "input_fp", help="Path to an bitmap (.bmp or .png) image")
 @click.option("--secret", "-s", "secret_fp", help="Path to a file to hide in the image")
 @click.option("--output", "-o", "output_fp", help="Path to an output file")
-@click.option(
-    "--lsb-count",
-    "-n",
-    default=2,
-    show_default=True,
-    help="How many LSBs to use",
-    type=int,
-)
-@click.option(
-    "--compression",
-    "-c",
-    help="1 (best speed) to 9 (smallest file size)",
-    default=1,
-    show_default=True,
-    type=click.IntRange(1, 9),
-)
+@click.option("--lsb-count", "-n", default=2, show_default=True, help="How many LSBs to use", type=int)
+@click.option("--compression", "-c", help="1 (best speed) to 9 (smallest file size)", default=1, show_default=True,
+              type=click.IntRange(1, 9))
 @click.pass_context
-def steglsb(
-    ctx: click.Context,
-    hide: bool,
-    recover: bool,
-    analyze: bool,
-    input_fp: str,
-    secret_fp: str,
-    output_fp: str,
-    lsb_count: int,
-    compression: int,
-) -> None:
+def steglsb(ctx: click.Context, hide: bool, recover: bool, analyze: bool, input_fp: str, secret_fp: str, output_fp: str,
+            lsb_count: int, compression: int) -> None:
     """Hides or recovers data in and from an image"""
     try:
         if analyze:
             LSBSteg.analysis(input_fp, secret_fp, lsb_count)
 
         if hide:
             LSBSteg.hide_data(input_fp, secret_fp, output_fp, lsb_count, compression)
@@ -92,65 +60,35 @@
     except ValueError as e:
         log.debug(e)
         click.echo(ctx.get_help())
 
 
 @main.command()
 @click.option("--input", "-i", "image_path", help="Path to an image")
-@click.option(
-    "--lsb-count",
-    "-n",
-    default=2,
-    show_default=2,
-    type=int,
-    help="How many LSBs to display",
-)
+@click.option("--lsb-count", "-n", default=2, show_default=2, type=int, help="How many LSBs to display")
 @click.pass_context
 def stegdetect(ctx: click.Context, image_path: str, lsb_count: int) -> None:
     """Shows the n least significant bits of image"""
     if image_path:
         StegDetect.show_lsb(image_path, lsb_count)
     else:
         click.echo(ctx.get_help())
 
 
 @main.command()
 @click.option("--hide", "-h", is_flag=True, help="To hide data in a sound file")
 @click.option("--recover", "-r", is_flag=True, help="To recover data from a sound file")
 @click.option("--input", "-i", "input_fp", help="Path to a .wav file")
-@click.option(
-    "--secret", "-s", "secret_fp", help="Path to a file to hide in the sound file"
-)
+@click.option("--secret", "-s", "secret_fp", help="Path to a file to hide in the sound file")
 @click.option("--output", "-o", "output_fp", help="Path to an output file")
-@click.option(
-    "--lsb-count",
-    "-n",
-    default=2,
-    show_default=True,
-    help="How many LSBs to use",
-    type=int,
-)
-@click.option(
-    "--bytes",
-    "-b",
-    "num_bytes",
-    help="How many bytes to recover from the sound file",
-    type=int,
-)
+@click.option("--lsb-count", "-n", default=2, show_default=True, help="How many LSBs to use", type=int)
+@click.option("--bytes", "-b", "num_bytes", help="How many bytes to recover from the sound file", type=int)
 @click.pass_context
-def wavsteg(
-    ctx: click.Context,
-    hide: bool,
-    recover: bool,
-    input_fp: str,
-    secret_fp: str,
-    output_fp: str,
-    lsb_count: int,
-    num_bytes: int,
-) -> None:
+def wavsteg(ctx: click.Context, hide: bool, recover: bool, input_fp: str, secret_fp: str, output_fp: str,
+            lsb_count: int, num_bytes: int) -> None:
     """Hides or recovers data in and from a sound file"""
     try:
         if hide:
             WavSteg.hide_data(input_fp, secret_fp, output_fp, lsb_count)
         elif recover:
             WavSteg.recover_data(input_fp, output_fp, lsb_count, num_bytes)
         else:
```

### Comparing `stego-lsb-1.4.4/stego_lsb.egg-info/PKG-INFO` & `stego-lsb-1.5.0/stego_lsb.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stego-lsb
-Version: 1.4.4
+Version: 1.5.0
 Summary: stego lsb
 Home-page: https://github.com/ragibson/Steganography
 Author: Ryan Gibson
 Author-email: ryanalexandergibson@gmail.com
 License: MIT
 Keywords: stego lsb
 Classifier: Development Status :: 4 - Beta
@@ -23,35 +23,36 @@
 License-File: AUTHORS.md
 
 # Steganography
 
 ![Steganography illustration](readme_illustration.png)
 
 # Table of Contents
-  * [Installation](#Installation)
-  * [Byte Sequence Manipulation](#ByteSequenceManipulation)
-  * [WavSteg](#WavSteg)
-  * [LSBSteg](#LSBSteg)
-  * [StegDetect](#StegDetect)
 
-<a name = "Installation"></a>
+* [Installation](#installation)
+* [Byte Sequence Manipulation](#byte-sequence-manipulation)
+* [WavSteg](#wavsteg)
+* [LSBSteg](#lsbsteg)
+* [StegDetect](#stegdetect)
+
 ## Installation
+
 This project is on [PyPI](https://pypi.org/project/stego-lsb/) and can be
 installed with
 
     pip install stego-lsb
 
 Alternatively, you can install it from this repository directly:
 
     git clone https://github.com/ragibson/Steganography
     cd Steganography
     python3 setup.py install
 
-<a name = "ByteSequenceManipulation"></a>
 ## Byte Sequence Manipulation
+
 bit_manipulation provides the ability to (quickly) interleave the bytes of a
 payload directly in the least significant bits of a carrier byte sequence.
 
 Specifically, it contains four primary functions:
 
     # Interleave the bytes of payload into the num_lsb LSBs of carrier.
     lsb_interleave_bytes(carrier, payload, num_lsb, truncate=False)
@@ -78,23 +79,24 @@
     | 4      | 112.4  MB/s  | 105.9  MB/s  |
     | 5      | 135.9  MB/s  | 129.8  MB/s  |
     | 6      | 159.9  MB/s  | 152.4  MB/s  |
     | 7      | 181.7  MB/s  | 174.6  MB/s  |
     | 8      | 372.8  MB/s  | 1121.8 MB/s  |
     ----------------------------------------
 
-<a name = "WavSteg"></a>
 ## WavSteg
+
 WavSteg uses least significant bit steganography to hide a file in the samples
 of a .wav file.
 
 For each sample in the audio file, we overwrite the least significant bits with
 the data from our file.
 
 ### How to use
+
 WavSteg requires Python 3
 
 Run WavSteg with the following command line arguments:
 
     Command Line Arguments:
      -h, --hide               To hide data in a sound file
      -r, --recover            To recover data from a sound file
@@ -108,14 +110,15 @@
 Example:
 
     $ stegolsb wavsteg -h -i sound.wav -s file.txt -o sound_steg.wav -n 1
     # OR
     $ stegolsb wavsteg -r -i sound_steg.wav -o output.txt -n 1 -b 1000
 
 ### Hiding Data
+
 Hiding data uses the arguments -h, -i, -s, -o, and -n.
 
 The following command would hide the contents of file.txt into sound.wav and
 save the result as sound_steg.wav. The command also outputs how many bytes have
 been used out of a theoretical maximum.
 
 Example:
@@ -126,38 +129,40 @@
     5589889 bytes hidden           in 0.24s
     Output wav written             in 0.03s
 
 If you attempt to hide too much data, WavSteg will print the minimum number of
 LSBs required to hide your data.
 
 ### Recovering Data
+
 Recovering data uses the arguments -r, -i, -o, -n, and -b
 
 The following command would recover the hidden data from sound_steg.wav and
 save it as output.txt. This requires the size in bytes of the hidden data to
 be accurate or the result may be too short or contain extraneous data.
 
 Example:
 
     $ stegolsb wavsteg -r -i sound_steg.wav -o output.txt -n 2 -b 5589889
     Files read                     in 0.02s
     Recovered 5589889 bytes        in 0.18s
     Written output file            in 0.00s
 
-<a name = "LSBSteg"></a>
 ## LSBSteg
+
 LSBSteg uses least significant bit steganography to hide a file in the color
 information of an RGB image (.bmp or .png).
 
-For each color channel (R,G,B) in each pixel of the image, we overwrite the
-least significant bits of the color value with the data from our file.
-In order to make recovering this data easier, we also hide the file size
+For each color channel (e.g., R, G, and B) in each pixel of the image, we
+overwrite the least significant bits of the color value with the data from our
+file. In order to make recovering this data easier, we also hide the file size
 of our input file in the first few color channels of the image.
 
 ### How to use
+
 You need Python 3 and Pillow, a fork of the Python Imaging Library (PIL).
 
 Run LSBSteg with the following command line arguments:
 
     Command Line Arguments:
      -h, --hide                      To hide data in an image file
      -r, --recover                   To recover data from an image file
@@ -175,56 +180,61 @@
     $ stegolsb steglsb -a -i input_image.png -s input_file.zip -n 2
     # OR
     $ stegolsb steglsb -h -i input_image.png -s input_file.zip -o steg.png -n 2 -c 1
     # OR
     $ stegolsb steglsb -r -i steg.png -o output_file.zip -n 2
 
 ### Analyzing
-Before hiding data in an image, it can useful to see how much data can be
+
+Before hiding data in an image, it can be useful to see how much data can be
 hidden. The following command will achieve this, producing output similar to
 
     $ stegolsb steglsb -a -i input_image.png -s input_file.zip -n 2
-    Image resolution: (2000, 1100)
+    Image resolution: (2000, 1100, 3)
     Using 2 LSBs, we can hide:     1650000 B
     Size of input file:            1566763 B
     File size tag:                 3 B
 
 ### Hiding Data
+
 The following command will hide data in the input image and write the result to
 the steganographed image, producing output similar to
 
     $ stegolsb steglsb -h -i input_image.png -s input_file.zip -o steg.png -n 2 -c 1
     Files read                     in 0.26s
     1566763 bytes hidden           in 0.31s
     Image overwritten              in 0.27s
 
 ### Recovering Data
+
 The following command will recover data from the steganographed image and write
 the result to the output file, producing output similar to
 
     $ stegolsb steglsb -r -i steg.png -o output_file.zip -n 2
     Files read                     in 0.30s
     1566763 bytes recovered        in 0.28s
     Output file written            in 0.00s
 
-<a name = "StegDetect"></a>
 ## StegDetect
+
 StegDetect provides one method for detecting simple steganography in images.
 
 ### How to Use
+
 You need Python 3 and Pillow, a fork of the Python Imaging Library (PIL).
 
 Run StegDetect with the following command line arguments:
 
     Command Line Arguments:
      -i, --input TEXT         Path to an image
      -n, --lsb-count INTEGER  How many LSBs to display  [default: 2]
      --help                   Show this message and exit.
 
 ### Showing the Least Significant Bits of an Image
+
 We sum the least significant n bits of the RGB color channels for each pixel
 and normalize the result to the range 0-255. This value is then applied to each
 color channel for the pixel. Where n is the number of least significant bits to
 show, the following command will save the resulting image, appending "_nLSBs"
 to the file name, and will produce output similar to the following:
 
     $ stegolsb stegdetect -i input_image.png -n 2
```

### Comparing `stego-lsb-1.4.4/tests/test_bit_manipulation.py` & `stego-lsb-1.5.0/tests/test_bit_manipulation.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,48 +1,34 @@
 from stego_lsb.bit_manipulation import lsb_interleave_bytes, lsb_deinterleave_bytes
 import numpy as np
 import unittest
 
 
 class TestBitManipulation(unittest.TestCase):
-    def assertConsistentInterleaving(
-        self, carrier: bytes, payload: bytes, num_lsb: int, byte_depth: int = 1
-    ) -> None:
+    def assertConsistentInterleaving(self, carrier: bytes, payload: bytes, num_lsb: int, byte_depth: int = 1) -> None:
         num_payload_bits = 8 * len(payload)
 
         encoded = lsb_interleave_bytes(carrier, payload, num_lsb, byte_depth=byte_depth)
-        decoded = lsb_deinterleave_bytes(
-            encoded, num_payload_bits, num_lsb, byte_depth=byte_depth
-        )
+        decoded = lsb_deinterleave_bytes(encoded, num_payload_bits, num_lsb, byte_depth=byte_depth)
         self.assertEqual(decoded, payload)  # payload correctly decoded
-        self.assertEqual(
-            len(encoded), len(carrier)
-        )  # message length is unchanged after interleaving
-
-        truncated_encode = lsb_interleave_bytes(
-            carrier, payload, num_lsb, byte_depth=byte_depth, truncate=True
-        )
-        truncated_decode = lsb_deinterleave_bytes(
-            truncated_encode, num_payload_bits, num_lsb, byte_depth=byte_depth
-        )
+        self.assertEqual(len(encoded), len(carrier))  # message length is unchanged after interleaving
+
+        truncated_encode = lsb_interleave_bytes(carrier, payload, num_lsb, byte_depth=byte_depth, truncate=True)
+        truncated_decode = lsb_deinterleave_bytes(truncated_encode, num_payload_bits, num_lsb, byte_depth=byte_depth)
         self.assertEqual(truncated_decode, payload)
 
-    def check_random_interleaving(
-        self, byte_depth: int = 1, num_trials: int = 1024
-    ) -> None:
+    def check_random_interleaving(self, byte_depth: int = 1, num_trials: int = 1024) -> None:
         np.random.seed(0)
         for _ in range(num_trials):
             carrier_len = np.random.randint(1, 16384)
             num_lsb = np.random.randint(1, 8 * byte_depth + 1)
             payload_len = carrier_len * num_lsb // (8 * byte_depth)
             carrier = np.random.randint(0, 256, size=carrier_len).tobytes()
             payload = np.random.randint(0, 256, size=payload_len).tobytes()
-            self.assertConsistentInterleaving(
-                carrier, payload, num_lsb, byte_depth=byte_depth
-            )
+            self.assertConsistentInterleaving(carrier, payload, num_lsb, byte_depth=byte_depth)
 
     def test_interleaving_consistency_8bit(self) -> None:
         self.check_random_interleaving(byte_depth=1)
 
     def test_interleaving_consistency_16bit(self) -> None:
         self.check_random_interleaving(byte_depth=2)
```

### Comparing `stego-lsb-1.4.4/tests/test_wavsteg.py` & `stego-lsb-1.5.0/tests/test_wavsteg.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,94 +5,68 @@
 import string
 from typing import Any, Type
 import unittest
 import wave
 
 
 class TestWavSteg(unittest.TestCase):
-    def write_random_wav(
-        self,
-        filename: str,
-        num_channels: int,
-        sample_width: int,
-        framerate: int,
-        num_frames: int,
-    ) -> None:
+    def write_random_wav(self, filename: str, num_channels: int, sample_width: int, framerate: int,
+                         num_frames: int) -> None:
         if sample_width != 1 and sample_width != 2:
             # WavSteg doesn't support higher sample widths
             raise ValueError("File has an unsupported bit-depth")
 
-        file = wave.open(filename, "w")
-        file.setnchannels(num_channels)
-        file.setsampwidth(sample_width)
-        file.setframerate(framerate)
-
-        dtype: Type[np.unsignedinteger[Any]]
-        if sample_width == 1:
-            dtype = np.uint8
-        else:
-            dtype = np.uint16
-
-        data = np.random.randint(
-            0, 2 ** (8 * sample_width), dtype=dtype, size=num_frames * num_channels
-        )
-        # note: typing does not recognize that "writeframes() accepts any bytes-like object" (see documentation)
-        file.writeframes(data)  # type: ignore
+        with wave.open(filename, "w") as file:
+            file.setnchannels(num_channels)
+            file.setsampwidth(sample_width)
+            file.setframerate(framerate)
+
+            dtype: Type[np.unsignedinteger[Any]]
+            if sample_width == 1:
+                dtype = np.uint8
+            else:
+                dtype = np.uint16
+
+            data = np.random.randint(0, 2 ** (8 * sample_width), dtype=dtype, size=num_frames * num_channels)
+            # note: typing does not recognize that "writeframes() accepts any bytes-like object" (see documentation)
+            file.writeframes(data)  # type: ignore
 
     def write_random_file(self, filename: str, num_bytes: int) -> None:
         with open(filename, "wb") as file:
             file.write(os.urandom(num_bytes))
 
-    def check_random_interleaving(
-        self, byte_depth: int = 1, num_trials: int = 256, filename_length: int = 5
-    ) -> None:
-        filename = "".join(
-            choice(string.ascii_lowercase) for _ in range(filename_length)
-        )
-        wav_input_filename = filename + ".wav"
-        payload_input_filename = filename + ".txt"
-        wav_output_filename = filename + "_steg.wav"
-        payload_output_filename = filename + "_recovered.txt"
+    def check_random_interleaving(self, byte_depth: int = 1, num_trials: int = 256, filename_length: int = 5) -> None:
+        filename = "".join(choice(string.ascii_lowercase) for _ in range(filename_length))
+        wav_input_filename = f"{filename}.wav"
+        payload_input_filename = f"{filename}.txt"
+        wav_output_filename = f"{filename}_steg.wav"
+        payload_output_filename = f"{filename}_recovered.txt"
 
         np.random.seed(0)
         for _ in range(num_trials):
             num_channels = np.random.randint(1, 64)
             num_frames = np.random.randint(1, 16384)
             num_lsb = np.random.randint(1, 8 * byte_depth + 1)
             payload_len = (num_frames * num_lsb * num_channels) // 8
 
-            self.write_random_wav(
-                wav_input_filename,
-                num_channels=num_channels,
-                sample_width=byte_depth,
-                framerate=44100,
-                num_frames=num_frames,
-            )
+            self.write_random_wav(wav_input_filename, num_channels=num_channels, sample_width=byte_depth,
+                                  framerate=44100, num_frames=num_frames)
             self.write_random_file(payload_input_filename, num_bytes=payload_len)
 
             try:
-                hide_data(
-                    wav_input_filename,
-                    payload_input_filename,
-                    wav_output_filename,
-                    num_lsb,
-                )
-                recover_data(
-                    wav_output_filename, payload_output_filename, num_lsb, payload_len
-                )
+                hide_data(wav_input_filename, payload_input_filename, wav_output_filename, num_lsb)
+                recover_data(wav_output_filename, payload_output_filename, num_lsb, payload_len)
             except ValueError as e:
                 os.remove(wav_input_filename)
                 os.remove(payload_input_filename)
                 os.remove(wav_output_filename)
                 os.remove(payload_output_filename)
                 raise e
 
-            with open(payload_input_filename, "rb") as input_file, open(
-                payload_output_filename, "rb"
-            ) as output_file:
+            with open(payload_input_filename, "rb") as input_file, open(payload_output_filename, "rb") as output_file:
                 input_payload_data = input_file.read()
                 output_payload_data = output_file.read()
 
             os.remove(wav_input_filename)
             os.remove(payload_input_filename)
             os.remove(wav_output_filename)
             os.remove(payload_output_filename)
```

