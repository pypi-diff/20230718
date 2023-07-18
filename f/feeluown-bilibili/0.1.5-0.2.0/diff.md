# Comparing `tmp/feeluown_bilibili-0.1.5.tar.gz` & `tmp/feeluown_bilibili-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feeluown_bilibili-0.1.5.tar", max compression
+gzip compressed data, was "feeluown_bilibili-0.2.0.tar", max compression
```

## Comparing `feeluown_bilibili-0.1.5.tar` & `feeluown_bilibili-0.2.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
--rw-r--r--   0        0        0    35149 2023-03-24 15:53:58.791133 feeluown_bilibili-0.1.5/LICENSE.txt
--rw-r--r--   0        0        0     1299 2023-03-24 15:53:58.791133 feeluown_bilibili-0.1.5/README.md
--rw-r--r--   0        0        0      805 2023-03-24 15:53:58.791133 feeluown_bilibili-0.1.5/fuo_bilibili/__init__.py
--rw-r--r--   0        0        0     5279 2023-03-24 15:53:58.791133 feeluown_bilibili-0.1.5/fuo_bilibili/api/__init__.py
--rw-r--r--   0        0        0     2381 2023-03-24 15:53:58.791133 feeluown_bilibili-0.1.5/fuo_bilibili/api/audio.py
--rw-r--r--   0        0        0     1735 2023-03-24 15:53:58.791133 feeluown_bilibili-0.1.5/fuo_bilibili/api/base.py
--rw-r--r--   0        0        0     1671 2023-03-24 15:53:58.791133 feeluown_bilibili-0.1.5/fuo_bilibili/api/history.py
--rw-r--r--   0        0        0     1194 2023-03-24 15:53:58.791133 feeluown_bilibili-0.1.5/fuo_bilibili/api/live.py
--rw-r--r--   0        0        0     3022 2023-03-24 15:53:58.791133 feeluown_bilibili-0.1.5/fuo_bilibili/api/login.py
--rw-r--r--   0        0        0     1117 2023-03-24 15:53:58.791133 feeluown_bilibili-0.1.5/fuo_bilibili/api/media.py
--rw-r--r--   0        0        0     2551 2023-03-24 15:53:58.791133 feeluown_bilibili-0.1.5/fuo_bilibili/api/playlist.py
--rw-r--r--   0        0        0        0 2023-03-24 15:53:58.791133 feeluown_bilibili-0.1.5/fuo_bilibili/api/schema/__init__.py
--rw-r--r--   0        0        0     3750 2023-03-24 15:53:58.791133 feeluown_bilibili-0.1.5/fuo_bilibili/api/schema/enums.py
--rw-r--r--   0        0        0     4469 2023-03-24 15:53:58.791133 feeluown_bilibili-0.1.5/fuo_bilibili/api/schema/requests.py
--rw-r--r--   0        0        0    26033 2023-03-24 15:53:58.791133 feeluown_bilibili-0.1.5/fuo_bilibili/api/schema/responses.py
--rw-r--r--   0        0        0     1729 2023-03-24 15:53:58.791133 feeluown_bilibili-0.1.5/fuo_bilibili/api/user.py
--rw-r--r--   0        0        0     2041 2023-03-24 15:53:58.791133 feeluown_bilibili-0.1.5/fuo_bilibili/api/video.py
--rw-r--r--   0        0        0     1840 2023-03-24 15:53:58.791133 feeluown_bilibili-0.1.5/fuo_bilibili/assets/icon.svg
--rw-r--r--   0        0        0      745 2023-03-24 15:53:58.791133 feeluown_bilibili-0.1.5/fuo_bilibili/const.py
--rw-r--r--   0        0        0    40663 2023-03-24 15:53:58.791133 feeluown_bilibili-0.1.5/fuo_bilibili/danmaku2ass.py
--rw-r--r--   0        0        0        0 2023-03-24 15:53:58.791133 feeluown_bilibili-0.1.5/fuo_bilibili/geetest/__init__.py
--rw-r--r--   0        0        0     7737 2023-03-24 15:53:58.791133 feeluown_bilibili-0.1.5/fuo_bilibili/geetest/index.html
--rw-r--r--   0        0        0     2155 2023-03-24 15:53:58.791133 feeluown_bilibili-0.1.5/fuo_bilibili/geetest/server.py
--rw-r--r--   0        0        0    17753 2023-03-24 15:53:58.791133 feeluown_bilibili-0.1.5/fuo_bilibili/model.py
--rw-r--r--   0        0        0     2571 2023-03-24 15:53:58.791133 feeluown_bilibili-0.1.5/fuo_bilibili/page_home.py
--rw-r--r--   0        0        0     1934 2023-03-24 15:53:58.791133 feeluown_bilibili-0.1.5/fuo_bilibili/page_ranking.py
--rw-r--r--   0        0        0    26611 2023-03-24 15:53:58.791133 feeluown_bilibili-0.1.5/fuo_bilibili/provider.py
--rw-r--r--   0        0        0    13933 2023-03-24 15:53:58.791133 feeluown_bilibili-0.1.5/fuo_bilibili/ui.py
--rw-r--r--   0        0        0     1594 2023-03-24 15:53:58.791133 feeluown_bilibili-0.1.5/fuo_bilibili/util.py
--rw-r--r--   0        0        0      832 2023-03-24 15:53:58.791133 feeluown_bilibili-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2285 1970-01-01 00:00:00.000000 feeluown_bilibili-0.1.5/setup.py
--rw-r--r--   0        0        0     1963 1970-01-01 00:00:00.000000 feeluown_bilibili-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-18 16:44:26.676485 feeluown_bilibili-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     1329 2023-07-18 16:44:26.676485 feeluown_bilibili-0.2.0/README.md
+-rw-r--r--   0        0        0      805 2023-07-18 16:44:26.680485 feeluown_bilibili-0.2.0/fuo_bilibili/__init__.py
+-rw-r--r--   0        0        0     5278 2023-07-18 16:44:26.680485 feeluown_bilibili-0.2.0/fuo_bilibili/api/__init__.py
+-rw-r--r--   0        0        0     2380 2023-07-18 16:44:26.680485 feeluown_bilibili-0.2.0/fuo_bilibili/api/audio.py
+-rw-r--r--   0        0        0     1734 2023-07-18 16:44:26.680485 feeluown_bilibili-0.2.0/fuo_bilibili/api/base.py
+-rw-r--r--   0        0        0       60 2023-07-18 16:44:26.680485 feeluown_bilibili-0.2.0/fuo_bilibili/api/compat.py
+-rw-r--r--   0        0        0     1670 2023-07-18 16:44:26.680485 feeluown_bilibili-0.2.0/fuo_bilibili/api/history.py
+-rw-r--r--   0        0        0     1193 2023-07-18 16:44:26.680485 feeluown_bilibili-0.2.0/fuo_bilibili/api/live.py
+-rw-r--r--   0        0        0     3013 2023-07-18 16:44:26.680485 feeluown_bilibili-0.2.0/fuo_bilibili/api/login.py
+-rw-r--r--   0        0        0     1116 2023-07-18 16:44:26.680485 feeluown_bilibili-0.2.0/fuo_bilibili/api/media.py
+-rw-r--r--   0        0        0     2550 2023-07-18 16:44:26.680485 feeluown_bilibili-0.2.0/fuo_bilibili/api/playlist.py
+-rw-r--r--   0        0        0        0 2023-07-18 16:44:26.680485 feeluown_bilibili-0.2.0/fuo_bilibili/api/schema/__init__.py
+-rw-r--r--   0        0        0     3750 2023-07-18 16:44:26.680485 feeluown_bilibili-0.2.0/fuo_bilibili/api/schema/enums.py
+-rw-r--r--   0        0        0     4484 2023-07-18 16:44:26.680485 feeluown_bilibili-0.2.0/fuo_bilibili/api/schema/requests.py
+-rw-r--r--   0        0        0    26049 2023-07-18 16:44:26.680485 feeluown_bilibili-0.2.0/fuo_bilibili/api/schema/responses.py
+-rw-r--r--   0        0        0     1728 2023-07-18 16:44:26.680485 feeluown_bilibili-0.2.0/fuo_bilibili/api/user.py
+-rw-r--r--   0        0        0     2041 2023-07-18 16:44:26.680485 feeluown_bilibili-0.2.0/fuo_bilibili/api/video.py
+-rw-r--r--   0        0        0     1840 2023-07-18 16:44:26.680485 feeluown_bilibili-0.2.0/fuo_bilibili/assets/icon.svg
+-rw-r--r--   0        0        0      745 2023-07-18 16:44:26.680485 feeluown_bilibili-0.2.0/fuo_bilibili/const.py
+-rw-r--r--   0        0        0    40663 2023-07-18 16:44:26.680485 feeluown_bilibili-0.2.0/fuo_bilibili/danmaku2ass.py
+-rw-r--r--   0        0        0        0 2023-07-18 16:44:26.680485 feeluown_bilibili-0.2.0/fuo_bilibili/geetest/__init__.py
+-rw-r--r--   0        0        0     7737 2023-07-18 16:44:26.680485 feeluown_bilibili-0.2.0/fuo_bilibili/geetest/index.html
+-rw-r--r--   0        0        0     2155 2023-07-18 16:44:26.680485 feeluown_bilibili-0.2.0/fuo_bilibili/geetest/server.py
+-rw-r--r--   0        0        0    17672 2023-07-18 16:44:26.680485 feeluown_bilibili-0.2.0/fuo_bilibili/model.py
+-rw-r--r--   0        0        0     2571 2023-07-18 16:44:26.680485 feeluown_bilibili-0.2.0/fuo_bilibili/page_home.py
+-rw-r--r--   0        0        0     1934 2023-07-18 16:44:26.680485 feeluown_bilibili-0.2.0/fuo_bilibili/page_ranking.py
+-rw-r--r--   0        0        0    26610 2023-07-18 16:44:26.680485 feeluown_bilibili-0.2.0/fuo_bilibili/provider.py
+-rw-r--r--   0        0        0    13933 2023-07-18 16:44:26.680485 feeluown_bilibili-0.2.0/fuo_bilibili/ui.py
+-rw-r--r--   0        0        0     1586 2023-07-18 16:44:26.680485 feeluown_bilibili-0.2.0/fuo_bilibili/util.py
+-rw-r--r--   0        0        0      784 2023-07-18 16:44:26.680485 feeluown_bilibili-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2315 1970-01-01 00:00:00.000000 feeluown_bilibili-0.2.0/setup.py
+-rw-r--r--   0        0        0     1992 1970-01-01 00:00:00.000000 feeluown_bilibili-0.2.0/PKG-INFO
```

### Comparing `feeluown_bilibili-0.1.5/LICENSE.txt` & `feeluown_bilibili-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `feeluown_bilibili-0.1.5/README.md` & `feeluown_bilibili-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 yay -S feeluown-bilibili
 ```
 
 ## Development
 
 ```shell
 poetry install
+poetry run pre-commit install
 ```
 
 ## License
 
 [GPL-3.0](https://github.com/BruceZhang1993/feeluown-bilibili/blob/master/LICENSE.txt)
 
 ## Special notes
```

### Comparing `feeluown_bilibili-0.1.5/fuo_bilibili/__init__.py` & `feeluown_bilibili-0.2.0/fuo_bilibili/__init__.py`

 * *Files identical despite different names*

### Comparing `feeluown_bilibili-0.1.5/fuo_bilibili/api/__init__.py` & `feeluown_bilibili-0.2.0/fuo_bilibili/api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 from datetime import timedelta
 from http.cookiejar import MozillaCookieJar
 from typing import Type, Optional, Union, List
 
 import requests.cookies
 from cachetools import TTLCache, cached
-from pydantic import BaseModel
+from .compat import BaseModel
 
 from fuo_bilibili.api.audio import AudioMixin
 from fuo_bilibili.api.base import BaseMixin
 from fuo_bilibili.api.history import HistoryMixin
 from fuo_bilibili.api.live import LiveMixin
 from fuo_bilibili.api.login import LoginMixin
 from fuo_bilibili.api.media import MediaMixin
```

### Comparing `feeluown_bilibili-0.1.5/fuo_bilibili/api/audio.py` & `feeluown_bilibili-0.2.0/fuo_bilibili/api/audio.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Type, Any, Optional, Union
 
-from pydantic import BaseModel
+from .compat import BaseModel
 
 from fuo_bilibili.api.schema.requests import BaseRequest, PaginatedRequest, AudioFavoriteSongsRequest, \
     AudioGetUrlRequest
 from fuo_bilibili.api.schema.responses import BaseResponse, AudioFavoriteListResponse, AudioFavoriteSongsResponse, \
     AudioFavoriteInfoResponse, AudioGetUrlResponse
```

### Comparing `feeluown_bilibili-0.1.5/fuo_bilibili/api/base.py` & `feeluown_bilibili-0.2.0/fuo_bilibili/api/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Type, Any, Optional, Union
 
-from pydantic import BaseModel
+from .compat import BaseModel
 
 from fuo_bilibili.api.schema.requests import SearchRequest, BaseRequest, PaginatedRequest, HomeRecommendVideosRequest, \
     HomeDynamicVideoRequest
 from fuo_bilibili.api.schema.responses import SearchResponse, BaseResponse, NavInfoResponse, \
     HomeRecommendVideosResponse, HomeDynamicVideoResponse
```

### Comparing `feeluown_bilibili-0.1.5/fuo_bilibili/api/history.py` & `feeluown_bilibili-0.2.0/fuo_bilibili/api/history.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Type, Any, Optional, Union, List
 
-from pydantic import BaseModel
+from .compat import BaseModel
 
 from fuo_bilibili.api.schema.requests import BaseRequest, PaginatedRequest, HistoryAddLaterVideosRequest, \
     HistoryDelLaterVideosRequest
 from fuo_bilibili.api.schema.responses import BaseResponse, HistoryLaterVideoResponse, HistoryVideoResponse
 
 
 class HistoryMixin:
```

### Comparing `feeluown_bilibili-0.1.5/fuo_bilibili/api/live.py` & `feeluown_bilibili-0.2.0/fuo_bilibili/api/live.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Type, Any, Optional, Union
 
-from pydantic import BaseModel
+from .compat import BaseModel
 
 from fuo_bilibili.api.schema.requests import BaseRequest, AnotherPaginatedRequest, LivePlayUrlRequest
 from fuo_bilibili.api.schema.responses import BaseResponse, LiveFeedListResponse, LivePlayUrlResponse
 
 
 class LiveMixin:
     API_LIVE_BASE = 'https://api.live.bilibili.com'
```

### Comparing `feeluown_bilibili-0.1.5/fuo_bilibili/api/login.py` & `feeluown_bilibili-0.2.0/fuo_bilibili/api/login.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Type, Any, Optional, Union
 
-from pydantic import BaseModel
+from .compat import BaseModel
 
 from fuo_bilibili.api.schema.requests import BaseRequest, PasswordLoginRequest, SendSmsCodeRequest, \
     SmsCodeLoginRequest
 from fuo_bilibili.api.schema.responses import BaseResponse, RequestCaptchaResponse, \
     RequestLoginKeyResponse, PasswordLoginResponse, SendSmsCodeResponse, SmsCodeLoginResponse
 
 
@@ -23,19 +23,19 @@
     def post(self, url: str, param: Optional[BaseRequest], clazz: Type[BaseResponse], is_json=False, **kwargs) -> Any:
         pass
 
     def _dump_cookie_to_file(self):
         pass
 
     def request_captcha(self) -> RequestCaptchaResponse:
-        url = f'{self.PASSPORT_BASE}/x/passport-login/captcha?source=main_web'
+        url = f'{self.PASSPORT_BASE}/x/passport-login/captcha'
         return self.get_uncached(url, None, RequestCaptchaResponse)
 
     def request_login_key(self) -> RequestLoginKeyResponse:
-        url = f'{self.PASSPORT_BASE}/login?act=getkey'
+        url = f'{self.PASSPORT_BASE}/x/passport-login/web/key'
         response: RequestLoginKeyResponse = self.get_uncached(url, None, RequestLoginKeyResponse)
         # 接口没有状态码 pydantic 判断字段存在 根据字段是否空判断
         if response.key == '' or response.hash == '':
             raise RuntimeError('getkey error')
         return response
 
     def send_sms_code(self, request: SendSmsCodeRequest) -> SendSmsCodeResponse:
```

### Comparing `feeluown_bilibili-0.1.5/fuo_bilibili/api/media.py` & `feeluown_bilibili-0.2.0/fuo_bilibili/api/media.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Type, Any, Optional, Union
 
-from pydantic import BaseModel
+from .compat import BaseModel
 
 from fuo_bilibili.api.schema.requests import BaseRequest, MediaGetListRequest, MediaFavlistRequest
 from fuo_bilibili.api.schema.responses import BaseResponse, MediaGetListResponse, MediaFavlistResponse
 
 
 class MediaMixin:
     API_PGC_BASE = 'https://api.bilibili.com/pgc'
```

### Comparing `feeluown_bilibili-0.1.5/fuo_bilibili/api/playlist.py` & `feeluown_bilibili-0.2.0/fuo_bilibili/api/playlist.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Type, Any, Optional, Union, List
 
-from pydantic import BaseModel
+from .compat import BaseModel
 
 from fuo_bilibili.api.schema.requests import BaseRequest, FavoriteListRequest, FavoriteInfoRequest, \
     FavoriteResourceRequest, CollectedFavoriteListRequest, FavoriteSeasonResourceRequest, \
     FavoriteResourceOperateRequest, FavoriteNewRequest
 from fuo_bilibili.api.schema.responses import BaseResponse, FavoriteListResponse, FavoriteInfoResponse, \
     FavoriteResourceResponse, CollectedFavoriteListResponse, FavoriteSeasonResourceResponse
```

### Comparing `feeluown_bilibili-0.1.5/fuo_bilibili/api/schema/enums.py` & `feeluown_bilibili-0.2.0/fuo_bilibili/api/schema/enums.py`

 * *Files identical despite different names*

### Comparing `feeluown_bilibili-0.1.5/fuo_bilibili/api/schema/requests.py` & `feeluown_bilibili-0.2.0/fuo_bilibili/api/schema/requests.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pydantic import BaseModel, Field
+from fuo_bilibili.api.compat import BaseModel, Field
 
 from fuo_bilibili.api.schema.enums import VideoQualityNum, VideoFnval, SearchType, SearchOrderType, UserType, \
     VideoDurationType, FavoriteResourceOrderType, CommentType
 
 
 class BaseRequest(BaseModel):
     def __hash__(self):
```

### Comparing `feeluown_bilibili-0.1.5/fuo_bilibili/api/schema/responses.py` & `feeluown_bilibili-0.2.0/fuo_bilibili/api/schema/responses.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from datetime import datetime, timedelta
 from typing import Any, List, Union
 
-from pydantic import BaseModel, validator, Field
+from fuo_bilibili.api.compat import BaseModel, validator, Field
 
 from fuo_bilibili.api.schema.enums import VideoQualityNum, CodecId, VideoCopyright, VideoState, VideoFrom, SearchType, \
     VipType, MediaType
 
 
 class BaseResponse(BaseModel):
     code: int = None
@@ -994,8 +994,8 @@
             first_frame: str
             pub_location: str
             bvid: str
             rcmd_reason: str
 
         list: List[WeeklyDetail]
 
-    data: WeeklyDetailResponseData = None
+    data: WeeklyDetailResponseData = None
```

### Comparing `feeluown_bilibili-0.1.5/fuo_bilibili/api/user.py` & `feeluown_bilibili-0.2.0/fuo_bilibili/api/user.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Type, Any, Optional, Union
 
-from pydantic import BaseModel
+from .compat import BaseModel
 
 from fuo_bilibili.api.schema.requests import BaseRequest, UserInfoRequest, UserBestVideoRequest, UserVideoRequest, \
     UserFollowingRequest
 from fuo_bilibili.api.schema.responses import BaseResponse, UserInfoResponse, UserBestVideoResponse, UserVideoResponse, \
     UserFollowingResponse
```

### Comparing `feeluown_bilibili-0.1.5/fuo_bilibili/api/video.py` & `feeluown_bilibili-0.2.0/fuo_bilibili/api/video.py`

 * *Files identical despite different names*

### Comparing `feeluown_bilibili-0.1.5/fuo_bilibili/assets/icon.svg` & `feeluown_bilibili-0.2.0/fuo_bilibili/assets/icon.svg`

 * *Files identical despite different names*

### Comparing `feeluown_bilibili-0.1.5/fuo_bilibili/const.py` & `feeluown_bilibili-0.2.0/fuo_bilibili/const.py`

 * *Files identical despite different names*

### Comparing `feeluown_bilibili-0.1.5/fuo_bilibili/danmaku2ass.py` & `feeluown_bilibili-0.2.0/fuo_bilibili/danmaku2ass.py`

 * *Files identical despite different names*

### Comparing `feeluown_bilibili-0.1.5/fuo_bilibili/geetest/index.html` & `feeluown_bilibili-0.2.0/fuo_bilibili/geetest/index.html`

 * *Files identical despite different names*

### Comparing `feeluown_bilibili-0.1.5/fuo_bilibili/geetest/server.py` & `feeluown_bilibili-0.2.0/fuo_bilibili/geetest/server.py`

 * *Files identical despite different names*

### Comparing `feeluown_bilibili-0.1.5/fuo_bilibili/model.py` & `feeluown_bilibili-0.2.0/fuo_bilibili/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List, Union, Optional, Tuple
 
 from bs4 import BeautifulSoup
 from feeluown.library import SongModel, BriefArtistModel, PlaylistModel, BriefPlaylistModel, BriefUserModel, \
-    BriefSongModel, ArtistModel, CommentModel, VideoModel, BriefVideoModel, BriefAlbumModel, AlbumModel
-from feeluown.models import SearchModel, ModelExistence
+    BriefSongModel, ArtistModel, CommentModel, VideoModel, BriefVideoModel, BriefAlbumModel, AlbumModel, \
+    SimpleSearchResult
 
 from fuo_bilibili import __identifier__
 from fuo_bilibili.api import SearchType
 from fuo_bilibili.api.schema.requests import SearchRequest
 from fuo_bilibili.api.schema.responses import SearchResponse, SearchResultVideo, VideoInfoResponse, \
     FavoriteListResponse, FavoriteInfoResponse, FavoriteResourceResponse, CollectedFavoriteListResponse, \
     FavoriteSeasonResourceResponse, HistoryLaterVideoResponse, HomeDynamicVideoResponse, UserInfoResponse, \
@@ -44,14 +44,15 @@
             artists=[BriefArtistModel(
                 source=PROVIDER_ID,
                 identifier=au.uid,
                 name=au.author,
             )],
             duration=au.duration.total_seconds() * 1000,
             lyric=au.lyric,
+            pic_url=au.cover,
         )
 
     @classmethod
     def create_user_brief_model(cls, media: UserVideoResponse.UserVideoResponseData.RList.Video):
         return BriefSongModel(
             source=__identifier__,
             identifier=media.bvid,
@@ -75,14 +76,15 @@
             title=BeautifulSoup(item.title).get_text(),
             artists=[BriefArtistModel(
                 source=PROVIDER_ID,
                 identifier=item.owner.mid,
                 name=item.owner.name,
             )],
             duration=item.duration.total_seconds() * 1000,
+            pic_url=item.pic,
         )
 
     @classmethod
     def create_dynamic_brief_model(cls, item: HomeDynamicVideoResponse.HomeDynamicVideoResponseData.DynamicVideoItem):
         media = item.modules.module_dynamic.major.archive
         author = item.modules.module_author
         return BriefSongModel(
@@ -118,14 +120,15 @@
             title=BeautifulSoup(result.title).get_text(),
             artists=[BriefArtistModel(
                 source=PROVIDER_ID,
                 identifier=result.mid,
                 name=result.author,
             )],
             duration=result.duration.total_seconds() * 1000,
+            pic_url=result.pic,
         )
 
     @classmethod
     def create_info_model(cls, response: VideoInfoResponse) -> 'BSongModel':
         result = response.data
         lrc = None
         if result.subtitle.list is not None and len(result.subtitle.list) > 0:
@@ -143,16 +146,16 @@
             title=result.title,
             artists=[BriefArtistModel(
                 source=PROVIDER_ID,
                 identifier=result.owner.mid,
                 name=result.owner.name,
             )],
             duration=result.duration.total_seconds() * 1000,
-            lyric=lrc,
-            exists=ModelExistence.yes,
+            lyric=lrc or '',
+            pic_url=result.pic,
         )
 
     @classmethod
     def create_history_brief_model(cls, media):
         return BriefSongModel(
             source=__identifier__,
             identifier=media.bvid,
@@ -196,17 +199,15 @@
             artists=[],
             songs=[cls.create_episode_song_model(ep, media) for ep in media.episodes],
             cover=media.cover.replace('http://', 'https://'),
             description=media.evaluate,
         )
 
 
-class BSearchModel(SearchModel):
-    PROVIDER_ID = __identifier__
-
+class BSearchModel:
     # ['q', 'songs', 'playlists', 'artists', 'albums', 'videos']
     q: str
     songs = List[BSongModel]
 
     @staticmethod
     def search_user_model(user: SearchResultUser):
         return BriefArtistModel(
@@ -262,27 +263,24 @@
                 songs = list(map(lambda r_: BSongModel.create_model(r_), results))
             case SearchType.BILI_USER:
                 artists = list(map(cls.search_user_model, results))
             case SearchType.LIVE_ROOM:
                 videos = list(map(cls.search_live_model, results))
             case SearchType.BANGUMI:
                 albums = list(map(cls.search_media_model, results))
-        return cls(
-            source=PROVIDER_ID,
+        return SimpleSearchResult(
             q=request[0].keyword if isinstance(request, Tuple) else request.keyword,
-            songs=songs,
-            artists=artists,
-            videos=videos,
-            albums=albums,
+            songs=songs or [],
+            artists=artists or [],
+            videos=videos or [],
+            albums=albums or [],
         )
 
 
 class BPlaylistModel(PlaylistModel):
-    PROVIDER_ID = __identifier__
-
     count: int
 
     @classmethod
     def create_audio_model(cls, p: AudioPlaylist):
         identifier = None
         desc = ''
         count = 0
@@ -442,16 +440,14 @@
 
     @classmethod
     def create_model_list(cls, response: Union[FavoriteListResponse, CollectedFavoriteListResponse]):
         return [cls.create_brief_model(f) for f in response.data.list]
 
 
 class BArtistModel(ArtistModel):
-    PROVIDER_ID = __identifier__
-
     @classmethod
     def create_model(cls, resp: UserInfoResponse, video_resp: UserBestVideoResponse) -> 'BArtistModel':
         alias = []
         if resp.data.fans_badge and resp.data.fans_medal.show and resp.data.fans_medal.wear \
                 and resp.data.fans_medal.medal is not None:
             alias.append(f'Lv{resp.data.fans_medal.medal.level} {resp.data.fans_medal.medal.medal_name}')
         return cls(
@@ -462,16 +458,14 @@
             aliases=alias,
             hot_songs=[BSongModel.create_hot_model(v) for v in video_resp.data],
             description=resp.data.sign
         )
 
 
 class BCommentModel(CommentModel):
-    PROVIDER_ID = __identifier__
-
     @classmethod
     def create_model(cls, reply: VideoHotCommentsResponse.VideoHotCommentsResponseData.Reply):
         return cls(
             source=PROVIDER_ID,
             identifier=str(reply.rpid),
             user=BriefUserModel(
                 source=PROVIDER_ID,
```

### Comparing `feeluown_bilibili-0.1.5/fuo_bilibili/page_home.py` & `feeluown_bilibili-0.2.0/fuo_bilibili/page_home.py`

 * *Files identical despite different names*

### Comparing `feeluown_bilibili-0.1.5/fuo_bilibili/page_ranking.py` & `feeluown_bilibili-0.2.0/fuo_bilibili/page_ranking.py`

 * *Files identical despite different names*

### Comparing `feeluown_bilibili-0.1.5/fuo_bilibili/provider.py` & `feeluown_bilibili-0.2.0/fuo_bilibili/provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 from time import time
 from typing import List, Optional, Union, Tuple
 
 from feeluown.excs import NoUserLoggedIn
 from feeluown.library import AbstractProvider, ProviderV2, ProviderFlags as Pf, UserModel, VideoModel, \
     BriefPlaylistModel, BriefSongModel, LyricModel, SupportsSongSimilar, BriefSongProtocol, SupportsSongHotComments, \
     SupportsAlbumGet, BriefAlbumModel, SupportsPlaylistAddSong, SupportsPlaylistRemoveSong, BriefUserModel, \
-    BriefArtistModel
+    BriefArtistModel, SearchType as FuoSearchType, ModelType, SimpleSearchResult
 from feeluown.media import Quality, Media, MediaType, VideoAudioManifest
-from feeluown.models import SearchType as FuoSearchType, ModelType
 from feeluown.utils.reader import SequentialReader
 
 from fuo_bilibili import __identifier__, __alias__
 from fuo_bilibili.api import BilibiliApi, SearchRequest, SearchType as BilibiliSearchType, VideoInfoRequest, \
     PlayUrlRequest, VideoQualityNum
 from fuo_bilibili.api.schema.enums import VideoFnval, CommentType
 from fuo_bilibili.api.schema.requests import PasswordLoginRequest, SendSmsCodeRequest, SmsCodeLoginRequest, \
@@ -144,15 +143,15 @@
 
     def password_login(self, request: PasswordLoginRequest) -> PasswordLoginResponse:
         return self._api.password_login(request)
 
     def sms_code_login(self, request: SmsCodeLoginRequest) -> SmsCodeLoginResponse:
         return self._api.sms_code_login(request)
 
-    def search(self, keyword, type_, *args, **kwargs) -> Optional[BSearchModel]:
+    def search(self, keyword, type_, *args, **kwargs) -> Optional[SimpleSearchResult]:
         request = self._format_search_request(keyword, type_)
         if isinstance(request, Tuple):
             response = tuple([self._api.search(r) for r in request])
         else:
             response = self._api.search(request)
         return BSearchModel.create_model(request, response)
```

### Comparing `feeluown_bilibili-0.1.5/fuo_bilibili/ui.py` & `feeluown_bilibili-0.2.0/fuo_bilibili/ui.py`

 * *Files identical despite different names*

### Comparing `feeluown_bilibili-0.1.5/fuo_bilibili/util.py` & `feeluown_bilibili-0.2.0/fuo_bilibili/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     """
     RSA公钥加密
     :param text:
     :param public_key:
     :return:
     """
     import base64
-    from Cryptodome.PublicKey import RSA
-    from Cryptodome.Cipher import PKCS1_v1_5
+    from Crypto.PublicKey import RSA
+    from Crypto.Cipher import PKCS1_v1_5
     key = RSA.import_key(public_key.encode())
     encrypted = PKCS1_v1_5.new(key).encrypt(text.encode())
     return base64.b64encode(encrypted).decode()
 
 
 def format_timedelta_to_hms(td: timedelta) -> str:
     ss = int(td.total_seconds())
```

### Comparing `feeluown_bilibili-0.1.5/pyproject.toml` & `feeluown_bilibili-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 [tool.poetry]
 name = "feeluown-bilibili"
-version = "0.1.5"
+version = "0.2.0"
 description = "Bilibili provider for FeelUOwn player."
 homepage = "https://github.com/BruceZhang1993/feeluown-bilibili"
 authors = ["Bruce Zhang <zttt183525594@gmail.com>"]
 packages = [{ include = "fuo_bilibili" }]
 include = ["fuo_bilibili/assets/icon.svg", "fuo_bilibili/geetest/index.html"]
 license = "GPL-3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 feeluown = ">=3.8.7"
 cachetools = "*"
 beautifulsoup4 = "*"
-pycryptodomex = "*"
+pycryptodome = "*"
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
 PyQt5 = "*"
 fuo-dl = "^0.3"
-feeluown = { git = "https://github.com/feeluown/FeelUOwn.git", branch = "master" }
+pre-commit = "*"
+poetry2setup = "*"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."fuo.plugins_v1"]
 "bilibili" = "fuo_bilibili"
```

### Comparing `feeluown_bilibili-0.1.5/setup.py` & `feeluown_bilibili-0.2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,24 +7,24 @@
  'fuo_bilibili.api.schema',
  'fuo_bilibili.geetest']
 
 package_data = \
 {'': ['*'], 'fuo_bilibili': ['assets/*']}
 
 install_requires = \
-['beautifulsoup4', 'cachetools', 'feeluown>=3.8.7', 'pycryptodomex']
+['beautifulsoup4', 'cachetools', 'feeluown>=3.8.7', 'pycryptodome']
 
 entry_points = \
 {'fuo.plugins_v1': ['bilibili = fuo_bilibili']}
 
 setup_kwargs = {
     'name': 'feeluown-bilibili',
-    'version': '0.1.5',
+    'version': '0.2.0',
     'description': 'Bilibili provider for FeelUOwn player.',
-    'long_description': '# Yet another bilibili plugin for FeelUOwn player\n\n![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/brucezhang1993/feeluown-bilibili/build.yml?style=for-the-badge)\n![AUR version](https://img.shields.io/aur/version/feeluown-bilibili?style=for-the-badge)\n![PyPI](https://img.shields.io/pypi/v/feeluown_bilibili?style=for-the-badge)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/feeluown_bilibili?style=for-the-badge)\n![Libraries.io dependency status for GitHub repo](https://img.shields.io/librariesio/github/brucezhang1993/feeluown-bilibili?style=for-the-badge)\n\n## Prerequisite\n\nYou must have [FeelUOwn](https://github.com/feeluown/FeelUOwn) first\n\n- Python >= 3.10  \n- FeelUOwn >= 3.8.7\n\n## Installation\n\n### PyPI\n\nhttps://pypi.org/project/feeluown-bilibili/\n\n```shell\npip install feeluown-bilibili\n```\n\n### Arch Linux\n\nhttps://aur.archlinux.org/packages/feeluown-bilibili\n\n```shell\nyay -S feeluown-bilibili\n```\n\n## Development\n\n```shell\npoetry install\n```\n\n## License\n\n[GPL-3.0](https://github.com/BruceZhang1993/feeluown-bilibili/blob/master/LICENSE.txt)\n\n## Special notes\n\n- Proudly use [danmaku2ass](https://github.com/m13253/danmaku2ass) to transform danmaku format\n- Proudly use [poetry](https://python-poetry.org/) as dependency manager tool\n',
+    'long_description': '# Yet another bilibili plugin for FeelUOwn player\n\n![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/brucezhang1993/feeluown-bilibili/build.yml?style=for-the-badge)\n![AUR version](https://img.shields.io/aur/version/feeluown-bilibili?style=for-the-badge)\n![PyPI](https://img.shields.io/pypi/v/feeluown_bilibili?style=for-the-badge)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/feeluown_bilibili?style=for-the-badge)\n![Libraries.io dependency status for GitHub repo](https://img.shields.io/librariesio/github/brucezhang1993/feeluown-bilibili?style=for-the-badge)\n\n## Prerequisite\n\nYou must have [FeelUOwn](https://github.com/feeluown/FeelUOwn) first\n\n- Python >= 3.10  \n- FeelUOwn >= 3.8.7\n\n## Installation\n\n### PyPI\n\nhttps://pypi.org/project/feeluown-bilibili/\n\n```shell\npip install feeluown-bilibili\n```\n\n### Arch Linux\n\nhttps://aur.archlinux.org/packages/feeluown-bilibili\n\n```shell\nyay -S feeluown-bilibili\n```\n\n## Development\n\n```shell\npoetry install\npoetry run pre-commit install\n```\n\n## License\n\n[GPL-3.0](https://github.com/BruceZhang1993/feeluown-bilibili/blob/master/LICENSE.txt)\n\n## Special notes\n\n- Proudly use [danmaku2ass](https://github.com/m13253/danmaku2ass) to transform danmaku format\n- Proudly use [poetry](https://python-poetry.org/) as dependency manager tool\n',
     'author': 'Bruce Zhang',
     'author_email': 'zttt183525594@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/BruceZhang1993/feeluown-bilibili',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `feeluown_bilibili-0.1.5/PKG-INFO` & `feeluown_bilibili-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: feeluown-bilibili
-Version: 0.1.5
+Version: 0.2.0
 Summary: Bilibili provider for FeelUOwn player.
 Home-page: https://github.com/BruceZhang1993/feeluown-bilibili
 License: GPL-3.0
 Author: Bruce Zhang
 Author-email: zttt183525594@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4
 Requires-Dist: cachetools
 Requires-Dist: feeluown (>=3.8.7)
-Requires-Dist: pycryptodomex
+Requires-Dist: pycryptodome
 Description-Content-Type: text/markdown
 
 # Yet another bilibili plugin for FeelUOwn player
 
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/brucezhang1993/feeluown-bilibili/build.yml?style=for-the-badge)
 ![AUR version](https://img.shields.io/aur/version/feeluown-bilibili?style=for-the-badge)
 ![PyPI](https://img.shields.io/pypi/v/feeluown_bilibili?style=for-the-badge)
@@ -50,14 +50,15 @@
 yay -S feeluown-bilibili
 ```
 
 ## Development
 
 ```shell
 poetry install
+poetry run pre-commit install
 ```
 
 ## License
 
 [GPL-3.0](https://github.com/BruceZhang1993/feeluown-bilibili/blob/master/LICENSE.txt)
 
 ## Special notes
```

