# Comparing `tmp/anicli_api-0.4.5.tar.gz` & `tmp/anicli_api-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anicli_api-0.4.5.tar", max compression
+gzip compressed data, was "anicli_api-0.4.7.tar", max compression
```

## Comparing `anicli_api-0.4.5.tar` & `anicli_api-0.4.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     4216 2023-05-15 08:36:21.974286 anicli_api-0.4.5/README.MD
--rw-r--r--   0        0        0     2940 2023-07-14 17:47:29.562755 anicli_api-0.4.5/anicli_api/_http.py
--rw-r--r--   0        0        0     1511 2023-05-15 08:36:21.974286 anicli_api-0.4.5/anicli_api/_logger.py
--rw-r--r--   0        0        0     3337 2023-07-17 14:57:08.210234 anicli_api-0.4.5/anicli_api/base.py
--rw-r--r--   0        0        0      615 2023-05-15 08:38:52.517152 anicli_api-0.4.5/anicli_api/player/__init__.py
--rw-r--r--   0        0        0      921 2023-07-14 17:47:29.562755 anicli_api-0.4.5/anicli_api/player/__template__.py
--rw-r--r--   0        0        0     2147 2023-07-14 17:47:29.562755 anicli_api-0.4.5/anicli_api/player/aniboom.py
--rw-r--r--   0        0        0     1055 2023-07-14 17:47:29.562755 anicli_api-0.4.5/anicli_api/player/animejoy.py
--rw-r--r--   0        0        0     3434 2023-07-14 17:47:29.562755 anicli_api-0.4.5/anicli_api/player/base.py
--rw-r--r--   0        0        0     1198 2023-07-14 17:47:29.562755 anicli_api-0.4.5/anicli_api/player/csst.py
--rw-r--r--   0        0        0     1456 2023-07-14 17:47:29.562755 anicli_api-0.4.5/anicli_api/player/dzen.py
--rw-r--r--   0        0        0     4047 2023-07-17 10:02:25.493422 anicli_api-0.4.5/anicli_api/player/kodik.py
--rw-r--r--   0        0        0     1837 2023-07-14 17:47:29.562755 anicli_api-0.4.5/anicli_api/player/mailru.py
--rw-r--r--   0        0        0     1697 2023-07-14 17:47:29.562755 anicli_api-0.4.5/anicli_api/player/okru.py
--rw-r--r--   0        0        0     1106 2023-07-14 17:47:29.562755 anicli_api-0.4.5/anicli_api/player/sibnet.py
--rw-r--r--   0        0        0     1139 2023-07-14 17:47:29.562755 anicli_api-0.4.5/anicli_api/player/sovetromantica.py
--rw-r--r--   0        0        0     1527 2023-07-14 17:47:29.562755 anicli_api-0.4.5/anicli_api/player/vkcom.py
--rw-r--r--   0        0        0        0 2023-05-15 08:38:52.517152 anicli_api-0.4.5/anicli_api/source/__init__.py
--rw-r--r--   0        0        0     2516 2023-07-14 17:47:29.562755 anicli_api-0.4.5/anicli_api/source/__template__.py
--rw-r--r--   0        0        0     6163 2023-07-14 17:47:29.562755 anicli_api-0.4.5/anicli_api/source/anilibria.py
--rw-r--r--   0        0        0    10795 2023-07-17 15:00:57.999414 anicli_api-0.4.5/anicli_api/source/animego.py
--rw-r--r--   0        0        0     8722 2023-07-14 17:47:29.562755 anicli_api-0.4.5/anicli_api/source/animejoy.py
--rw-r--r--   0        0        0     5543 2023-07-14 17:47:29.562755 anicli_api-0.4.5/anicli_api/source/animevost.py
--rw-r--r--   0        0        0     6462 2023-07-14 17:47:29.562755 anicli_api-0.4.5/anicli_api/source/sovetromantica.py
--rw-r--r--   0        0        0       58 2023-05-15 08:36:21.974286 anicli_api-0.4.5/anicli_api/tools/__init__.py
--rw-r--r--   0        0        0     2704 2022-12-17 13:02:20.525429 anicli_api-0.4.5/anicli_api/tools/random_useragent.py
--rw-r--r--   0        0        0      198 2023-07-14 17:47:29.562755 anicli_api-0.4.5/anicli_api/tools/utils.py
--rw-r--r--   0        0        0     2342 2023-07-17 15:02:45.656349 anicli_api-0.4.5/pyproject.toml
--rw-r--r--   0        0        0     5483 1970-01-01 00:00:00.000000 anicli_api-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     4216 2023-05-14 13:35:05.718934 anicli_api-0.4.7/README.MD
+-rw-r--r--   0        0        0     2940 2023-07-18 11:11:13.119093 anicli_api-0.4.7/anicli_api/_http.py
+-rw-r--r--   0        0        0     1511 2023-05-14 13:35:05.718934 anicli_api-0.4.7/anicli_api/_logger.py
+-rw-r--r--   0        0        0     3367 2023-07-18 11:11:13.119093 anicli_api-0.4.7/anicli_api/base.py
+-rw-r--r--   0        0        0      615 2023-07-18 11:11:13.120093 anicli_api-0.4.7/anicli_api/player/__init__.py
+-rw-r--r--   0        0        0      921 2023-07-18 11:11:13.120093 anicli_api-0.4.7/anicli_api/player/__template__.py
+-rw-r--r--   0        0        0     2147 2023-07-18 11:11:13.120093 anicli_api-0.4.7/anicli_api/player/aniboom.py
+-rw-r--r--   0        0        0     1055 2023-07-18 11:11:13.120093 anicli_api-0.4.7/anicli_api/player/animejoy.py
+-rw-r--r--   0        0        0     3434 2023-07-18 11:11:13.120093 anicli_api-0.4.7/anicli_api/player/base.py
+-rw-r--r--   0        0        0     1198 2023-07-18 11:11:13.120093 anicli_api-0.4.7/anicli_api/player/csst.py
+-rw-r--r--   0        0        0     1456 2023-07-18 11:11:13.120093 anicli_api-0.4.7/anicli_api/player/dzen.py
+-rw-r--r--   0        0        0     3999 2023-07-18 16:07:07.929504 anicli_api-0.4.7/anicli_api/player/kodik.py
+-rw-r--r--   0        0        0     1837 2023-07-18 11:11:13.120093 anicli_api-0.4.7/anicli_api/player/mailru.py
+-rw-r--r--   0        0        0     1697 2023-07-18 11:11:13.120093 anicli_api-0.4.7/anicli_api/player/okru.py
+-rw-r--r--   0        0        0     1106 2023-07-18 11:11:13.121093 anicli_api-0.4.7/anicli_api/player/sibnet.py
+-rw-r--r--   0        0        0     1139 2023-07-18 11:11:13.121093 anicli_api-0.4.7/anicli_api/player/sovetromantica.py
+-rw-r--r--   0        0        0     1527 2023-07-18 11:11:13.121093 anicli_api-0.4.7/anicli_api/player/vkcom.py
+-rw-r--r--   0        0        0        0 2023-07-18 11:11:13.121093 anicli_api-0.4.7/anicli_api/source/__init__.py
+-rw-r--r--   0        0        0     2516 2023-07-18 11:11:13.121093 anicli_api-0.4.7/anicli_api/source/__template__.py
+-rw-r--r--   0        0        0     6163 2023-07-18 11:11:13.121093 anicli_api-0.4.7/anicli_api/source/anilibria.py
+-rw-r--r--   0        0        0    10726 2023-07-18 11:11:13.121093 anicli_api-0.4.7/anicli_api/source/animego.py
+-rw-r--r--   0        0        0     8722 2023-07-18 11:11:13.122093 anicli_api-0.4.7/anicli_api/source/animejoy.py
+-rw-r--r--   0        0        0     5543 2023-07-18 11:11:13.122093 anicli_api-0.4.7/anicli_api/source/animevost.py
+-rw-r--r--   0        0        0     6462 2023-07-18 11:11:13.122093 anicli_api-0.4.7/anicli_api/source/sovetromantica.py
+-rw-r--r--   0        0        0       58 2023-01-25 23:19:25.549656 anicli_api-0.4.7/anicli_api/tools/__init__.py
+-rw-r--r--   0        0        0     2704 2022-12-06 17:11:19.675846 anicli_api-0.4.7/anicli_api/tools/random_useragent.py
+-rw-r--r--   0        0        0      198 2023-07-18 11:11:13.122093 anicli_api-0.4.7/anicli_api/tools/utils.py
+-rw-r--r--   0        0        0     2342 2023-07-18 16:13:25.771718 anicli_api-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0     5483 1970-01-01 00:00:00.000000 anicli_api-0.4.7/PKG-INFO
```

### Comparing `anicli_api-0.4.5/README.MD` & `anicli_api-0.4.7/README.MD`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.5/anicli_api/_http.py` & `anicli_api-0.4.7/anicli_api/_http.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.5/anicli_api/_logger.py` & `anicli_api-0.4.7/anicli_api/_logger.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.5/anicli_api/base.py` & `anicli_api-0.4.7/anicli_api/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import warnings
 from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, List, Optional, ClassVar, Type
+from typing import TYPE_CHECKING, ClassVar, List, Optional, Type
 
 from parsel import Selector
 from scrape_schema import BaseSchema
 
 from anicli_api._http import HTTPAsync, HTTPSync
 from anicli_api.player import ALL_DECODERS
 
@@ -107,14 +107,15 @@
     async def a_get_sources(self):
         pass
 
 
 class BaseSource(MainSchema):
     ALL_VIDEO_EXTRACTORS = ALL_DECODERS
     url: str = NotImplemented
+    dub: str = NotImplemented
 
     def _pre_validate_url_attr(self) -> None:
         if self.url is NotImplemented:
             raise AttributeError(f"{self.__class__.__name__} missing url attribute.")
 
     def get_videos(self) -> List["Video"]:
         self._pre_validate_url_attr()
```

### Comparing `anicli_api-0.4.5/anicli_api/player/__init__.py` & `anicli_api-0.4.7/anicli_api/player/__init__.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.5/anicli_api/player/__template__.py` & `anicli_api-0.4.7/anicli_api/player/__template__.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.5/anicli_api/player/aniboom.py` & `anicli_api-0.4.7/anicli_api/player/aniboom.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.5/anicli_api/player/animejoy.py` & `anicli_api-0.4.7/anicli_api/player/animejoy.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.5/anicli_api/player/base.py` & `anicli_api-0.4.7/anicli_api/player/base.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.5/anicli_api/player/csst.py` & `anicli_api-0.4.7/anicli_api/player/csst.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.5/anicli_api/player/dzen.py` & `anicli_api-0.4.7/anicli_api/player/dzen.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.5/anicli_api/player/kodik.py` & `anicli_api-0.4.7/anicli_api/player/kodik.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,19 +42,15 @@
                 (ord(e.group(0)) + 13 - (65 if e.group(0) <= "Z" else 97)) % 26 + (65 if e.group(0) <= "Z" else 97)
             )
 
         base64_url = re.sub(r"[a-zA-Z]", char_wrapper, url_encoded)
         if not base64_url.endswith("=="):
             base64_url += "=="
         decoded_url = b64decode(base64_url).decode()
-        return (
-            decoded_url
-            if decoded_url.startswith("https")
-            else f"https:{b64decode(base64_url).decode()}"
-        )
+        return decoded_url if decoded_url.startswith("https") else f"https:{b64decode(base64_url).decode()}"
 
     @kodik_validator
     def parse(self, url: str, **kwargs) -> List[Video]:
         response = self.http.get(url).text
         payload = _KodikPayload(response).dict()
         url_api = f"https://{urlsplit(url).netloc}/gvi"
         response_api = self.http.post(
@@ -91,14 +87,14 @@
         return [
             Video(type="m3u8", quality=360, url=self._decode(response_api["360"][0]["src"])),
             Video(type="m3u8", quality=480, url=self._decode(response_api["480"][0]["src"])),
             # maybe return only 360, 480 keys
             Video(
                 type="m3u8",
                 quality=720,
-                url=self._decode(response_api["480"][0]["src"]).replace("360.mp4", "720.mp4"),
+                url=self._decode(response_api["480"][0]["src"]).replace("480.mp4", "720.mp4"),
             ),
         ]
 
 
 if __name__ == "__main__":
     Kodik().parse("https://kodik.info/seria/1133512/04d5f7824ba3563bd78e44a22451bb45/720p")
```

### Comparing `anicli_api-0.4.5/anicli_api/player/mailru.py` & `anicli_api-0.4.7/anicli_api/player/mailru.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.5/anicli_api/player/okru.py` & `anicli_api-0.4.7/anicli_api/player/okru.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.5/anicli_api/player/sibnet.py` & `anicli_api-0.4.7/anicli_api/player/sibnet.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.5/anicli_api/player/sovetromantica.py` & `anicli_api-0.4.7/anicli_api/player/sovetromantica.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.5/anicli_api/player/vkcom.py` & `anicli_api-0.4.7/anicli_api/player/vkcom.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.5/anicli_api/source/__template__.py` & `anicli_api-0.4.7/anicli_api/source/__template__.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.5/anicli_api/source/anilibria.py` & `anicli_api-0.4.7/anicli_api/source/anilibria.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.5/anicli_api/source/animego.py` & `anicli_api-0.4.7/anicli_api/source/animego.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,19 +169,21 @@
 
     @staticmethod
     def _get_dubbers(response: str) -> Dict[str, str]:
         # sel = Selector(response)
         dubbers_id: List[str] = (
             Parsel().xpath('//*[@id="video-dubbing"]/span/@data-dubbing').getall().sc_parse(response)
         )
-        dubbers_name: List[str] = (Parsel()
-                                   .xpath('//*[@id="video-dubbing"]/span/span/text()')
-                                   .getall()
-                                   .fn(lambda lst: [s.strip() for s in lst])
-                                   .sc_parse(response))
+        dubbers_name: List[str] = (
+            Parsel()
+            .xpath('//*[@id="video-dubbing"]/span/span/text()')
+            .getall()
+            .fn(lambda lst: [s.strip() for s in lst])
+            .sc_parse(response)
+        )
         return dict(zip(dubbers_id, dubbers_name))
 
     def get_episodes(self) -> List["Episode"]:
         response = self.HTTP().get(f"https://animego.org/anime/{self.anime_id}/player?_allow=true").json()["content"]
 
         _dubbers_table = self._get_dubbers(response)
         chunks = Parsel().xpath('//*[@id="video-carousel"]/div/div').getall().sc_parse(response)
@@ -199,15 +201,15 @@
             for ep in episodes:
                 setattr(ep, "_dubbers_table", _dubbers_table)
             return episodes
 
 
 class Episode(BaseEpisode):
     _episode_type: Sc[int, Parsel().xpath("//div/@data-episode-type").get()]
-    _dubbers_table: Dict[str, str] # setattr
+    _dubbers_table: Dict[str, str]  # setattr
     num: Sc[int, Parsel().xpath("//div/@data-episode").get()]
     title: Sc[str, Parsel().xpath("//div/@data-episode-title").get()]
 
     data_id: Sc[int, Parsel().xpath("//div/@data-id").get()]
     released: Sc[str, Parsel().xpath("//div/@data-episode-released").get()]
 
     def __str__(self):
```

### Comparing `anicli_api-0.4.5/anicli_api/source/animejoy.py` & `anicli_api-0.4.7/anicli_api/source/animejoy.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.5/anicli_api/source/animevost.py` & `anicli_api-0.4.7/anicli_api/source/animevost.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.5/anicli_api/source/sovetromantica.py` & `anicli_api-0.4.7/anicli_api/source/sovetromantica.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.5/anicli_api/tools/random_useragent.py` & `anicli_api-0.4.7/anicli_api/tools/random_useragent.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.5/pyproject.toml` & `anicli_api-0.4.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anicli_api"
-version = "0.4.5"
+version = "0.4.7"
 description = "Anime extractor api implementation"
 authors = ["Georgiy aka Vypivshiy"]
 license = "MIT"
 readme = "README.MD"
 packages = [{include = "anicli_api"}]
 exclude = ["tests/"]
 keywords = [
```

### Comparing `anicli_api-0.4.5/PKG-INFO` & `anicli_api-0.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anicli-api
-Version: 0.4.5
+Version: 0.4.7
 Summary: Anime extractor api implementation
 License: MIT
 Keywords: anime,api,ru,russia,asyncio,parser,httpx,dev
 Author: Georgiy aka Vypivshiy
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

