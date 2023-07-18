# Comparing `tmp/automate_email-0.0.1.tar.gz` & `tmp/automate_email-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/xavierh/automate_email/dist/.tmp-84dlfyzl/automate_email-0.0.1.tar", last modified: Tue Jul 18 01:48:58 2023, max compression
+gzip compressed data, was "/Users/xavierh/automate_email/dist/.tmp-31fzjmqn/automate_email-0.0.2.tar", last modified: Tue Jul 18 02:24:08 2023, max compression
```

## Comparing `automate_email-0.0.1.tar` & `automate_email-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 xavierh    (501) staff       (20)        0 2023-07-18 01:48:58.110701 automate_email-0.0.1/
--rw-r--r--   0 xavierh    (501) staff       (20)     1070 2023-07-17 23:22:26.000000 automate_email-0.0.1/LICENSE
--rw-r--r--   0 xavierh    (501) staff       (20)      387 2023-07-18 01:48:58.110887 automate_email-0.0.1/PKG-INFO
-drwxr-xr-x   0 xavierh    (501) staff       (20)        0 2023-07-18 01:48:58.107101 automate_email-0.0.1/automate_email/
--rw-r--r--   0 xavierh    (501) staff       (20)     1292 2023-07-18 01:43:26.000000 automate_email-0.0.1/automate_email/__init__.py
-drwxr-xr-x   0 xavierh    (501) staff       (20)        0 2023-07-18 01:48:58.110201 automate_email-0.0.1/automate_email.egg-info/
--rw-r--r--   0 xavierh    (501) staff       (20)      387 2023-07-18 01:48:58.000000 automate_email-0.0.1/automate_email.egg-info/PKG-INFO
--rw-r--r--   0 xavierh    (501) staff       (20)      211 2023-07-18 01:48:58.000000 automate_email-0.0.1/automate_email.egg-info/SOURCES.txt
--rw-r--r--   0 xavierh    (501) staff       (20)        1 2023-07-18 01:48:58.000000 automate_email-0.0.1/automate_email.egg-info/dependency_links.txt
--rw-r--r--   0 xavierh    (501) staff       (20)       15 2023-07-18 01:48:58.000000 automate_email-0.0.1/automate_email.egg-info/top_level.txt
--rw-r--r--   0 xavierh    (501) staff       (20)       93 2023-07-18 00:39:07.000000 automate_email-0.0.1/pyproject.toml
--rw-r--r--   0 xavierh    (501) staff       (20)      454 2023-07-18 01:48:58.111708 automate_email-0.0.1/setup.cfg
+drwxr-xr-x   0 xavierh    (501) staff       (20)        0 2023-07-18 02:24:08.795406 automate_email-0.0.2/
+-rw-r--r--   0 xavierh    (501) staff       (20)     1070 2023-07-17 23:22:26.000000 automate_email-0.0.2/LICENSE
+-rw-r--r--   0 xavierh    (501) staff       (20)      387 2023-07-18 02:24:08.795547 automate_email-0.0.2/PKG-INFO
+drwxr-xr-x   0 xavierh    (501) staff       (20)        0 2023-07-18 02:24:08.792826 automate_email-0.0.2/automate_email/
+-rw-r--r--   0 xavierh    (501) staff       (20)     1339 2023-07-18 02:21:21.000000 automate_email-0.0.2/automate_email/__init__.py
+drwxr-xr-x   0 xavierh    (501) staff       (20)        0 2023-07-18 02:24:08.794861 automate_email-0.0.2/automate_email.egg-info/
+-rw-r--r--   0 xavierh    (501) staff       (20)      387 2023-07-18 02:24:08.000000 automate_email-0.0.2/automate_email.egg-info/PKG-INFO
+-rw-r--r--   0 xavierh    (501) staff       (20)      211 2023-07-18 02:24:08.000000 automate_email-0.0.2/automate_email.egg-info/SOURCES.txt
+-rw-r--r--   0 xavierh    (501) staff       (20)        1 2023-07-18 02:24:08.000000 automate_email-0.0.2/automate_email.egg-info/dependency_links.txt
+-rw-r--r--   0 xavierh    (501) staff       (20)       15 2023-07-18 02:24:08.000000 automate_email-0.0.2/automate_email.egg-info/top_level.txt
+-rw-r--r--   0 xavierh    (501) staff       (20)       93 2023-07-18 00:39:07.000000 automate_email-0.0.2/pyproject.toml
+-rw-r--r--   0 xavierh    (501) staff       (20)      454 2023-07-18 02:24:08.796160 automate_email-0.0.2/setup.cfg
```

### Comparing `automate_email-0.0.1/LICENSE` & `automate_email-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `automate_email-0.0.1/automate_email/__init__.py` & `automate_email-0.0.2/automate_email/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 import platform
 import win32com.client as win32
 outlook = win32.Dispatch('Outlook.Application') if platform.system() == "Windows" else Exception("This package is only compatible with Windows.")
+olNS = outlook.GetNamespace("MAPI")
 
 def is_internal(email: str) -> bool:
     """Returns true if email is internal, false otherwise."""
-    recipient = outlook.CreateRecipient(email)
+    recipient = olNS.createRecipient(email)
     recipient.Resolve()
     if recipient.Resolved:
         return True if recipient.AddressEntry == 0 else False
     else:
         raise Exception(f"Email {email} could not be resolved.")
 
 
@@ -18,10 +19,9 @@
     mail = outlook.CreateItem(0)
     mail.to = ';'.join(to)
     mail.cc = ';'.join(cc)
     mail.Importance = 2 if high_priority else 1
     mail.Subject = subject
     for attachment in attachments:
         mail.Attachments.Add(attachment)
-    mail.BodyFormat = 2 if use_HTML else 1
-    mail.body = body
+    mail.HTMLBody = f"<HTML><BODY>{body}</BODY></HTML>" if use_HTML else body
     mail.Send() if output == "SEND" else mail.Display() if output == "DISPLAY" else mail.Save() if output == "SAVE" else Exception(f"Invalid output option: {output}.")
```

