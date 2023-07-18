# Comparing `tmp/pywa-0.0.1rc24-py3-none-any.whl.zip` & `tmp/pywa-0.0.1rc25-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 33022 bytes, number of entries: 21
+Zip file size: 33023 bytes, number of entries: 21
 -rw-r--r--  2.0 unx      117 b- defN 23-Jul-13 18:15 pywa/__init__.py
--rw-r--r--  2.0 unx       26 b- defN 23-Jul-16 20:36 pywa/__version__.py
+-rw-r--r--  2.0 unx       26 b- defN 23-Jul-18 07:44 pywa/__version__.py
 -rw-r--r--  2.0 unx    14220 b- defN 23-Jul-13 18:15 pywa/api.py
--rw-r--r--  2.0 unx    29401 b- defN 23-Jul-13 18:15 pywa/client.py
+-rw-r--r--  2.0 unx    29404 b- defN 23-Jul-18 07:44 pywa/client.py
 -rw-r--r--  2.0 unx     7191 b- defN 23-Jul-13 18:15 pywa/errors.py
 -rw-r--r--  2.0 unx    21625 b- defN 23-Jul-16 20:52 pywa/filters.py
 -rw-r--r--  2.0 unx     3846 b- defN 23-Jul-13 18:15 pywa/handlers.py
 -rw-r--r--  2.0 unx      873 b- defN 23-Jul-13 18:15 pywa/utils.py
 -rw-r--r--  2.0 unx     4600 b- defN 23-Jul-13 18:15 pywa/webhook.py
 -rw-r--r--  2.0 unx      336 b- defN 23-Jul-13 18:15 pywa/types/__init__.py
 -rw-r--r--  2.0 unx     8951 b- defN 23-Jul-13 18:15 pywa/types/base_update.py
 -rw-r--r--  2.0 unx     5523 b- defN 23-Jul-13 18:30 pywa/types/callback.py
 -rw-r--r--  2.0 unx     4609 b- defN 23-Jul-13 18:15 pywa/types/media.py
 -rw-r--r--  2.0 unx    11234 b- defN 23-Jul-13 18:15 pywa/types/message.py
 -rw-r--r--  2.0 unx     1934 b- defN 23-Jul-13 18:15 pywa/types/message_status.py
 -rw-r--r--  2.0 unx     9156 b- defN 23-Jul-13 18:15 pywa/types/others.py
--rw-r--r--  2.0 unx     1066 b- defN 23-Jul-16 21:10 pywa-0.0.1rc24.dist-info/LICENSE
--rw-r--r--  2.0 unx     4420 b- defN 23-Jul-16 21:10 pywa-0.0.1rc24.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-16 21:10 pywa-0.0.1rc24.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Jul-16 21:10 pywa-0.0.1rc24.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1591 b- defN 23-Jul-16 21:10 pywa-0.0.1rc24.dist-info/RECORD
-21 files, 130816 bytes uncompressed, 30496 bytes compressed:  76.7%
+-rw-r--r--  2.0 unx     1066 b- defN 23-Jul-18 07:44 pywa-0.0.1rc25.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4420 b- defN 23-Jul-18 07:44 pywa-0.0.1rc25.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-18 07:44 pywa-0.0.1rc25.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Jul-18 07:44 pywa-0.0.1rc25.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1591 b- defN 23-Jul-18 07:44 pywa-0.0.1rc25.dist-info/RECORD
+21 files, 130819 bytes uncompressed, 30497 bytes compressed:  76.7%
```

## zipnote {}

```diff
@@ -42,23 +42,23 @@
 
 Filename: pywa/types/message_status.py
 Comment: 
 
 Filename: pywa/types/others.py
 Comment: 
 
-Filename: pywa-0.0.1rc24.dist-info/LICENSE
+Filename: pywa-0.0.1rc25.dist-info/LICENSE
 Comment: 
 
-Filename: pywa-0.0.1rc24.dist-info/METADATA
+Filename: pywa-0.0.1rc25.dist-info/METADATA
 Comment: 
 
-Filename: pywa-0.0.1rc24.dist-info/WHEEL
+Filename: pywa-0.0.1rc25.dist-info/WHEEL
 Comment: 
 
-Filename: pywa-0.0.1rc24.dist-info/top_level.txt
+Filename: pywa-0.0.1rc25.dist-info/top_level.txt
 Comment: 
 
-Filename: pywa-0.0.1rc24.dist-info/RECORD
+Filename: pywa-0.0.1rc25.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pywa/__version__.py

```diff
@@ -1 +1 @@
-__version__ = "0.0.1rc24"
+__version__ = "0.0.1rc25"
```

## pywa/client.py

```diff
@@ -306,16 +306,16 @@
             if media.startswith(("https://", "http://")):
                 return True, media
             elif not os.path.isfile(media) and media.isdigit():
                 return False, media  # assume it's a media ID
             else:
                 return False, self.upload_media(
                     media=media,
-                    mime_type=mimetypes.guess_type(media)[0] or mime_type,
-                    file_name=os.path.basename(media) or file_name
+                    mime_type=mime_type or mimetypes.guess_type(media)[0],
+                    file_name=file_name or os.path.basename(media)
                 )
         else:
             return False, self.api.upload_media(media=media, mime_type=mime_type, file_name=file_name)['id']
 
     def send_image(
             self,
             to: str,
@@ -715,26 +715,26 @@
 
         Returns:
             The media ID.
         """
         if isinstance(media, str):
             if os.path.isfile(media):
                 file, file_name, mime_type = \
-                    open(media, 'rb'), os.path.basename(media), (mimetypes.guess_type(media)[0] or mime_type)
+                    open(media, 'rb'), file_name or os.path.basename(media), (mimetypes.guess_type(media)[0] or mime_type)
             elif media.startswith(("https://", "http://")):
                 res = requests.get(media)
                 res.raise_for_status()
                 file, file_name, mime_type = \
-                    res.content, os.path.basename(media) or file_name, (res.headers['Content-Type'] or mime_type)
+                    res.content, file_name or os.path.basename(media), (res.headers['Content-Type'] or mime_type)
             else:
                 raise ValueError(f'File not found or invalid URL: {media}')
         else:
             file = media
         return self.api.upload_media(
-            file_name=file_name or 'file',
+            file_name=file_name,
             media=file,
             mime_type=mime_type,
         )['id']
 
     def get_media_url(
             self,
             media_id: str
```

## Comparing `pywa-0.0.1rc24.dist-info/LICENSE` & `pywa-0.0.1rc25.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pywa-0.0.1rc24.dist-info/METADATA` & `pywa-0.0.1rc25.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywa
-Version: 0.0.1rc24
+Version: 0.0.1rc25
 Summary: Python wrapper for the WhatsApp Cloud API
 Download-URL: https://pypi.org/project/pywa/
 Author: David Lev
 Author-email: davidlev@telegmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/david-lev/pywa#readme
 Project-URL: Issue Tracker, https://github.com/david-lev/pywa/issues
```

## Comparing `pywa-0.0.1rc24.dist-info/RECORD` & `pywa-0.0.1rc25.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 pywa/__init__.py,sha256=u98CpT0wYk8-XDPUGB_hW-a_23agBkzTSzfwmoqnsE0,117
-pywa/__version__.py,sha256=agXX6xC2qTdAJxv32RKAtdPJSGbsCvJqRcLqSuryx6M,26
+pywa/__version__.py,sha256=5gQSLTod6G3Z8H3mwpS8LFLnj9D9ncyBS5YQKpKJdEQ,26
 pywa/api.py,sha256=xiFBJ-PHNkzN-3HFUXE0YO4xwgTWPDI1PSbafpmRuF0,14220
-pywa/client.py,sha256=wZLrY-weLF1qeOVzmXAZ7M0mONm8yP3yWVuoRjSxkzc,29401
+pywa/client.py,sha256=1hDMBjhbekyGrriSq1eJB0p4F7DD7ND-U-Syq1wfGT0,29404
 pywa/errors.py,sha256=ErB0UGIpIOF5vZXK39WmiSrB_PSYvTJL8PLIp90vTjU,7191
 pywa/filters.py,sha256=0pNYHsoH2hv2q9YN3Px-aTRq4Jdff5O6tVa83GHEZCw,21625
 pywa/handlers.py,sha256=VD3Z3gocBbxRoHXscBkaP8SONt-M9CDVaiL8duWiL9w,3846
 pywa/utils.py,sha256=vIPGDuXFo80xAhv88mboE-rU-uDEv594cAxEPsMrIZg,873
 pywa/webhook.py,sha256=1IjiwZTYSh5RvRI-DTa2qajVg-tqBQepm_dcHO9rogo,4600
 pywa/types/__init__.py,sha256=HwhabvWT9b1bgPLnvXBDOmYNTh-FYjCC-ot-rh8xqzo,336
 pywa/types/base_update.py,sha256=EW5Fl6rWyCfnIzOQVz7PfCvPzDAnvXlVlqqZh-w4w3c,8951
 pywa/types/callback.py,sha256=rTNO6XTsXXnEq0_19lqWNVxMEYu3FjRkl9pAN6tGvHc,5523
 pywa/types/media.py,sha256=4T5yOsoZwFmJaTUZf49VnMsXACsGLq1crC6wzSBqanA,4609
 pywa/types/message.py,sha256=zNKvifHA3P89TOxKoV4dLnt-B9jbu7whlP8gdu304Xo,11234
 pywa/types/message_status.py,sha256=wgUlrgTCaKKqEZgVaZt_yYY_PKyJMhBGz-Rh3WaXSB0,1934
 pywa/types/others.py,sha256=UeXSWEY1pekZDVBDacbUsXff_OmYbxbAe9P2o_am4es,9156
-pywa-0.0.1rc24.dist-info/LICENSE,sha256=RwljuP8WgWttLkSivccHoHEFSDhOY8aLM_vg6Ix48yQ,1066
-pywa-0.0.1rc24.dist-info/METADATA,sha256=PPaghzwPm1JNAhUGXtzfBGqu2QYQlqKvpiTXJ1OkcVc,4420
-pywa-0.0.1rc24.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-pywa-0.0.1rc24.dist-info/top_level.txt,sha256=Cl24ggXVvxvOUnQfKRASer1LzHxpYCPZd5ZcVyS98Oo,5
-pywa-0.0.1rc24.dist-info/RECORD,,
+pywa-0.0.1rc25.dist-info/LICENSE,sha256=RwljuP8WgWttLkSivccHoHEFSDhOY8aLM_vg6Ix48yQ,1066
+pywa-0.0.1rc25.dist-info/METADATA,sha256=1dBS3zsb5D3AUN4HIFDhZyA8j-L5jWnE1bYstRl05Ro,4420
+pywa-0.0.1rc25.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+pywa-0.0.1rc25.dist-info/top_level.txt,sha256=Cl24ggXVvxvOUnQfKRASer1LzHxpYCPZd5ZcVyS98Oo,5
+pywa-0.0.1rc25.dist-info/RECORD,,
```

