# Comparing `tmp/tnzapi-2.2.0.0.tar.gz` & `tmp/tnzapi-2.3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tnzapi-2.2.0.0.tar", last modified: Mon Jul 18 05:01:09 2022, max compression
+gzip compressed data, was "tnzapi-2.3.0.0.tar", last modified: Tue Jul 18 04:31:59 2023, max compression
```

## Comparing `tnzapi-2.2.0.0.tar` & `tnzapi-2.3.0.0.tar`

### file list

```diff
@@ -1,53 +1,19 @@
-drwxrwxrwx   0        0        0        0 2022-07-18 05:01:09.273495 tnzapi-2.2.0.0/
--rw-rw-rw-   0        0        0     4976 2022-07-18 05:01:09.274472 tnzapi-2.2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3046 2022-07-15 04:25:07.000000 tnzapi-2.2.0.0/README.md
--rw-rw-rw-   0        0        0       86 2022-07-18 05:01:09.279318 tnzapi-2.2.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1179 2021-11-10 23:40:05.000000 tnzapi-2.2.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-07-18 05:01:08.774726 tnzapi-2.2.0.0/tnzapi/
--rw-rw-rw-   0        0        0     1337 2022-07-14 04:44:01.000000 tnzapi-2.2.0.0/tnzapi/__init__.py
--rw-rw-rw-   0        0        0      346 2022-07-14 04:09:36.000000 tnzapi-2.2.0.0/tnzapi/_config.py
-drwxrwxrwx   0        0        0        0 2022-07-18 05:01:08.875288 tnzapi-2.2.0.0/tnzapi/base/
--rw-rw-rw-   0        0        0     1802 2021-07-05 02:25:54.000000 tnzapi-2.2.0.0/tnzapi/base/__init__.py
--rw-rw-rw-   0        0        0      733 2020-07-09 22:04:38.000000 tnzapi-2.2.0.0/tnzapi/base/functions.py
-drwxrwxrwx   0        0        0        0 2022-07-18 05:01:08.946536 tnzapi-2.2.0.0/tnzapi/base/get/
--rw-rw-rw-   0        0        0        0 2020-06-08 21:57:31.000000 tnzapi-2.2.0.0/tnzapi/base/get/__init__.py
--rw-rw-rw-   0        0        0     6190 2021-12-15 04:32:57.000000 tnzapi-2.2.0.0/tnzapi/base/get/result_request_result.py
--rw-rw-rw-   0        0        0     2441 2021-12-15 04:33:34.000000 tnzapi-2.2.0.0/tnzapi/base/get/sms_received_result.py
--rw-rw-rw-   0        0        0     4114 2021-12-15 04:33:50.000000 tnzapi-2.2.0.0/tnzapi/base/get/sms_reply_result.py
--rw-rw-rw-   0        0        0     4857 2021-12-15 04:34:01.000000 tnzapi-2.2.0.0/tnzapi/base/get/status_request_result.py
-drwxrwxrwx   0        0        0        0 2022-07-18 05:01:08.990422 tnzapi-2.2.0.0/tnzapi/base/send/
--rw-rw-rw-   0        0        0        0 2020-06-08 21:57:38.000000 tnzapi-2.2.0.0/tnzapi/base/send/__init__.py
--rw-rw-rw-   0        0        0     1506 2020-10-08 22:51:48.000000 tnzapi-2.2.0.0/tnzapi/base/send/keypad.py
--rw-rw-rw-   0        0        0     2270 2021-07-05 02:25:10.000000 tnzapi-2.2.0.0/tnzapi/base/send/message_result.py
-drwxrwxrwx   0        0        0        0 2022-07-18 05:01:09.007051 tnzapi-2.2.0.0/tnzapi/base/set/
--rw-rw-rw-   0        0        0        0 2020-06-08 21:57:46.000000 tnzapi-2.2.0.0/tnzapi/base/set/__init__.py
--rw-rw-rw-   0        0        0     2860 2021-07-05 02:25:39.000000 tnzapi-2.2.0.0/tnzapi/base/set/set_request_result.py
-drwxrwxrwx   0        0        0        0 2022-07-18 05:01:09.095863 tnzapi-2.2.0.0/tnzapi/get/
--rw-rw-rw-   0        0        0     1166 2021-08-13 00:34:56.000000 tnzapi-2.2.0.0/tnzapi/get/__init__.py
--rw-rw-rw-   0        0        0     1985 2022-07-14 04:52:13.000000 tnzapi-2.2.0.0/tnzapi/get/_common.py
--rw-rw-rw-   0        0        0     3099 2022-07-14 04:53:55.000000 tnzapi-2.2.0.0/tnzapi/get/result.py
--rw-rw-rw-   0        0        0     4020 2022-07-14 04:45:49.000000 tnzapi-2.2.0.0/tnzapi/get/sms_received.py
--rw-rw-rw-   0        0        0     3124 2022-07-14 04:54:25.000000 tnzapi-2.2.0.0/tnzapi/get/sms_reply.py
--rw-rw-rw-   0        0        0     3091 2022-07-14 04:55:08.000000 tnzapi-2.2.0.0/tnzapi/get/status.py
-drwxrwxrwx   0        0        0        0 2022-07-18 05:01:09.182729 tnzapi-2.2.0.0/tnzapi/send/
--rw-rw-rw-   0        0        0     1274 2021-08-13 00:35:19.000000 tnzapi-2.2.0.0/tnzapi/send/__init__.py
--rw-rw-rw-   0        0        0     6407 2022-07-14 04:52:08.000000 tnzapi-2.2.0.0/tnzapi/send/_common.py
--rw-rw-rw-   0        0        0     5922 2022-07-15 03:00:18.000000 tnzapi-2.2.0.0/tnzapi/send/email.py
--rw-rw-rw-   0        0        0     5902 2022-07-15 02:13:23.000000 tnzapi-2.2.0.0/tnzapi/send/fax.py
--rw-rw-rw-   0        0        0     5783 2022-07-15 02:14:31.000000 tnzapi-2.2.0.0/tnzapi/send/sms.py
--rw-rw-rw-   0        0        0     7565 2022-07-15 02:16:06.000000 tnzapi-2.2.0.0/tnzapi/send/tts.py
--rw-rw-rw-   0        0        0     9173 2022-07-15 02:18:36.000000 tnzapi-2.2.0.0/tnzapi/send/voice.py
-drwxrwxrwx   0        0        0        0 2022-07-18 05:01:09.262761 tnzapi-2.2.0.0/tnzapi/set/
--rw-rw-rw-   0        0        0     1138 2021-08-13 00:36:27.000000 tnzapi-2.2.0.0/tnzapi/set/__init__.py
--rw-rw-rw-   0        0        0     1985 2022-07-14 04:52:04.000000 tnzapi-2.2.0.0/tnzapi/set/_common.py
--rw-rw-rw-   0        0        0     3325 2022-07-15 02:48:15.000000 tnzapi-2.2.0.0/tnzapi/set/abort.py
--rw-rw-rw-   0        0        0     3851 2022-07-15 02:54:39.000000 tnzapi-2.2.0.0/tnzapi/set/pacing.py
--rw-rw-rw-   0        0        0     3843 2022-07-15 02:55:37.000000 tnzapi-2.2.0.0/tnzapi/set/reschedule.py
--rw-rw-rw-   0        0        0     3677 2022-07-15 02:58:53.000000 tnzapi-2.2.0.0/tnzapi/set/resubmit.py
-drwxrwxrwx   0        0        0        0 2022-07-18 05:01:08.845039 tnzapi-2.2.0.0/tnzapi.egg-info/
--rw-rw-rw-   0        0        0     4976 2022-07-18 05:01:07.000000 tnzapi-2.2.0.0/tnzapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1052 2022-07-18 05:01:08.000000 tnzapi-2.2.0.0/tnzapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-18 05:01:07.000000 tnzapi-2.2.0.0/tnzapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2020-12-16 00:34:38.000000 tnzapi-2.2.0.0/tnzapi.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2022-07-18 05:01:07.000000 tnzapi-2.2.0.0/tnzapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-07-18 05:01:07.000000 tnzapi-2.2.0.0/tnzapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 04:31:59.589582 tnzapi-2.3.0.0/
+-rw-rw-rw-   0        0        0    16322 2023-07-18 04:31:59.593975 tnzapi-2.3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10531 2023-07-17 23:52:59.000000 tnzapi-2.3.0.0/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-18 04:31:59.604353 tnzapi-2.3.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1231 2023-07-10 01:36:56.000000 tnzapi-2.3.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 04:31:59.441531 tnzapi-2.3.0.0/tnzapi/
+-rw-rw-rw-   0        0        0     2770 2023-07-18 04:27:57.000000 tnzapi-2.3.0.0/tnzapi/__init__.py
+-rw-rw-rw-   0        0        0      346 2023-07-07 00:22:17.000000 tnzapi-2.3.0.0/tnzapi/_config.py
+drwxrwxrwx   0        0        0        0 2023-07-18 04:31:59.569341 tnzapi-2.3.0.0/tnzapi/helpers/
+-rw-rw-rw-   0        0        0        0 2023-07-10 00:23:18.000000 tnzapi-2.3.0.0/tnzapi/helpers/__init__.py
+-rw-rw-rw-   0        0        0      133 2023-07-17 05:11:27.000000 tnzapi-2.3.0.0/tnzapi/helpers/custom_json_encoder.py
+-rw-rw-rw-   0        0        0     1299 2023-07-17 06:18:08.000000 tnzapi-2.3.0.0/tnzapi/helpers/functions.py
+drwxrwxrwx   0        0        0        0 2023-07-18 04:31:59.504567 tnzapi-2.3.0.0/tnzapi.egg-info/
+-rw-rw-rw-   0        0        0    16322 2023-07-18 04:31:58.000000 tnzapi-2.3.0.0/tnzapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2023-07-18 04:31:58.000000 tnzapi-2.3.0.0/tnzapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 04:31:58.000000 tnzapi-2.3.0.0/tnzapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2020-12-16 00:34:38.000000 tnzapi-2.3.0.0/tnzapi.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-07-18 04:31:58.000000 tnzapi-2.3.0.0/tnzapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-18 04:31:58.000000 tnzapi-2.3.0.0/tnzapi.egg-info/top_level.txt
```

### Comparing `tnzapi-2.2.0.0/setup.py` & `tnzapi-2.3.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 
 def readme():
     with open('README.md') as f:
         return f.read()
 
 setup(
     name='tnzapi',
-    version='2.2.0.0',
+    version='2.3.0.0',
     description='TNZ REST API Helper Library for Python',
     long_description=readme(),
     long_description_content_type='text/markdown',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         "Intended Audience :: Developers",
         'License :: OSI Approved :: MIT License',
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Communications :: Telephony",
         'Operating System :: OS Independent'
     ],
     url='https://www.tnz.co.nz',
     author='TNZ Group Limited',
     author_email='support@tnz.co.nz',
```

