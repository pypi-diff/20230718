# Comparing `tmp/ayt-api-0.1.2.tar.gz` & `tmp/ayt-api-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ayt-api-0.1.2.tar", last modified: Sat Jun 17 11:22:07 2023, max compression
+gzip compressed data, was "ayt-api-0.1.3.tar", last modified: Tue Jul 18 12:11:49 2023, max compression
```

## Comparing `ayt-api-0.1.2.tar` & `ayt-api-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:22:07.010930 ayt-api-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-17 11:21:56.000000 ayt-api-0.1.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-06-17 11:22:07.010930 ayt-api-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-06-17 11:21:56.000000 ayt-api-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:22:07.010930 ayt-api-0.1.2/ayt_api/
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-17 11:21:56.000000 ayt-api-0.1.2/ayt_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-06-17 11:21:56.000000 ayt-api-0.1.2/ayt_api/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-06-17 11:21:56.000000 ayt-api-0.1.2/ayt_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    51228 2023-06-17 11:21:56.000000 ayt-api-0.1.2/ayt_api/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-17 11:21:56.000000 ayt-api-0.1.2/ayt_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:22:07.010930 ayt-api-0.1.2/ayt_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-06-17 11:22:07.000000 ayt-api-0.1.2/ayt_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-17 11:22:07.000000 ayt-api-0.1.2/ayt_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 11:22:07.000000 ayt-api-0.1.2/ayt_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-17 11:22:07.000000 ayt-api-0.1.2/ayt_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-17 11:22:07.000000 ayt-api-0.1.2/ayt_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-17 11:21:56.000000 ayt-api-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-17 11:21:56.000000 ayt-api-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-17 11:22:07.010930 ayt-api-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-17 11:21:56.000000 ayt-api-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:11:49.409800 ayt-api-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-18 12:11:36.000000 ayt-api-0.1.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-07-18 12:11:49.409800 ayt-api-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-07-18 12:11:36.000000 ayt-api-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:11:49.409800 ayt-api-0.1.3/ayt_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-18 12:11:36.000000 ayt-api-0.1.3/ayt_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-07-18 12:11:36.000000 ayt-api-0.1.3/ayt_api/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-07-18 12:11:36.000000 ayt-api-0.1.3/ayt_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52925 2023-07-18 12:11:36.000000 ayt-api-0.1.3/ayt_api/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-18 12:11:36.000000 ayt-api-0.1.3/ayt_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:11:49.409800 ayt-api-0.1.3/ayt_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-07-18 12:11:49.000000 ayt-api-0.1.3/ayt_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-18 12:11:49.000000 ayt-api-0.1.3/ayt_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 12:11:49.000000 ayt-api-0.1.3/ayt_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-18 12:11:49.000000 ayt-api-0.1.3/ayt_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-18 12:11:49.000000 ayt-api-0.1.3/ayt_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-18 12:11:36.000000 ayt-api-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-18 12:11:36.000000 ayt-api-0.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-18 12:11:49.409800 ayt-api-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-18 12:11:36.000000 ayt-api-0.1.3/setup.py
```

### Comparing `ayt-api-0.1.2/LICENSE.md` & `ayt-api-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ayt-api-0.1.2/PKG-INFO` & `ayt-api-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ayt-api
-Version: 0.1.2
+Version: 0.1.3
 Summary: An Asynchronous, Object oriented python library for the YouTube api
 Home-page: https://github.com/Revnoplex/ayt-api
 Author: Revnoplex
 Author-email: Revnoplex <revnoplex.business@protonmail.com>
 License: # MIT License
         
         Copyright (c) 2022-2023 Revnoplex
```

### Comparing `ayt-api-0.1.2/README.md` & `ayt-api-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ayt-api-0.1.2/ayt_api/__init__.py` & `ayt-api-0.1.3/ayt_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from .exceptions import *
 from . import utils
 
 __title__ = "ayt-api"
 __author__ = "Revnoplex"
 __license__ = "MIT"
 __copyright__ = "Copyright (c) 2022-2023 Revnoplex"
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 
 
 class VersionInfo(_NamedTuple):
     major: int
     minor: int
     micro: int
     release_level: str
```

### Comparing `ayt-api-0.1.2/ayt_api/api.py` & `ayt-api-0.1.3/ayt_api/api.py`

 * *Files identical despite different names*

### Comparing `ayt-api-0.1.2/ayt_api/exceptions.py` & `ayt-api-0.1.3/ayt_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `ayt-api-0.1.2/ayt_api/types.py` & `ayt-api-0.1.3/ayt_api/types.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,34 @@
 import datetime
+import re
+from dataclasses import dataclass
 from typing import Union, Optional
 import isodate
 from .exceptions import MissingDataFromMetadata
 
 
+@dataclass
 class YoutubeThumbnail:
     """Data for an individual YouTube thumbnail.
     Attributes:
-        data (Optional[dict]):
-            The raw thumbnail data
         url (Optional[str]): The file url for the thumbnail
         width (Optional[int]): The amount of horizontal pixels in the thumbnail
         height (Optional[int]): The amount of vertical pixels in the thumbnail
         resolution (str): The Width x Height of the thumbnail
     """
-    def __init__(self, data: dict):
-        """
-        Args:
-            data (dict): The raw thumbnail data
-        """
-        self.data = data
-        self.url: Optional[str] = data.get("url")
-        self.width: Optional[int] = data.get("width")
-        self.height: Optional[int] = data.get("height")
+    url: Optional[str]
+    width: Optional[int]
+    height: Optional[int]
+
+    def __post_init__(self):
         self.resolution = "{}x{}".format(self.width, self.height)
 
     def __str__(self):
         return self.url
 
-    def __repr__(self):
-        return f"YoutubeThumbnail({self.url}, {self.width},{self.height})"
-
 
 class YoutubeThumbnailMetadata:
     """Data for the available thumbnails of a video"""
     def __init__(self, thumbnail_metadata: dict):
         """
         Args:
             thumbnail_metadata (dict): the raw thumbnail metadata to provide
@@ -46,100 +40,83 @@
 
     def __repr__(self):
         return f"YoutubeThumbnailMetadata(default={repr(self.default)},medium={repr(self.medium)}," \
                f"high={repr(self.high)},standard={repr(self.standard)},maxres={repr(self.maxres)})"
 
     @property
     def default(self) -> Optional[YoutubeThumbnail]:
-        """The default video thumbnail. Could be None.
+        """The default video thumbnail. The value is not guaranteed and could be `None`.
+        This is the most guaranteed to actually return a thumbnail
         Returns:
-            Optional[YoutubeThumbnail]: A YouTube thumbnail object. Could be None"""
+            Optional[YoutubeThumbnail]: A YouTube thumbnail object. Could be `None`"""
         if self.metadata.get("default") is not None:
-            return YoutubeThumbnail(self.metadata["default"])
+            return YoutubeThumbnail(**self.metadata["default"])
 
     @property
     def medium(self) -> Optional[YoutubeThumbnail]:
-        """The medium video thumbnail. Could be None
+        """The medium video thumbnail. The value is not guaranteed and could be `None`.
         Returns:
-            Optional[YoutubeThumbnail]: A YouTube thumbnail object. Could be None"""
+            Optional[YoutubeThumbnail]: A YouTube thumbnail object. Could be `None`"""
         if self.metadata.get("medium") is not None:
-            return YoutubeThumbnail(self.metadata["medium"])
+            return YoutubeThumbnail(**self.metadata["medium"])
 
     @property
     def high(self) -> Optional[YoutubeThumbnail]:
-        """The high video thumbnail. Could be None
+        """The high video thumbnail. The value is not guaranteed and could be `None`.
         Returns:
-            Optional[YoutubeThumbnail]: A YouTube thumbnail object. Could be None"""
+            Optional[YoutubeThumbnail]: A YouTube thumbnail object. Could be `None`"""
         if self.metadata.get("high") is not None:
-            return YoutubeThumbnail(self.metadata["high"])
+            return YoutubeThumbnail(**self.metadata["high"])
 
     @property
     def standard(self) -> Optional[YoutubeThumbnail]:
-        """The standard video thumbnail. Could be None
+        """The standard video thumbnail. The value is not guaranteed and could be `None`.
         Returns:
-            Optional[YoutubeThumbnail]: A YouTube thumbnail object. Could be None"""
+            Optional[YoutubeThumbnail]: A YouTube thumbnail object. Could be `None`"""
         if self.metadata.get("standard") is not None:
-            return YoutubeThumbnail(self.metadata["standard"])
+            return YoutubeThumbnail(**self.metadata["standard"])
 
     @property
     def maxres(self) -> Optional[YoutubeThumbnail]:
-        """The maximum resolution video thumbnail. Could be None
+        """The maximum resolution video thumbnail. The value is not guaranteed and could be `None`.
         Returns:
-            Optional[YoutubeThumbnail]: A YouTube thumbnail object. Could be None"""
+            Optional[YoutubeThumbnail]: A YouTube thumbnail object. Could be `None`"""
         if self.metadata.get("maxres") is not None:
-            return YoutubeThumbnail(self.metadata["maxres"])
-
+            return YoutubeThumbnail(**self.metadata["maxres"])
 
 
+@dataclass
 class LocalName:
     """Represents the video title and description in a local language if available
-    Attributes:
-        data (dict): The raw data associated with the local text
-        language (Optional[str]): The language code
-        title (str): The title in a local language
-        description (str): The description in a local language
+        Attributes:
+            language (Optional[str]): The language code
+            title (str): The title in a local language
+            description (str): The description in a local language
     """
-    def __init__(self, data: dict, lang_key: str = None):
-        """
-        Args:
-            data (dict): The raw local text data
-            lang_key (str): The language code
-        """
-        try:
-            self.data = data
-            self.language = lang_key
-            self.title: str = data["title"]
-            self.description: str = data["description"]
-        except KeyError as missing_snippet_data:
-            raise MissingDataFromMetadata(str(missing_snippet_data), data, missing_snippet_data)
+    title: str
+    description: str
+    language: str = None
 
 
+@dataclass
 class RegionRestrictions:
     """Represents information about the countries where a video is (or is not) viewable.
     Attributes:
-        data (dict): The raw data about what regions are blocked or allowed
-
-        allowed (Optional[list[str]]): The countries that are allowed to view the video. Could be None
-
-        blocked (Optional[list[str]]): The countries that are blocked from viewing the video. Could be None"""
-    def __init__(self, data: dict):
-        """
-        Args:
-            data (dict): The raw regionRestriction data
-        """
-        self.data = data
-        self.allowed: Optional[list[str]] = self.data.get("allowed")
-        self.blocked: Optional[list[str]] = self.data.get("blocked")
+        allowed (Optional[list[str]]): The countries that are allowed to view the video. Could be `None`
+        blocked (Optional[list[str]]): The countries that are blocked from viewing the video. Could be `None`
+    """
+    allowed: list[str] = None
+    blocked: list[str] = None
 
 
 class ContentRating:
     """Specifies the ratings that the video received under various rating schemes.
 
         There are many attributes for each rating system, only 1 or 2 (if there is a reason) will be available,
-        the rest will be None or all if there is no restrictions set.
+        the rest will be `None` or all if there is no restrictions set.
     Attributes:
         acb (Optional[str]): The video's Australian Classification Board (ACB) or Australian Communications and Media
             Authority (ACMA) rating. ACMA ratings are used to classify children's television programming.
         youtube (Optional[str]): A rating that YouTube uses to identify age-restricted content.
     """
     def __init__(self, data: dict):
         """
@@ -210,34 +187,25 @@
         self.skfilm: Optional[str] = data.get("skfilmRating")
         self.smais: Optional[str] = data.get("smaisRating")
         self.smsa: Optional[str] = data.get("smsaRating")
         self.tvpg: Optional[str] = data.get("tvpgRating")
         self.youtube: Optional[str] = data.get("ytRating")
 
 
+@dataclass
 class RecordingLocation:
     """The geolocation information associated with the video. if specified by the video uploader
     Attributes:
-        data (dict): The raw geolocation data used to construct this class
         latitude (float): Latitude in degrees.
         longitude (float): Longitude in degrees.
         altitude (float): Altitude above the reference ellipsoid, in meters.
     """
-    def __init__(self, data: dict):
-        """
-        Args:
-            data (dict): The raw geolocation data
-        """
-        try:
-            self.data = data
-            self.latitude: float = self.data["latitude"]
-            self.longitude: float = self.data["longitude"]
-            self.altitude: float = self.data["altitude"]
-        except KeyError as missing_snippet_data:
-            raise MissingDataFromMetadata(str(missing_snippet_data), data, missing_snippet_data)
+    latitude: float
+    longitude: float
+    altitude: float
 
 
 class RecordingDetails:
     """Contains details of the location and date of the video recording if specified by the video uploader.
     Attributes:
         data (dict): The raw information about the location, date and address where the video was recorded.
         description (Optional[str]): The text description of the location where the video was recorded.
@@ -250,15 +218,15 @@
             data (dict): The raw recording details used to construct this class
         """
         self.data = data
         self.description: Optional[str] = data.get("locationDescription")
         if data.get("location") is None:
             self.location: Optional[RecordingLocation] = None
         else:
-            self.location: Optional[RecordingLocation] = RecordingLocation(data["location"])
+            self.location: Optional[RecordingLocation] = RecordingLocation(**data["location"])
         if data.get("recordingDate") is None:
             self.date: Optional[datetime.datetime] = None
         else:
             self.date: Optional[datetime.datetime] = isodate.parse_datetime(data["recordingDate"])
 
 
 class VideoStream:
@@ -380,19 +348,44 @@
     def __str__(self):
         if self.category_restricts:
             return f'Tag Suggestion: "{self.tag}" with restrictions: {",".join(self.category_restricts)}'
         else:
             return f'Tag Suggestion: "{self.tag}"'
 
 
-class ABCVideoMetadata:
-    pass
+@dataclass
+class VideoChapter:
+    """
+    The start time, duration and name of a YouTube video chapter
+    Attributes:
+        start (int): the start time of the chapter in seconds
+        duration: (int): the length of the chapter in seconds
+        name (str): The name of the chapter
+    """
+    start: datetime.timedelta
+    duration: datetime.timedelta
+    name: str
+
+    def __str__(self):
+        return self.name
+
+
+@dataclass
+class BaseVideo:
+    metadata: dict
+    call_url: str
+    id: str
+    url: str
+    title: str
+    description: str
+    thumbnails = YoutubeThumbnailMetadata
+    visibility: Optional[str]
 
 
-class YoutubeVideoMetadata(ABCVideoMetadata):
+class YoutubeVideoMetadata(BaseVideo):
     """A data class containing video data such as the title, id, description, channel, etc.
         Attributes:
             metadata (dict): The raw API response used to construct this class
             call_url (str): The url used to call the API. Intended use is for debugging purposes
             id (str): The ID of the video. Example: "dQw4w9WgXcQ" from the url:
                 "https://www.youtube.com/watch?v=dQw4w9WgXcQ". Look familiar?
             snippet (dict): The raw snippet data used to construct part this class
@@ -423,15 +416,15 @@
             dimension (str): Indicates whether the video is available in 3D or in 2D
             definition (str): Indicates whether the video is available in high definition (HD) or only in standard
                 definition.
             has_captions (bool): Indicates whether captions are available for the video.
             licensed_content (bool): Indicates whether the video represents licensed content, which means that the
                 content was uploaded to a channel linked to a YouTube content partner and then claimed by that partner.
             region_restrictions (Optional[RegionRestrictions]): contains information about the countries where a video
-                is (or is not) viewable. Can be None
+                is (or is not) viewable. Can be `None`
             content_rating (ContentRating): Specifies the ratings that the video received under various rating schemes.
             age_restricted (bool): Whether the video is age restricted or not.
             projection (str): Specifies the projection format of the video. (example: 360 or rectangular)
             upload_status (str): The status of the uploaded video.
             failure_reason (str): Explains why a video failed to upload. This attribute is only present if
                 the upload_status attribute is set to "failed".
             rejection_reason (str): Explains why YouTube rejected an uploaded video. This attribute is only
@@ -443,20 +436,20 @@
             embeddable (bool): Indicates whether the video can be embedded on another website.
             public_stats_viewable (bool): Indicates whether the extended video statistics on the video's watch page are
                 publicly viewable.
             made_for_kids (bool): Indicates whether the video is designated as child-directed, and it contains the
                 current "made for kids" status of the video.
             view_count (int): The number of times the video has been viewed.
             like_count (Optional[int]): The number of users who have indicated that they liked the video.
-            comment_count (Optional[int]): The number of comments on the video. This attribute is None if disabled
+            comment_count (Optional[int]): The number of comments on the video. This attribute is `None` if disabled
             embed_html (Optional[str]): An <iframe> tag that embeds a player that plays the video.
             embed_height (Optional[str]): The height of the embedded player returned to the embed_html attribute.
-                Is None unless the height and aspect ratio is known
+                Is `None` unless the height and aspect ratio is known
             embed_width (Optional[str]): The width of the embedded player returned to the embed_html attribute.
-                Is None unless the width and aspect ratio is known
+                Is `None` unless the width and aspect ratio is known
             topic_categories (Optional[list[str]]): A list of Wikipedia URLs that provide a high-level description of
                 the video's content.
             recording_details (RecordingDetails): Encapsulates information about the location, date and address where
                 the video was recorded.
             stream_actual_start_time (Optional[datetime.datetime]): The time that the broadcast actually started.
             stream_scheduled_start_time (Optional[datetime.datetime]): The time that the broadcast is scheduled to
                 begin.
@@ -502,15 +495,15 @@
             self.tags: Optional[list[str]] = self.snippet.get("tags")
             self.category_id: int = int(self.snippet["categoryId"])
             self.live_broadcast_content: str = self.snippet["liveBroadcastContent"]
             self.default_language: Optional[str] = self.snippet.get("defaultLanguage")
             if self.snippet.get("localized") is None:
                 self.localized: Optional[LocalName] = None
             else:
-                self.localised: Optional[LocalName] = LocalName(self.snippet["localized"])
+                self.localised: Optional[LocalName] = LocalName(**self.snippet["localized"])
             self.localized = self.localised
             self.default_audio_language: Optional[str] = self.snippet.get("defaultAudioLanguage")
             self.duration = isodate.parse_duration(self.content_details["duration"])
             self.dimension: str = self.content_details["dimension"]
             self.definition: str = self.content_details["definition"]
             if self.content_details["caption"] == "true":
                 self.has_captions = True
@@ -519,15 +512,15 @@
             else:
                 self.has_captions = None
             self.licensed_content: bool = self.content_details["licensedContent"]
             if self.content_details.get("regionRestriction") is None:
                 self.region_restrictions: Optional[RegionRestrictions] = None
             else:
                 self.region_restrictions: Optional[RegionRestrictions] = \
-                    RegionRestrictions(self.content_details["regionRestriction"])
+                    RegionRestrictions(**self.content_details["regionRestriction"])
             self.content_rating = ContentRating(self.content_details["contentRating"])
             self.age_restricted = bool(self.content_rating.youtube)
             self.projection: Optional[str] = self.content_details.get("projection")
             self.upload_status: Optional[str] = self.status.get("uploadStatus")
             self.failure_reason: Optional[str] = self.status.get("failureReason")
             self.rejection_reason: Optional[str] = self.status.get("rejectionReason")
             self.visibility: str = self.status["privacyStatus"]
@@ -586,22 +579,64 @@
                     datetime.timedelta(
                         seconds=datetime.datetime.now().timestamp() - self.stream_actual_start_time.timestamp())
             if self.raw_localisations is None:
                 self.localisations: Optional[list[LocalName]] = None
             else:
                 self.localisations: Optional[list[LocalName]] = []
                 for localisation in self.raw_localisations.items():
-                    self.localisations.append(LocalName(localisation[1], localisation[0]))
+                    self.localisations.append(LocalName(**localisation[1], language=localisation[0]))
             self.localizations = self.localisations
 
         except KeyError as missing_snippet_data:
             raise MissingDataFromMetadata(str(missing_snippet_data), metadata, missing_snippet_data)
+        except TypeError as missing_snippet_data:
+            missing_str = f"{str(missing_snippet_data).split('arguments: ')[-1]} in " \
+                          f"{str(missing_snippet_data).split('.')[0]}"
+            raise MissingDataFromMetadata(missing_str, metadata, missing_snippet_data)
+
+    @property
+    def chapters(self) -> Optional[list[VideoChapter]]:
+        """A list of chapters the video has if any otherwise just an empty list
+        Returns:
+            chapters (list[VideoChapter]): A list of chapters the video has if any otherwise `None`
+        """
+        found_chapters = []
+        for line in reversed(self.description.splitlines()):
+            # regex is from https://stackoverflow.com/a/11067610
+            parsed = re.search(r'(?:([0-5]?[0-9]):)?([0-5]?[0-9]):([0-5][0-9])', line)
+            if parsed is not None:
+                raw_stamp = parsed.group()
+                split_timestamp = raw_stamp.split(":")
+                seconds = 0
+                for index, part in enumerate(reversed(split_timestamp)):
+                    seconds += int(part) * 60 ** index
+                start = datetime.timedelta(seconds=seconds)
+                end = found_chapters[-1][0] if len(found_chapters) > 0 else self.duration
+                duration = end - start
+                found_chapters.append((start, duration, line.replace(raw_stamp, "", 1).strip()))
+        return [VideoChapter(*chapter_data) for chapter_data in reversed(found_chapters)] if found_chapters else None
+
+    def current_chapter(self, position: datetime.timedelta) -> Optional[VideoChapter]:
+        """
+        Gets the current chapter based on the position provided
+        Args:
+            position (datetime.timedelta): The position of the video to get the current chapter from
+        Returns:
+            Optional[VideoChapter]: The current video chapter at that position of the video. Returns `None` if either
+                                    the video doesn't have any chapters or the position is greater than the duration of
+                                    the video or is negative
+        """
+        if self.chapters:
+            for idx, chapter in enumerate(self.chapters):
+                if chapter.start <= position < chapter.start + chapter.duration or \
+                        (idx+1 == len(self.chapters) and position == self.duration):
+                    return chapter
 
 
-class PlaylistVideoMetadata(ABCVideoMetadata):
+class PlaylistVideoMetadata(BaseVideo):
     """A data class for videos in a playlist
     Attributes:
         metadata (dict): The raw metadata from the API call used to construct this class
         call_url (str): The url used to call the API. Intended use is for debugging purposes
         id (str): The ID of the video in the playlist. Example: "dQw4w9WgXcQ" from the url:
             "https://www.youtube.com/watch?v=dQw4w9WgXcQ". Look familiar?
         position (int): The position in the playlist the video is in
@@ -694,15 +729,15 @@
         published_at (datetime.datetime): The date and time the playlist was published
         channel_id (Optional[str]): The id of the channel that created the playlist
         channel_url (Optional[str]): The url of the channel that created the playlist
         title (str): The title of the playlist
         description (str): The description of the playlist
         thumbnails (YoutubeThumbnailMetadata): The available thumbnails the playlist has
         channel_title: (Optional[str]) The name of the channel that created the playlist
-        default_language (Optional[str]): The default language the video is set in. Can be None
+        default_language (Optional[str]): The default language the video is set in. Can be `None`
         localised (Optional[LocalName]): The localised language of the title and description of the video
         localized (Optional[LocalName]): an alias of localised
         visibility (Optional[str]): The video's privacy status. Can be private, public or unlisted
         item_count (Optional[int]): The number of items in the playlist
         embed_html (Optional[str]): An <iframe> tag that embeds a player that plays the video.
         localisations (Optional[list[LocalName]]): contains translations of the video's metadata.
         localizations (Optional[list[LocalName]]): an alias of localisations
@@ -736,25 +771,25 @@
             self.description: str = self.snippet["description"]
             self.thumbnails = YoutubeThumbnailMetadata(self.snippet["thumbnails"])
             self.channel_title: Optional[str] = self.snippet.get("channelTitle")
             self.default_language: Optional[str] = self.snippet.get("defaultLanguage")
             if self.snippet.get("localized") is None:
                 self.localised: Optional[LocalName] = None
             else:
-                self.localised: Optional[LocalName] = LocalName(self.snippet["localized"])
+                self.localised: Optional[LocalName] = LocalName(**self.snippet["localized"])
                 self.localized = self.localised
             self.visibility: Optional[str] = self.status.get("privacyStatus")
             self.item_count: Optional[int] = self.content_details.get("itemCount")
             self.embed_html: Optional[str] = self.player.get("embedHtml")
             if self.raw_localisations is None:
                 self.localisations: Optional[list[LocalName]] = None
             else:
                 self.localisations: Optional[list[LocalName]] = []
                 for localisation_name, localisation_value in self.raw_localisations.items():
-                    self.localisations.append(LocalName(localisation_value, localisation_name))
+                    self.localisations.append(LocalName(**localisation_value, language=localisation_name))
             self.localizations = self.localisations
         except KeyError as missing_snippet_data:
             raise MissingDataFromMetadata(str(missing_snippet_data), metadata, missing_snippet_data)
 
     async def fetch_videos(self) -> list[PlaylistVideoMetadata]:
         """
         Fetches a list of the videos in the playlist
```

### Comparing `ayt-api-0.1.2/ayt_api.egg-info/PKG-INFO` & `ayt-api-0.1.3/ayt_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ayt-api
-Version: 0.1.2
+Version: 0.1.3
 Summary: An Asynchronous, Object oriented python library for the YouTube api
 Home-page: https://github.com/Revnoplex/ayt-api
 Author: Revnoplex
 Author-email: Revnoplex <revnoplex.business@protonmail.com>
 License: # MIT License
         
         Copyright (c) 2022-2023 Revnoplex
```

### Comparing `ayt-api-0.1.2/pyproject.toml` & `ayt-api-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ayt-api-0.1.2/setup.py` & `ayt-api-0.1.3/setup.py`

 * *Files identical despite different names*

