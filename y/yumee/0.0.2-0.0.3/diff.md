# Comparing `tmp/yumee-0.0.2.tar.gz` & `tmp/yumee-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yumee-0.0.2.tar", max compression
+gzip compressed data, was "yumee-0.0.3.tar", max compression
```

## Comparing `yumee-0.0.2.tar` & `yumee-0.0.3.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0     1063 2023-07-17 13:43:05.935670 yumee-0.0.2/LICENSE
--rw-r--r--   0        0        0     2683 2023-07-17 13:43:05.935670 yumee-0.0.2/README.md
--rw-r--r--   0        0        0     1292 2023-07-17 13:43:05.935670 yumee-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      401 2023-07-17 13:43:06.139672 yumee-0.0.2/yumee/__init__.py
--rw-r--r--   0        0        0      650 2023-07-17 13:43:06.139672 yumee-0.0.2/yumee/classes/__init__.py
--rw-r--r--   0        0        0      535 2023-07-17 13:43:06.139672 yumee-0.0.2/yumee/classes/handlers/__init__.py
--rw-r--r--   0        0        0      716 2023-07-17 13:43:06.139672 yumee-0.0.2/yumee/classes/handlers/abstract_song_file_provider.py
--rw-r--r--   0        0        0      430 2023-07-17 13:43:06.139672 yumee-0.0.2/yumee/classes/handlers/flac_song_file_provider.py
--rw-r--r--   0        0        0      425 2023-07-17 13:43:06.139672 yumee-0.0.2/yumee/classes/handlers/m4a_song_file_provider.py
--rw-r--r--   0        0        0      425 2023-07-17 13:43:06.139672 yumee-0.0.2/yumee/classes/handlers/mp3_song_file_provider.py
--rw-r--r--   0        0        0      425 2023-07-17 13:43:06.139672 yumee-0.0.2/yumee/classes/handlers/ogg_song_file_provider.py
--rw-r--r--   0        0        0      430 2023-07-17 13:43:06.139672 yumee-0.0.2/yumee/classes/handlers/opus_song_file_provider.py
--rw-r--r--   0        0        0      385 2023-07-17 13:43:06.139672 yumee-0.0.2/yumee/classes/song_files/__init__.py
--rw-r--r--   0        0        0     7007 2023-07-17 13:43:06.139672 yumee-0.0.2/yumee/classes/song_files/abstract_song_file.py
--rw-r--r--   0        0        0     4859 2023-07-17 13:43:06.139672 yumee-0.0.2/yumee/classes/song_files/flac_song_file.py
--rw-r--r--   0        0        0     4377 2023-07-17 13:43:06.139672 yumee-0.0.2/yumee/classes/song_files/m4a_song_file.py
--rw-r--r--   0        0        0     7978 2023-07-17 13:43:06.139672 yumee-0.0.2/yumee/classes/song_files/mp3_song_file.py
--rw-r--r--   0        0        0     5104 2023-07-17 13:43:06.139672 yumee-0.0.2/yumee/classes/song_files/ogg_song_file.py
--rw-r--r--   0        0        0     5096 2023-07-17 13:43:06.139672 yumee-0.0.2/yumee/classes/song_files/opus_song_file.py
--rw-r--r--   0        0        0      827 2023-07-17 13:43:06.139672 yumee-0.0.2/yumee/classes/song_metadata.py
--rw-r--r--   0        0        0      522 2023-07-17 13:43:06.139672 yumee-0.0.2/yumee/classes/tag_preset.py
--rw-r--r--   0        0        0       59 2023-07-17 13:43:06.139672 yumee-0.0.2/yumee/classes/tools/__init__.py
--rw-r--r--   0        0        0     1824 2023-07-17 13:43:06.143672 yumee-0.0.2/yumee/classes/tools/lrc_helper.py
--rw-r--r--   0        0        0       67 2023-07-17 13:43:06.143672 yumee-0.0.2/yumee/di/__init__.py
--rw-r--r--   0        0        0      582 2023-07-17 13:43:06.143672 yumee-0.0.2/yumee/di/dependency_injector.py
--rw-r--r--   0        0        0      169 2023-07-17 13:43:06.143672 yumee-0.0.2/yumee/errors/__init__.py
--rw-r--r--   0        0        0       79 2023-07-17 13:43:06.143672 yumee-0.0.2/yumee/errors/song_metadata_error.py
--rw-r--r--   0        0        0      147 2023-07-17 13:43:06.143672 yumee-0.0.2/yumee/errors/song_metadata_file_error.py
--rw-r--r--   0        0        0      151 2023-07-17 13:43:06.143672 yumee-0.0.2/yumee/interfaces/__init__.py
--rw-r--r--   0        0        0     4252 2023-07-17 13:43:06.143672 yumee-0.0.2/yumee/interfaces/base_song_file.py
--rw-r--r--   0        0        0      196 2023-07-17 13:43:06.143672 yumee-0.0.2/yumee/interfaces/base_song_file_provider.py
--rw-r--r--   0        0        0     2763 2023-07-17 13:43:06.143672 yumee-0.0.2/yumee/main.py
--rw-r--r--   0        0        0        0 2023-07-17 13:43:06.143672 yumee-0.0.2/yumee/py.typed
--rw-r--r--   0        0        0     3732 1970-01-01 00:00:00.000000 yumee-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-18 13:40:25.085725 yumee-0.0.3/LICENSE
+-rw-r--r--   0        0        0     3361 2023-07-18 13:40:25.085725 yumee-0.0.3/README.md
+-rw-r--r--   0        0        0     1292 2023-07-18 13:40:25.085725 yumee-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      398 2023-07-18 13:40:25.305727 yumee-0.0.3/yumee/__init__.py
+-rw-r--r--   0        0        0      539 2023-07-18 13:40:25.309727 yumee-0.0.3/yumee/classes/__init__.py
+-rw-r--r--   0        0        0      535 2023-07-18 13:40:25.309727 yumee-0.0.3/yumee/classes/handlers/__init__.py
+-rw-r--r--   0        0        0      716 2023-07-18 13:40:25.309727 yumee-0.0.3/yumee/classes/handlers/abstract_song_file_provider.py
+-rw-r--r--   0        0        0      430 2023-07-18 13:40:25.309727 yumee-0.0.3/yumee/classes/handlers/flac_song_file_provider.py
+-rw-r--r--   0        0        0      425 2023-07-18 13:40:25.309727 yumee-0.0.3/yumee/classes/handlers/m4a_song_file_provider.py
+-rw-r--r--   0        0        0      425 2023-07-18 13:40:25.309727 yumee-0.0.3/yumee/classes/handlers/mp3_song_file_provider.py
+-rw-r--r--   0        0        0      425 2023-07-18 13:40:25.309727 yumee-0.0.3/yumee/classes/handlers/ogg_song_file_provider.py
+-rw-r--r--   0        0        0      430 2023-07-18 13:40:25.309727 yumee-0.0.3/yumee/classes/handlers/opus_song_file_provider.py
+-rw-r--r--   0        0        0      385 2023-07-18 13:40:25.309727 yumee-0.0.3/yumee/classes/song_files/__init__.py
+-rw-r--r--   0        0        0     9955 2023-07-18 13:40:25.309727 yumee-0.0.3/yumee/classes/song_files/abstract_song_file.py
+-rw-r--r--   0        0        0     4856 2023-07-18 13:40:25.309727 yumee-0.0.3/yumee/classes/song_files/flac_song_file.py
+-rw-r--r--   0        0        0     4374 2023-07-18 13:40:25.309727 yumee-0.0.3/yumee/classes/song_files/m4a_song_file.py
+-rw-r--r--   0        0        0     8000 2023-07-18 13:40:25.309727 yumee-0.0.3/yumee/classes/song_files/mp3_song_file.py
+-rw-r--r--   0        0        0     5101 2023-07-18 13:40:25.309727 yumee-0.0.3/yumee/classes/song_files/ogg_song_file.py
+-rw-r--r--   0        0        0     5093 2023-07-18 13:40:25.309727 yumee-0.0.3/yumee/classes/song_files/opus_song_file.py
+-rw-r--r--   0        0        0       59 2023-07-18 13:40:25.309727 yumee-0.0.3/yumee/classes/tools/__init__.py
+-rw-r--r--   0        0        0     1824 2023-07-18 13:40:25.309727 yumee-0.0.3/yumee/classes/tools/lrc_helper.py
+-rw-r--r--   0        0        0       73 2023-07-18 13:40:25.309727 yumee-0.0.3/yumee/data/__init__.py
+-rw-r--r--   0        0        0      827 2023-07-18 13:40:25.309727 yumee-0.0.3/yumee/data/song_metadata.py
+-rw-r--r--   0        0        0      522 2023-07-18 13:40:25.309727 yumee-0.0.3/yumee/data/tag_preset.py
+-rw-r--r--   0        0        0       67 2023-07-18 13:40:25.309727 yumee-0.0.3/yumee/di/__init__.py
+-rw-r--r--   0        0        0      582 2023-07-18 13:40:25.309727 yumee-0.0.3/yumee/di/dependency_injector.py
+-rw-r--r--   0        0        0      169 2023-07-18 13:40:25.309727 yumee-0.0.3/yumee/errors/__init__.py
+-rw-r--r--   0        0        0       79 2023-07-18 13:40:25.309727 yumee-0.0.3/yumee/errors/song_metadata_error.py
+-rw-r--r--   0        0        0      147 2023-07-18 13:40:25.309727 yumee-0.0.3/yumee/errors/song_metadata_file_error.py
+-rw-r--r--   0        0        0      151 2023-07-18 13:40:25.309727 yumee-0.0.3/yumee/interfaces/__init__.py
+-rw-r--r--   0        0        0     4470 2023-07-18 13:40:25.309727 yumee-0.0.3/yumee/interfaces/base_song_file.py
+-rw-r--r--   0        0        0      196 2023-07-18 13:40:25.309727 yumee-0.0.3/yumee/interfaces/base_song_file_provider.py
+-rw-r--r--   0        0        0      778 2023-07-18 13:40:25.309727 yumee-0.0.3/yumee/main.py
+-rw-r--r--   0        0        0        0 2023-07-18 13:40:25.309727 yumee-0.0.3/yumee/py.typed
+-rw-r--r--   0        0        0     4410 1970-01-01 00:00:00.000000 yumee-0.0.3/PKG-INFO
```

### Comparing `yumee-0.0.2/LICENSE` & `yumee-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yumee-0.0.2/README.md` & `yumee-0.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -29,17 +29,18 @@
 
 ## Usage
 
 There are 2 ways to use this library : using the SongMetadataEmbedder object or via the DI.
 
 ### Using SongMetadataEmbedder
 
-The library exposes the SongMetadataEmbedder class. This class has 2 method : `open_file` and `embed`.
+The library exposes the SongMetadataEmbedder class. This class has 1 method : `open_file`.
 
-`open_file` opens an audio file at a provided path and returns a `BaseSongFile` to manipulate its metadata. `embed` opens an audio file and modifies its metadata according to the data provided.
+`open_file` opens an audio file at a provided path and returns a `BaseSongFile` to manipulate its metadata.  
+Once you have a `BaseSongFile`, you have access to methods like `embed` or `extract`. `embed` modifies the metadata of the SongFile according to the data provided. `extract` returns the metadata that was embedded in the file.
 
 **Example 1 :**
 
 ```python
 from pathlib import Path
 from yumee import SongMetadataEmbedder
 
@@ -58,17 +59,20 @@
 from pathlib import Path
 from yumee import SongMetadataEmbedder, SongMetadata
 
 embedder = SongMetadataEmbedder()
 path = Path("path/to/file.mp3")
 metadata = SongMetadata(title="New Title")
 
-embedder.embed(path, metadata)
+song_file = embedder.open_file(path)
+song_file.embed(metadata)
 ```
 
+*The 'embed' method automatically saves the modifications done. This is why I don't use 'open_file' with a 'with' statement.*
+
 ### Using DI
 
 The library also exposes a `BaseSongFileProvider` interface and a `add_yumee` function for [Taipan-DI](https://github.com/Billuc/Taipan-DI).
 
 In this function, SongFileProviders are registered as a Pipeline. Each SongFileProvider correspond to a specific file type and generates a `BaseSongFile`. Resolve the pipeline and execute it to have a `BaseSongFile` you can then manipulate.
 
 **Example :**
@@ -87,7 +91,20 @@
 with song_file_provider.exec(path) as song_file:
     ...
 ```
 
 ## Inspirations
 
 This library is partially inspired by spotDL's [spotify-downloader](https://github.com/spotDL/spotify-downloader) and utilises [mutagen](https://mutagen.readthedocs.io/en/latest/).
+
+## TODO
+
+This library isn't stable yet and a lot of things can still be improved.
+If there is something you want to see added or if something does not work as you want it to, feel free to open an issue.
+
+Here is a list of features I have in mind and will be working on :
+
+- ~~Generate SongMetadata from a SongFile~~
+- Support Wav
+- ISRC tag
+- MP3 separator support
+- Popularity tag (ID3)
```

### Comparing `yumee-0.0.2/pyproject.toml` & `yumee-0.0.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Yumee"
-version = "0.0.2"
+version = "0.0.3"
 description = "Yet Unother MEtadata Embedder"
 authors = ["Billuc <billuc@hotmail.fr>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "yumee"}]
 
 keywords = ["yumee", "song metadata", "song", "metadata", "metadata embedder", "python", "mp3", "m4a", "ogg", "flac", "opus"]
```

### Comparing `yumee-0.0.2/yumee/classes/__init__.py` & `yumee-0.0.3/yumee/classes/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,19 @@
-from .song_metadata import SongMetadata
-from .tag_preset import TagPreset
 from .tools import LRCHelper
 
 from .handlers import (
     FlacSongFileProvider,
     M4ASongFileProvider,
     Mp3SongFileProvider,
     OggSongFileProvider,
     OpusSongFileProvider,
 )
 from .song_files import FlacSongFile, M4ASongFile, Mp3SongFile, OggSongFile, OpusSongFile
 
 __all__ = [
-    "SongMetadata",
-    "TagPreset",
     "LRCHelper",
     "FlacSongFile",
     "M4ASongFile",
     "Mp3SongFile",
     "OggSongFile",
     "OpusSongFile",
     "FlacSongFileProvider",
```

### Comparing `yumee-0.0.2/yumee/classes/handlers/__init__.py` & `yumee-0.0.3/yumee/classes/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `yumee-0.0.2/yumee/classes/handlers/abstract_song_file_provider.py` & `yumee-0.0.3/yumee/classes/handlers/abstract_song_file_provider.py`

 * *Files identical despite different names*

### Comparing `yumee-0.0.2/yumee/classes/song_files/flac_song_file.py` & `yumee-0.0.3/yumee/classes/song_files/flac_song_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 __all__ = ["FlacSongFile"]
 
 from typing import List, Optional, Tuple
 from mutagen.flac import FLAC, Picture
 import requests
 
-from yumee.classes import TagPreset
+from yumee.data import TagPreset
 from .abstract_song_file import AbstractSongFile
 
 
 class FlacSongFile(AbstractSongFile[FLAC]):
     @property
     def tag_preset(self) -> TagPreset:
         return TagPreset(
```

### Comparing `yumee-0.0.2/yumee/classes/song_files/m4a_song_file.py` & `yumee-0.0.3/yumee/classes/song_files/m4a_song_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 __all__ = ["M4ASongFile"]
 
 from typing import List, Optional, Tuple, cast
 from mutagen.mp4 import MP4, MP4Cover
 import requests
 
-from yumee.classes import TagPreset
+from yumee.data import TagPreset
 from .abstract_song_file import AbstractSongFile
 
 
 class M4ASongFile(AbstractSongFile[MP4]):
     @property
     def tag_preset(self) -> TagPreset:
         return TagPreset(
```

### Comparing `yumee-0.0.2/yumee/classes/song_files/mp3_song_file.py` & `yumee-0.0.3/yumee/classes/song_files/mp3_song_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 import requests
 
 from mutagen.mp3 import MP3, EasyMP3
 from mutagen.id3 import ID3
 from mutagen.id3._frames import APIC, COMM, WOAS, USLT, SYLT
 from mutagen.id3._specs import Encoding
 
-from yumee.classes import TagPreset, LRCHelper
+from yumee.classes import LRCHelper
+from yumee.data import TagPreset
 from .abstract_song_file import AbstractSongFile
 
 
 class Mp3SongFile(AbstractSongFile[MP3]):
     @property
     def tag_preset(self) -> TagPreset:
         return TagPreset(
```

### Comparing `yumee-0.0.2/yumee/classes/song_files/ogg_song_file.py` & `yumee-0.0.3/yumee/classes/song_files/ogg_song_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import base64
 from typing import List, Optional, Tuple
 from mutagen.flac import Picture
 from mutagen.oggvorbis import OggVorbis
 import requests
 
-from yumee.classes import TagPreset
+from yumee.data import TagPreset
 from .abstract_song_file import AbstractSongFile
 
 
 class OggSongFile(AbstractSongFile[OggVorbis]):
     @property
     def tag_preset(self) -> TagPreset:
         return TagPreset(
```

### Comparing `yumee-0.0.2/yumee/classes/song_files/opus_song_file.py` & `yumee-0.0.3/yumee/classes/song_files/opus_song_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import base64
 from typing import List, Optional, Tuple
 from mutagen.flac import Picture
 from mutagen.oggopus import OggOpus
 import requests
 
-from yumee.classes import TagPreset
+from yumee.data import TagPreset
 from .abstract_song_file import AbstractSongFile
 
 
 class OpusSongFile(AbstractSongFile[OggOpus]):
     @property
     def tag_preset(self) -> TagPreset:
         return TagPreset(
```

### Comparing `yumee-0.0.2/yumee/classes/song_metadata.py` & `yumee-0.0.3/yumee/data/song_metadata.py`

 * *Files identical despite different names*

### Comparing `yumee-0.0.2/yumee/classes/tag_preset.py` & `yumee-0.0.3/yumee/data/tag_preset.py`

 * *Files identical despite different names*

### Comparing `yumee-0.0.2/yumee/classes/tools/lrc_helper.py` & `yumee-0.0.3/yumee/classes/tools/lrc_helper.py`

 * *Files identical despite different names*

### Comparing `yumee-0.0.2/yumee/di/dependency_injector.py` & `yumee-0.0.3/yumee/di/dependency_injector.py`

 * *Files identical despite different names*

### Comparing `yumee-0.0.2/yumee/interfaces/base_song_file.py` & `yumee-0.0.3/yumee/interfaces/base_song_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import abc
 from typing import List, Optional, Protocol, Tuple
+from yumee.data import SongMetadata
 
 __all__ = ["BaseSongFile"]
 
 
 class BaseSongFile(Protocol):
     @abc.abstractmethod
     def __enter__(self) -> BaseSongFile:
@@ -14,14 +15,22 @@
     @abc.abstractmethod
     def __exit__(self, type, value, traceback):
         ...
 
     @abc.abstractmethod
     def save(self) -> None:
         ...
+        
+    @abc.abstractmethod
+    def embed(self, metadata: SongMetadata) -> None:
+        ...
+        
+    @abc.abstractmethod
+    def extract(self) -> SongMetadata:
+        ...
 
     # Title
 
     @property
     @abc.abstractmethod
     def title(self) -> Optional[List[str]]:
         ...
```

### Comparing `yumee-0.0.2/PKG-INFO` & `yumee-0.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yumee
-Version: 0.0.2
+Version: 0.0.3
 Summary: Yet Unother MEtadata Embedder
 Home-page: https://github.com/Billuc/Yumee
 License: MIT
 Keywords: yumee,song metadata,song,metadata,metadata embedder,python,mp3,m4a,ogg,flac,opus
 Author: Billuc
 Author-email: billuc@hotmail.fr
 Requires-Python: >=3.9,<4.0
@@ -56,17 +56,18 @@
 
 ## Usage
 
 There are 2 ways to use this library : using the SongMetadataEmbedder object or via the DI.
 
 ### Using SongMetadataEmbedder
 
-The library exposes the SongMetadataEmbedder class. This class has 2 method : `open_file` and `embed`.
+The library exposes the SongMetadataEmbedder class. This class has 1 method : `open_file`.
 
-`open_file` opens an audio file at a provided path and returns a `BaseSongFile` to manipulate its metadata. `embed` opens an audio file and modifies its metadata according to the data provided.
+`open_file` opens an audio file at a provided path and returns a `BaseSongFile` to manipulate its metadata.  
+Once you have a `BaseSongFile`, you have access to methods like `embed` or `extract`. `embed` modifies the metadata of the SongFile according to the data provided. `extract` returns the metadata that was embedded in the file.
 
 **Example 1 :**
 
 ```python
 from pathlib import Path
 from yumee import SongMetadataEmbedder
 
@@ -85,17 +86,20 @@
 from pathlib import Path
 from yumee import SongMetadataEmbedder, SongMetadata
 
 embedder = SongMetadataEmbedder()
 path = Path("path/to/file.mp3")
 metadata = SongMetadata(title="New Title")
 
-embedder.embed(path, metadata)
+song_file = embedder.open_file(path)
+song_file.embed(metadata)
 ```
 
+*The 'embed' method automatically saves the modifications done. This is why I don't use 'open_file' with a 'with' statement.*
+
 ### Using DI
 
 The library also exposes a `BaseSongFileProvider` interface and a `add_yumee` function for [Taipan-DI](https://github.com/Billuc/Taipan-DI).
 
 In this function, SongFileProviders are registered as a Pipeline. Each SongFileProvider correspond to a specific file type and generates a `BaseSongFile`. Resolve the pipeline and execute it to have a `BaseSongFile` you can then manipulate.
 
 **Example :**
@@ -115,7 +119,20 @@
     ...
 ```
 
 ## Inspirations
 
 This library is partially inspired by spotDL's [spotify-downloader](https://github.com/spotDL/spotify-downloader) and utilises [mutagen](https://mutagen.readthedocs.io/en/latest/).
 
+## TODO
+
+This library isn't stable yet and a lot of things can still be improved.
+If there is something you want to see added or if something does not work as you want it to, feel free to open an issue.
+
+Here is a list of features I have in mind and will be working on :
+
+- ~~Generate SongMetadata from a SongFile~~
+- Support Wav
+- ISRC tag
+- MP3 separator support
+- Popularity tag (ID3)
+
```

