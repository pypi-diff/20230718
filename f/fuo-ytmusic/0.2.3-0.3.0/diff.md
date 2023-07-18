# Comparing `tmp/fuo-ytmusic-0.2.3.tar.gz` & `tmp/fuo-ytmusic-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuo-ytmusic-0.2.3.tar", last modified: Sat Jul 15 03:56:18 2023, max compression
+gzip compressed data, was "fuo-ytmusic-0.3.0.tar", last modified: Tue Jul 18 15:51:49 2023, max compression
```

## Comparing `fuo-ytmusic-0.2.3.tar` & `fuo-ytmusic-0.3.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 03:56:18.905745 fuo-ytmusic-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-15 03:56:17.000000 fuo-ytmusic-0.2.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-15 03:56:18.905745 fuo-ytmusic-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-15 03:56:17.000000 fuo-ytmusic-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 03:56:18.905745 fuo-ytmusic-0.2.3/fuo_ytmusic/
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-15 03:56:17.000000 fuo-ytmusic-0.2.3/fuo_ytmusic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 03:56:18.905745 fuo-ytmusic-0.2.3/fuo_ytmusic/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-15 03:56:17.000000 fuo-ytmusic-0.2.3/fuo_ytmusic/assets/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-15 03:56:17.000000 fuo-ytmusic-0.2.3/fuo_ytmusic/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-15 03:56:17.000000 fuo-ytmusic-0.2.3/fuo_ytmusic/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18244 2023-07-15 03:56:17.000000 fuo-ytmusic-0.2.3/fuo_ytmusic/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-07-15 03:56:17.000000 fuo-ytmusic-0.2.3/fuo_ytmusic/page_explore_qml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-15 03:56:17.000000 fuo-ytmusic-0.2.3/fuo_ytmusic/page_fav.py
--rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-07-15 03:56:17.000000 fuo-ytmusic-0.2.3/fuo_ytmusic/page_more.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-15 03:56:17.000000 fuo-ytmusic-0.2.3/fuo_ytmusic/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10642 2023-07-15 03:56:17.000000 fuo-ytmusic-0.2.3/fuo_ytmusic/provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 03:56:18.905745 fuo-ytmusic-0.2.3/fuo_ytmusic/qml/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 03:56:18.905745 fuo-ytmusic-0.2.3/fuo_ytmusic/qml/dummydata/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-15 03:56:17.000000 fuo-ytmusic-0.2.3/fuo_ytmusic/qml/dummydata/explore_backend.qml
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-07-15 03:56:17.000000 fuo-ytmusic-0.2.3/fuo_ytmusic/qml/page_explore.qml
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-15 03:56:17.000000 fuo-ytmusic-0.2.3/fuo_ytmusic/qml/uploader.qml
--rw-r--r--   0 runner    (1001) docker     (123)    13967 2023-07-15 03:56:17.000000 fuo-ytmusic-0.2.3/fuo_ytmusic/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-07-15 03:56:17.000000 fuo-ytmusic-0.2.3/fuo_ytmusic/timeparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-07-15 03:56:17.000000 fuo-ytmusic-0.2.3/fuo_ytmusic/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 03:56:18.905745 fuo-ytmusic-0.2.3/fuo_ytmusic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-15 03:56:18.000000 fuo-ytmusic-0.2.3/fuo_ytmusic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-15 03:56:18.000000 fuo-ytmusic-0.2.3/fuo_ytmusic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 03:56:18.000000 fuo-ytmusic-0.2.3/fuo_ytmusic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-15 03:56:18.000000 fuo-ytmusic-0.2.3/fuo_ytmusic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-15 03:56:18.000000 fuo-ytmusic-0.2.3/fuo_ytmusic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-15 03:56:18.000000 fuo-ytmusic-0.2.3/fuo_ytmusic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-15 03:56:17.000000 fuo-ytmusic-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-15 03:56:18.909745 fuo-ytmusic-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-15 03:56:17.000000 fuo-ytmusic-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:51:49.914305 fuo-ytmusic-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-18 15:51:48.000000 fuo-ytmusic-0.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-18 15:51:49.914305 fuo-ytmusic-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-18 15:51:48.000000 fuo-ytmusic-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:51:49.910305 fuo-ytmusic-0.3.0/fuo_ytmusic/
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-18 15:51:48.000000 fuo-ytmusic-0.3.0/fuo_ytmusic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:51:49.914305 fuo-ytmusic-0.3.0/fuo_ytmusic/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-18 15:51:48.000000 fuo-ytmusic-0.3.0/fuo_ytmusic/assets/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-18 15:51:48.000000 fuo-ytmusic-0.3.0/fuo_ytmusic/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-18 15:51:48.000000 fuo-ytmusic-0.3.0/fuo_ytmusic/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18260 2023-07-18 15:51:48.000000 fuo-ytmusic-0.3.0/fuo_ytmusic/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-07-18 15:51:48.000000 fuo-ytmusic-0.3.0/fuo_ytmusic/page_explore_qml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-18 15:51:48.000000 fuo-ytmusic-0.3.0/fuo_ytmusic/page_fav.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-07-18 15:51:48.000000 fuo-ytmusic-0.3.0/fuo_ytmusic/page_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-18 15:51:48.000000 fuo-ytmusic-0.3.0/fuo_ytmusic/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10642 2023-07-18 15:51:48.000000 fuo-ytmusic-0.3.0/fuo_ytmusic/provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:51:49.914305 fuo-ytmusic-0.3.0/fuo_ytmusic/qml/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:51:49.914305 fuo-ytmusic-0.3.0/fuo_ytmusic/qml/dummydata/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-18 15:51:48.000000 fuo-ytmusic-0.3.0/fuo_ytmusic/qml/dummydata/explore_backend.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-07-18 15:51:48.000000 fuo-ytmusic-0.3.0/fuo_ytmusic/qml/page_explore.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-18 15:51:48.000000 fuo-ytmusic-0.3.0/fuo_ytmusic/qml/uploader.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    13967 2023-07-18 15:51:48.000000 fuo-ytmusic-0.3.0/fuo_ytmusic/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-07-18 15:51:48.000000 fuo-ytmusic-0.3.0/fuo_ytmusic/timeparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-07-18 15:51:48.000000 fuo-ytmusic-0.3.0/fuo_ytmusic/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:51:49.914305 fuo-ytmusic-0.3.0/fuo_ytmusic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-18 15:51:49.000000 fuo-ytmusic-0.3.0/fuo_ytmusic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-18 15:51:49.000000 fuo-ytmusic-0.3.0/fuo_ytmusic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 15:51:49.000000 fuo-ytmusic-0.3.0/fuo_ytmusic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-18 15:51:49.000000 fuo-ytmusic-0.3.0/fuo_ytmusic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-18 15:51:49.000000 fuo-ytmusic-0.3.0/fuo_ytmusic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-18 15:51:49.000000 fuo-ytmusic-0.3.0/fuo_ytmusic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-18 15:51:48.000000 fuo-ytmusic-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-18 15:51:49.914305 fuo-ytmusic-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-18 15:51:48.000000 fuo-ytmusic-0.3.0/setup.py
```

### Comparing `fuo-ytmusic-0.2.3/LICENSE.txt` & `fuo-ytmusic-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fuo-ytmusic-0.2.3/PKG-INFO` & `fuo-ytmusic-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: fuo-ytmusic
-Version: 0.2.3
+Version: 0.3.0
 Summary: feeluown Youtube Music plugin
 Home-page: https://github.com/feeluown/feeluown-ytmusic
 Author: Bruce Zhang
 Author-email: zttt183525594@gmail.com
 License: UNKNOWN
 Description: # YouTube Music plugin for FeelUOwn player
```

### Comparing `fuo-ytmusic-0.2.3/README.md` & `fuo-ytmusic-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,16 @@
 - [x] Get song detail by id
 - [ ] Add/remove song from a playlist
 - [ ] Upload songs to cloud
 - [ ] Discovering page
 
 ## Changelog
 
+- v0.3.0 (2023-07-18)
+  - use pydantic>=2.0
 - v0.2.3 (2023-07-15)
   - fix loading header_file failed
 - v0.2.2 (2023-07-13)
   - fix can't get song media properly
 
 ## License
```

### Comparing `fuo-ytmusic-0.2.3/fuo_ytmusic/__init__.py` & `fuo-ytmusic-0.3.0/fuo_ytmusic/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from feeluown.app import App
 
 __alias__ = 'ytmusic'
-__version__ = '0.2.3'
+__version__ = '0.3.0'
 __desc__ = 'YouTube Music plugin'
 
 
 ui_mgr = None
 
 
 def init_config(config):
```

### Comparing `fuo-ytmusic-0.2.3/fuo_ytmusic/assets/icon.svg` & `fuo-ytmusic-0.3.0/fuo_ytmusic/assets/icon.svg`

 * *Files identical despite different names*

### Comparing `fuo-ytmusic-0.2.3/fuo_ytmusic/models.py` & `fuo-ytmusic-0.3.0/fuo_ytmusic/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Optional, Union, List, Tuple
 
-from feeluown.utils.reader import SequentialReader
-from pydantic import BaseModel as PydanticBaseModel
-from pydantic.fields import Field
 # noinspection PyProtectedMember
-from pydantic.main import ModelMetaclass
+from pydantic.v1.fields import Field
+from pydantic.v1 import BaseModel as PydanticBaseModel
+from pydantic.v1.main import ModelMetaclass
 
+from feeluown.utils.reader import SequentialReader
 from feeluown.media import Quality
 from feeluown.library import (
     VideoModel, ModelState, BriefArtistModel, BriefUserModel,
     AlbumModel as AlbumModelV2, BriefSongModel, SongModel as SongModelV2,
     BriefAlbumModel, ArtistModel as ArtistModelV2, PlaylistModel,
     BriefPlaylistModel,
 )
@@ -227,15 +227,15 @@
 
 class YtmusicLibraryArtist(YtmusicSearchArtist):
     subscribers: str  # 歌曲数量
 
 
 class YtmusicSearchPlaylist(YtmusicSearchBase, YtmusicCoverMixin):
     title: str  # 歌单名
-    itemCount: Optional[int]  # 歌曲数量
+    itemCount: Optional[int] = None  # 歌曲数量
     author: str  # 歌单作者
     browseId: str  # 查询ID
 
     def v2_brief_model(self) -> BriefPlaylistModel:
         return BriefPlaylistModel(
             identifier=self.browseId,
             source=self.source,
```

### Comparing `fuo-ytmusic-0.2.3/fuo_ytmusic/page_explore_qml.py` & `fuo-ytmusic-0.3.0/fuo_ytmusic/page_explore_qml.py`

 * *Files identical despite different names*

### Comparing `fuo-ytmusic-0.2.3/fuo_ytmusic/page_fav.py` & `fuo-ytmusic-0.3.0/fuo_ytmusic/page_fav.py`

 * *Files identical despite different names*

### Comparing `fuo-ytmusic-0.2.3/fuo_ytmusic/page_more.py` & `fuo-ytmusic-0.3.0/fuo_ytmusic/page_more.py`

 * *Files identical despite different names*

### Comparing `fuo-ytmusic-0.2.3/fuo_ytmusic/patch.py` & `fuo-ytmusic-0.3.0/fuo_ytmusic/patch.py`

 * *Files identical despite different names*

### Comparing `fuo-ytmusic-0.2.3/fuo_ytmusic/provider.py` & `fuo-ytmusic-0.3.0/fuo_ytmusic/provider.py`

 * *Files identical despite different names*

### Comparing `fuo-ytmusic-0.2.3/fuo_ytmusic/qml/dummydata/explore_backend.qml` & `fuo-ytmusic-0.3.0/fuo_ytmusic/qml/dummydata/explore_backend.qml`

 * *Files identical despite different names*

### Comparing `fuo-ytmusic-0.2.3/fuo_ytmusic/qml/page_explore.qml` & `fuo-ytmusic-0.3.0/fuo_ytmusic/qml/page_explore.qml`

 * *Files identical despite different names*

### Comparing `fuo-ytmusic-0.2.3/fuo_ytmusic/qml/uploader.qml` & `fuo-ytmusic-0.3.0/fuo_ytmusic/qml/uploader.qml`

 * *Files identical despite different names*

### Comparing `fuo-ytmusic-0.2.3/fuo_ytmusic/service.py` & `fuo-ytmusic-0.3.0/fuo_ytmusic/service.py`

 * *Files identical despite different names*

### Comparing `fuo-ytmusic-0.2.3/fuo_ytmusic/timeparse.py` & `fuo-ytmusic-0.3.0/fuo_ytmusic/timeparse.py`

 * *Files identical despite different names*

### Comparing `fuo-ytmusic-0.2.3/fuo_ytmusic/ui.py` & `fuo-ytmusic-0.3.0/fuo_ytmusic/ui.py`

 * *Files identical despite different names*

### Comparing `fuo-ytmusic-0.2.3/fuo_ytmusic.egg-info/PKG-INFO` & `fuo-ytmusic-0.3.0/fuo_ytmusic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: fuo-ytmusic
-Version: 0.2.3
+Version: 0.3.0
 Summary: feeluown Youtube Music plugin
 Home-page: https://github.com/feeluown/feeluown-ytmusic
 Author: Bruce Zhang
 Author-email: zttt183525594@gmail.com
 License: UNKNOWN
 Description: # YouTube Music plugin for FeelUOwn player
```

### Comparing `fuo-ytmusic-0.2.3/fuo_ytmusic.egg-info/SOURCES.txt` & `fuo-ytmusic-0.3.0/fuo_ytmusic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fuo-ytmusic-0.2.3/pyproject.toml` & `fuo-ytmusic-0.3.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fuo-ytmusic"
-version = "0.2.3"
+version = "0.3.0"
 description = "feeluown Youtube Music plugin"
 authors = ["Bruce Zhang <zttt183525594@gmail.com>"]
 keywords = ["feeluown", "ytmusic", "youtube"]
 homepage = "https://github.com/feeluown/feeluown-ytmusic"
 readme = "README.md"
 include = ["fuo_ytmusic/assets/*.svg", "fuo_ytmusic/qml/*.qml"]
```

### Comparing `fuo-ytmusic-0.2.3/setup.py` & `fuo-ytmusic-0.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['cachetools', 'feeluown>=3.7.13', 'pydantic', 'pytube', 'ytmusicapi']
 
 entry_points = \
 {'fuo.plugins_v1': ['ytmusic = fuo_ytmusic']}
 
 setup_kwargs = {
     'name': 'fuo-ytmusic',
-    'version': '0.2.3',
+    'version': '0.3.0',
     'description': 'feeluown Youtube Music plugin',
     'long_description': "# YouTube Music plugin for FeelUOwn player\n\n## Prerequisites\n\nInstall [FeelUOwn](https://github.com/feeluown/FeelUOwn) before installing this plugin.\nSees: [Documentation](https://feeluown.readthedocs.io/)\n\n## Installation\n\n```shell\npip install fuo-ytmusic  # Lastest stable release\npip install https://github.com/feeluown/feeluown-ytmusic.git  # master branch\npoetry install  # Local development\n```\n\n## Configuration\n\n### Proxies\n\n```python\n# In ~/.fuorc\nconfig.deffield('YTM_HTTP_PROXY', type_=str, default='', desc='YouTube Music 代理设置')\nconfig.YTM_HTTP_PROXY='127.0.0.1:10809'\n```\n\n## Contributing\n\nPull requests are welcome. For major changes, please create a new issue first to discuss what you'd like to change.\n\nPlease make sure to compatible with [FeelUOwn](https://github.com/feeluown/FeelUOwn) lastest stable release.\n\n## License\n\nThis project is licensed under the [GPLv3](LICENSE.txt).\n",
     'author': 'Bruce Zhang',
     'author_email': 'zttt183525594@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/feeluown/feeluown-ytmusic',
```

