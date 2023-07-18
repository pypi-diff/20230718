# Comparing `tmp/threads_py-0.0.8.tar.gz` & `tmp/threads_py-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threads_py-0.0.8.tar", max compression
+gzip compressed data, was "threads_py-0.0.9.tar", max compression
```

## Comparing `threads_py-0.0.8.tar` & `threads_py-0.0.9.tar`

### file list

```diff
@@ -1,40 +1,42 @@
--rw-r--r--   0        0        0     1066 2023-07-16 04:06:05.352298 threads_py-0.0.8/LICENSE
--rw-r--r--   0        0        0     5016 2023-07-16 13:38:52.326551 threads_py-0.0.8/README.md
--rw-r--r--   0        0        0      783 2023-07-16 13:38:50.963547 threads_py-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      117 2023-07-16 13:38:44.023233 threads_py-0.0.8/threadspy/__init__.py
--rw-r--r--   0        0        0       58 2023-07-16 12:39:36.364575 threads_py-0.0.8/threadspy/ai/__init__.py
--rw-r--r--   0        0        0     5537 2023-07-16 12:39:36.364749 threads_py-0.0.8/threadspy/ai/agent.py
--rw-r--r--   0        0        0       29 2023-07-16 12:39:36.364876 threads_py-0.0.8/threadspy/ai/templates/__init__.py
--rw-r--r--   0        0        0      128 2023-07-16 12:39:36.364956 threads_py-0.0.8/threadspy/ai/templates/qna.py
--rw-r--r--   0        0        0      261 2023-07-16 12:39:36.365613 threads_py-0.0.8/threadspy/constants.py
--rw-r--r--   0        0        0    25214 2023-07-16 12:39:36.366733 threads_py-0.0.8/threadspy/threads_api.py
--rw-r--r--   0        0        0     1950 2023-07-16 12:39:36.367180 threads_py-0.0.8/threadspy/types/__init__.py
--rw-r--r--   0        0        0      190 2023-07-16 12:39:36.367376 threads_py-0.0.8/threadspy/types/candidate.py
--rw-r--r--   0        0        0      136 2023-07-16 12:39:36.367602 threads_py-0.0.8/threadspy/types/caption.py
--rw-r--r--   0        0        0      622 2023-07-16 03:01:37.259110 threads_py-0.0.8/threadspy/types/common.py
--rw-r--r--   0        0        0      144 2023-07-16 12:39:36.367812 threads_py-0.0.8/threadspy/types/extensions.py
--rw-r--r--   0        0        0      302 2023-07-16 03:01:37.259277 threads_py-0.0.8/threadspy/types/get_thread_likers_response.py
--rw-r--r--   0        0        0      314 2023-07-16 03:01:37.259370 threads_py-0.0.8/threadspy/types/get_user_profile_replies_response.py
--rw-r--r--   0        0        0      302 2023-07-16 03:01:37.259449 threads_py-0.0.8/threadspy/types/get_user_profile_response.py
--rw-r--r--   0        0        0      315 2023-07-16 03:01:37.259525 threads_py-0.0.8/threadspy/types/get_user_profile_thread_response.py
--rw-r--r--   0        0        0      314 2023-07-16 03:22:06.009163 threads_py-0.0.8/threadspy/types/get_user_profile_threads_response.py
--rw-r--r--   0        0        0      233 2023-07-16 03:43:54.986708 threads_py-0.0.8/threadspy/types/image_versions2.py
--rw-r--r--   0        0        0      216 2023-07-16 03:01:37.259923 threads_py-0.0.8/threadspy/types/media_data.py
--rw-r--r--   0        0        0      772 2023-07-16 03:01:37.260014 threads_py-0.0.8/threadspy/types/post.py
--rw-r--r--   0        0        0      766 2023-07-16 03:01:37.260090 threads_py-0.0.8/threadspy/types/quoted_post.py
--rw-r--r--   0        0        0      191 2023-07-16 12:39:36.368023 threads_py-0.0.8/threadspy/types/reply_facepile_user.py
--rw-r--r--   0        0        0      812 2023-07-16 03:01:37.260232 threads_py-0.0.8/threadspy/types/reposted_post.py
--rw-r--r--   0        0        0      304 2023-07-16 03:01:37.260298 threads_py-0.0.8/threadspy/types/share_info.py
--rw-r--r--   0        0        0      313 2023-07-16 03:42:07.939582 threads_py-0.0.8/threadspy/types/text_post_app_info.py
--rw-r--r--   0        0        0      299 2023-07-16 03:01:37.260436 threads_py-0.0.8/threadspy/types/thread.py
--rw-r--r--   0        0        0      280 2023-07-16 03:01:37.260503 threads_py-0.0.8/threadspy/types/thread_data.py
--rw-r--r--   0        0        0      433 2023-07-16 03:41:29.770812 threads_py-0.0.8/threadspy/types/thread_item.py
--rw-r--r--   0        0        0      142 2023-07-16 03:01:37.260628 threads_py-0.0.8/threadspy/types/threads_bio_link.py
--rw-r--r--   0        0        0      185 2023-07-16 03:01:37.260692 threads_py-0.0.8/threadspy/types/threads_hd_profile_pic_version.py
--rw-r--r--   0        0        0      729 2023-07-16 03:43:52.128369 threads_py-0.0.8/threadspy/types/threads_user.py
--rw-r--r--   0        0        0      222 2023-07-16 03:01:37.260815 threads_py-0.0.8/threadspy/types/threads_user_summary.py
--rw-r--r--   0        0        0      198 2023-07-16 03:01:37.260877 threads_py-0.0.8/threadspy/types/user_data.py
--rw-r--r--   0        0        0      200 2023-07-16 03:01:37.260949 threads_py-0.0.8/threadspy/types/user_profile_data.py
--rw-r--r--   0        0        0      230 2023-07-16 03:01:37.261016 threads_py-0.0.8/threadspy/types/users.py
--rw-r--r--   0        0        0      176 2023-07-16 12:39:36.368230 threads_py-0.0.8/threadspy/types/video_version.py
--rw-r--r--   0        0        0     6927 1970-01-01 00:00:00.000000 threads_py-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-07 02:31:26.110980 threads_py-0.0.9/LICENSE
+-rw-r--r--   0        0        0     6645 2023-07-18 04:21:44.749343 threads_py-0.0.9/README.md
+-rw-r--r--   0        0        0      783 2023-07-18 04:31:29.815612 threads_py-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      117 2023-07-18 04:31:30.160088 threads_py-0.0.9/threadspy/__init__.py
+-rw-r--r--   0        0        0       58 2023-07-18 03:53:09.690317 threads_py-0.0.9/threadspy/ai/__init__.py
+-rw-r--r--   0        0        0     5537 2023-07-18 03:53:09.690402 threads_py-0.0.9/threadspy/ai/agent.py
+-rw-r--r--   0        0        0       29 2023-07-18 03:53:09.690709 threads_py-0.0.9/threadspy/ai/templates/__init__.py
+-rw-r--r--   0        0        0      128 2023-07-18 03:53:09.690974 threads_py-0.0.9/threadspy/ai/templates/qna.py
+-rw-r--r--   0        0        0      261 2023-07-18 03:53:09.691043 threads_py-0.0.9/threadspy/constants.py
+-rw-r--r--   0        0        0    34518 2023-07-18 04:17:28.121600 threads_py-0.0.9/threadspy/threads_api.py
+-rw-r--r--   0        0        0     2115 2023-07-18 04:17:43.275296 threads_py-0.0.9/threadspy/types/__init__.py
+-rw-r--r--   0        0        0      190 2023-07-18 03:53:09.691449 threads_py-0.0.9/threadspy/types/candidate.py
+-rw-r--r--   0        0        0      136 2023-07-18 03:53:09.691537 threads_py-0.0.9/threadspy/types/caption.py
+-rw-r--r--   0        0        0      622 2023-07-07 18:28:28.774860 threads_py-0.0.9/threadspy/types/common.py
+-rw-r--r--   0        0        0      144 2023-07-18 03:53:09.691620 threads_py-0.0.9/threadspy/types/extensions.py
+-rw-r--r--   0        0        0      309 2023-07-18 04:14:09.588594 threads_py-0.0.9/threadspy/types/get_suggested_users_response.py
+-rw-r--r--   0        0        0      302 2023-07-18 04:12:23.435800 threads_py-0.0.9/threadspy/types/get_thread_likers_response.py
+-rw-r--r--   0        0        0      314 2023-07-07 17:56:07.981241 threads_py-0.0.9/threadspy/types/get_user_profile_replies_response.py
+-rw-r--r--   0        0        0      302 2023-07-07 18:03:46.099016 threads_py-0.0.9/threadspy/types/get_user_profile_response.py
+-rw-r--r--   0        0        0      315 2023-07-07 17:57:17.524317 threads_py-0.0.9/threadspy/types/get_user_profile_thread_response.py
+-rw-r--r--   0        0        0      314 2023-07-07 17:57:25.006451 threads_py-0.0.9/threadspy/types/get_user_profile_threads_response.py
+-rw-r--r--   0        0        0      233 2023-07-07 16:58:01.037729 threads_py-0.0.9/threadspy/types/image_versions2.py
+-rw-r--r--   0        0        0      216 2023-07-10 10:27:03.640776 threads_py-0.0.9/threadspy/types/media_data.py
+-rw-r--r--   0        0        0      772 2023-07-07 17:21:37.211579 threads_py-0.0.9/threadspy/types/post.py
+-rw-r--r--   0        0        0      766 2023-07-07 17:21:46.906734 threads_py-0.0.9/threadspy/types/quoted_post.py
+-rw-r--r--   0        0        0      191 2023-07-18 03:53:09.691716 threads_py-0.0.9/threadspy/types/reply_facepile_user.py
+-rw-r--r--   0        0        0      812 2023-07-07 17:22:01.972854 threads_py-0.0.9/threadspy/types/reposted_post.py
+-rw-r--r--   0        0        0      304 2023-07-07 16:58:01.058484 threads_py-0.0.9/threadspy/types/share_info.py
+-rw-r--r--   0        0        0     1087 2023-07-18 04:18:27.363853 threads_py-0.0.9/threadspy/types/suggested_user.py
+-rw-r--r--   0        0        0      313 2023-07-07 18:29:52.928826 threads_py-0.0.9/threadspy/types/text_post_app_info.py
+-rw-r--r--   0        0        0      299 2023-07-07 16:58:01.050147 threads_py-0.0.9/threadspy/types/thread.py
+-rw-r--r--   0        0        0      280 2023-07-08 19:54:05.923801 threads_py-0.0.9/threadspy/types/thread_data.py
+-rw-r--r--   0        0        0      433 2023-07-07 16:58:01.037616 threads_py-0.0.9/threadspy/types/thread_item.py
+-rw-r--r--   0        0        0      142 2023-07-07 17:23:07.797423 threads_py-0.0.9/threadspy/types/threads_bio_link.py
+-rw-r--r--   0        0        0      185 2023-07-07 17:20:54.069996 threads_py-0.0.9/threadspy/types/threads_hd_profile_pic_version.py
+-rw-r--r--   0        0        0      729 2023-07-08 18:23:31.082453 threads_py-0.0.9/threadspy/types/threads_user.py
+-rw-r--r--   0        0        0      222 2023-07-07 17:20:21.160051 threads_py-0.0.9/threadspy/types/threads_user_summary.py
+-rw-r--r--   0        0        0      198 2023-07-07 16:58:01.036997 threads_py-0.0.9/threadspy/types/user_data.py
+-rw-r--r--   0        0        0      200 2023-07-07 16:58:00.996617 threads_py-0.0.9/threadspy/types/user_profile_data.py
+-rw-r--r--   0        0        0      230 2023-07-07 18:11:06.772804 threads_py-0.0.9/threadspy/types/users.py
+-rw-r--r--   0        0        0      176 2023-07-18 03:53:09.691811 threads_py-0.0.9/threadspy/types/video_version.py
+-rw-r--r--   0        0        0     8556 1970-01-01 00:00:00.000000 threads_py-0.0.9/PKG-INFO
```

### Comparing `threads_py-0.0.8/LICENSE` & `threads_py-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `threads_py-0.0.8/README.md` & `threads_py-0.0.9/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 > Unofficial, Reverse-Engineered Python client for Meta's Threads.
 
 **Looking for the TypeScript version?** _Check out **[junhoyeo/threads-api. ![](https://img.shields.io/github/stars/junhoyeo%2Fthreads-api?style=social)](https://github.com/junhoyeo/threads-api)**_
 
 ## Installation
 
 ```bash
-pip install threads-py
+pip install --no-cache-dir --upgrade threads-py
 ```
 
 <details>
 <summary><h3>🚀 Usage (Read)</h3></summary>
 
 ```python
 from threadspy import ThreadsAPI
@@ -93,65 +93,148 @@
 api.publish({
   text: '🤖 Beep',
   link: 'https://github.com/junhoyeo/threads-py',
   parent_post_id: parent_post_id,
 })
 ```
 
-#### ✨ Like/Unlike a Thread (from v0.0.8)
+#### 🔎 Search Users
+
+```python
+search_parameter = "DrunkLeen"
+# 💡 Uses current credentials
+api.search(search_parameter)
+```
+
+#### 👍 Like/Unlike a Thread
 
 ```python
 post_url = 'https://www.threads.net/t/CugF-EjhQ3r'
 post_id = api.get_post_id_from_url(post_url) # or use `get_post_id_from_thread_id`
 
 # 💡 Uses current credentials
 api.like(postIDToLike)
 api.unlike(postIDToLike)
 ```
 
-#### ✨ Follow/Unfollow a User (from v0.0.8)
+#### 👉 Follow/Unfollow a User
+
+```python
+user_id = api.get_user_id_from_username('junhoyeo')
+
+# 💡 Uses current credentials
+api.follow(user_id)
+api.unfollow(user_id)
+```
+
+#### ⛔ Block/Unblock a User
 
 ```python
-user_id_to_follow = api.get_user_id_from_username('junhoyeo')
+user_id = api.get_user_id_from_username('junhoyeo')
 
 # 💡 Uses current credentials
-api.follow(user_id_to_follow)
-api.unfollow(user_id_to_follow)
+api.block(user_id)
+api.unblock(user_id)
 ```
 
+#### 🔇 Mute/Unmute a User
+
+```python
+user_id = api.get_user_id_from_username('junhoyeo')
+
+# 💡 Uses current credentials
+api.mute(user_id)
+api.unmute(user_id)
+```
+
+#### ⏹️ Restrict/Unrestrict a User
+
+```python
+user_id = api.get_user_id_from_username('junhoyeo')
+
+# 💡 Uses current credentials
+api.restrict(user_id)
+api.unrestrict(user_id)
+```
+
+#### 🧑‍🦳 Check FriendshipStatus with a User
+
+```python
+user_id = api.get_user_id_from_username('junhoyeo')
+
+# 💡 Uses current credentials
+api.friendship_status(user_id)
+```
+
+#### 👉🏻👈🏻 Get User Followings and Followers
+
+```python
+user_id = api.get_user_id_from_username('junhoyeo')
+
+# 💡 Uses current credentials
+api.get_followings(user_id)
+api.get_followers(user_id)
+```
+
+#### ➕ Get Suggested Users
+
+```python
+# 💡 Uses current credentials
+api.get_suggested_users()
+# or
+api.get_suggested_users(count=5)
+# or
+api.get_suggested_users(paging=3)
+# or
+api.get_suggested_users(count=5, paging=2)
+# "count" and "paging" parameters are optional
+# default: count = 15 "paging" are optional
+# default: paging = None
+```
+
+
 ## [<img src="./.github/emojis/pushpin.png" width="30" height="30" />](https://github.com/junhoyeo) Roadmap
 
 - [x] ✅ Read public data
   - [x] ✅ Fetch UserID(`314216`) via username(`zuck`)
   - [ ] 🚧 Read timeline feed
   - [x] ✅ Read User Profile Info
   - [x] ✅ Read list of User Threads
     - [ ] 🚧 With Pagination (If auth provided)
   - [x] ✅ Read list of User Replies
     - [ ] 🚧 With Pagination (If auth provided)
   - [x] ✅ Fetch PostID(`3140957200974444958`) via ThreadID(`CuW6-7KyXme`) or PostURL(`https://www.threads.net/t/CuW6-7KyXme`)
   - [x] ✅ Read Threads via PostID
   - [x] ✅ Read Likers in Thread via PostID
-  - [ ] 🚧 Read User Followers
-  - [ ] 🚧 Read User Followings
 - [ ] 🚧 LangChain Agent (`threadspy.ai`)
   - [ ] 🚧 Threads Tool for LangChain
   - [ ] 📌 Link Threads & LLaMa ([@Mineru98](https://github.com/Mineru98))
   - [ ] 📌 Provide statistical analysis of posts in Threads ([@Mineru98](https://github.com/Mineru98))
-- [x] ✅ Write data (i.e. write automated Threads)
-  - [x] ✅ Create new Thread with text
-    - [x] ✅ Make link previews to get shown
-  - [x] ✅ Create new Thread with media
+- [x] ✅ Read user private data
+  - [x] ✅ Get suggested users
+  - [x] ✅ Read User Followers
+  - [x] ✅ Read User Followings
+- [ ] 🚧 Write data (i.e. write automated Threads)
+  - [ ] 🚧 Create new Thread with text
+    - [ ] 🚧 Make link previews to get shown
+  - [ ] 🚧 Create new Thread with media
   - [ ] 🚧 Create new Thread with multiple images
-  - [x] ✅ Reply to existing Thread
+  - [ ] 🚧 Reply to existing Thread
   - [ ] 🚧 Quote Thread
   - [ ] 🚧 Delete Thread
 - [x] ✅ Friendships
   - [x] ✅ Follow User
   - [x] ✅ Unfollow User
+  - [x] ✅ Block User
+  - [x] ✅ Unblock User
+  - [x] ✅ Mute User
+  - [x] ✅ Unmute User
+  - [x] ✅ Restrict User
+  - [x] ✅ Unrestrict User
+  - [x] ✅ Check FriendshipStatus with a User
 - [x] ✅ Interactions
   - [x] ✅ Like Thread
   - [x] ✅ Unlike Thread
 
 ## License
 
 <p align="center">
```

### Comparing `threads_py-0.0.8/pyproject.toml` & `threads_py-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 packages = [{ include = "threadspy", from = "." }]
 name = "threads-py"
-version = "0.0.8"
+version = "0.0.9"
 description = "Unofficial, Reverse-Engineered Python client for Meta's Threads."
 license = "MIT"
 authors = [
   "Junho Yeo <i@junho.io>",
   "iamiks <rmstjr1030@naver.com>",
   "DrunkLeen <reza.df.x@gmail.com>",
   "Ashrf <ashrftvm1@gmail.com>",
```

### Comparing `threads_py-0.0.8/threadspy/ai/agent.py` & `threads_py-0.0.9/threadspy/ai/agent.py`

 * *Files identical despite different names*

### Comparing `threads_py-0.0.8/threadspy/types/__init__.py` & `threads_py-0.0.9/threadspy/types/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,30 +6,33 @@
 from .share_info import ShareInfo
 from .extensions import Extensions
 from .quoted_post import QuotedPost
 from .thread_item import ThreadItem
 from .thread_data import ThreadData
 from .reposted_post import RepostedPost
 from .users import UsersData
+from .suggested_user import SuggestedUser
 from .threads_user import ThreadsUser
 from .video_version import VideoVersion
 from .image_versions2 import ImageVersions2
 from .user_profile_data import UserProfileData
 from .text_post_app_info import TextPostAppInfo
 from .reply_facepile_user import ReplyFacepileUser
 from .threads_user_summary import ThreadsUserSummary
 from .threads_hd_profile_pic_version import ThreadsHdProfilePicVersion
 from .common import (
     CommonMediaDataResponse,
     CommonThreadDataResponse,
     CommonUserProfileDataResponse,
 )
 
+
 from .get_user_profile_response import GetUserProfileResponse
 from .get_thread_likers_response import GetThreadLikersResponse
+from .get_suggested_users_response import GetSuggestedUsersResponse
 from .get_user_profile_thread_response import GetUserProfileThreadResponse
 from .get_user_profile_threads_response import GetUserProfileThreadsResponse
 from .get_user_profile_replies_response import GetUserProfileRepliesResponse
 
 __all__ = [
     "Thread",
     "Caption",
@@ -39,24 +42,26 @@
     "ShareInfo",
     "Extensions",
     "QuotedPost",
     "ThreadItem",
     "ThreadData",
     "RepostedPost",
     "UsersData",
+    "SuggestedUser",
     "ThreadsUser",
     "VideoVersion",
     "ImageVersions2",
     "UserProfileData",
     "TextPostAppInfo",
     "ReplyFacepileUser",
     "ThreadsUserSummary",
     "ThreadsHdProfilePicVersion",
     "CommonMediaDataResponse",
     "CommonThreadDataResponse",
     "CommonUserProfileDataResponse",
     "GetUserProfileResponse",
     "GetThreadLikersResponse",
+    "GetSuggestedUsersResponse",
     "GetUserProfileThreadResponse",
     "GetUserProfileThreadsResponse",
     "GetUserProfileRepliesResponse",
 ]
```

### Comparing `threads_py-0.0.8/threadspy/types/common.py` & `threads_py-0.0.9/threadspy/types/common.py`

 * *Files identical despite different names*

### Comparing `threads_py-0.0.8/threadspy/types/post.py` & `threads_py-0.0.9/threadspy/types/post.py`

 * *Files identical despite different names*

### Comparing `threads_py-0.0.8/threadspy/types/quoted_post.py` & `threads_py-0.0.9/threadspy/types/quoted_post.py`

 * *Files identical despite different names*

### Comparing `threads_py-0.0.8/threadspy/types/reposted_post.py` & `threads_py-0.0.9/threadspy/types/reposted_post.py`

 * *Files identical despite different names*

### Comparing `threads_py-0.0.8/threadspy/types/threads_user.py` & `threads_py-0.0.9/threadspy/types/threads_user.py`

 * *Files identical despite different names*

### Comparing `threads_py-0.0.8/PKG-INFO` & `threads_py-0.0.9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threads-py
-Version: 0.0.8
+Version: 0.0.9
 Summary: Unofficial, Reverse-Engineered Python client for Meta's Threads.
 Home-page: https://github.com/junhoyeo/threads-py
 License: MIT
 Keywords: threads,instagram,facebook,meta,api
 Author: Junho Yeo
 Author-email: i@junho.io
 Requires-Python: >=3.8.1,<4.0
@@ -27,15 +27,15 @@
 > Unofficial, Reverse-Engineered Python client for Meta's Threads.
 
 **Looking for the TypeScript version?** _Check out **[junhoyeo/threads-api. ![](https://img.shields.io/github/stars/junhoyeo%2Fthreads-api?style=social)](https://github.com/junhoyeo/threads-api)**_
 
 ## Installation
 
 ```bash
-pip install threads-py
+pip install --no-cache-dir --upgrade threads-py
 ```
 
 <details>
 <summary><h3>🚀 Usage (Read)</h3></summary>
 
 ```python
 from threadspy import ThreadsAPI
@@ -115,65 +115,148 @@
 api.publish({
   text: '🤖 Beep',
   link: 'https://github.com/junhoyeo/threads-py',
   parent_post_id: parent_post_id,
 })
 ```
 
-#### ✨ Like/Unlike a Thread (from v0.0.8)
+#### 🔎 Search Users
+
+```python
+search_parameter = "DrunkLeen"
+# 💡 Uses current credentials
+api.search(search_parameter)
+```
+
+#### 👍 Like/Unlike a Thread
 
 ```python
 post_url = 'https://www.threads.net/t/CugF-EjhQ3r'
 post_id = api.get_post_id_from_url(post_url) # or use `get_post_id_from_thread_id`
 
 # 💡 Uses current credentials
 api.like(postIDToLike)
 api.unlike(postIDToLike)
 ```
 
-#### ✨ Follow/Unfollow a User (from v0.0.8)
+#### 👉 Follow/Unfollow a User
+
+```python
+user_id = api.get_user_id_from_username('junhoyeo')
+
+# 💡 Uses current credentials
+api.follow(user_id)
+api.unfollow(user_id)
+```
+
+#### ⛔ Block/Unblock a User
 
 ```python
-user_id_to_follow = api.get_user_id_from_username('junhoyeo')
+user_id = api.get_user_id_from_username('junhoyeo')
 
 # 💡 Uses current credentials
-api.follow(user_id_to_follow)
-api.unfollow(user_id_to_follow)
+api.block(user_id)
+api.unblock(user_id)
 ```
 
+#### 🔇 Mute/Unmute a User
+
+```python
+user_id = api.get_user_id_from_username('junhoyeo')
+
+# 💡 Uses current credentials
+api.mute(user_id)
+api.unmute(user_id)
+```
+
+#### ⏹️ Restrict/Unrestrict a User
+
+```python
+user_id = api.get_user_id_from_username('junhoyeo')
+
+# 💡 Uses current credentials
+api.restrict(user_id)
+api.unrestrict(user_id)
+```
+
+#### 🧑‍🦳 Check FriendshipStatus with a User
+
+```python
+user_id = api.get_user_id_from_username('junhoyeo')
+
+# 💡 Uses current credentials
+api.friendship_status(user_id)
+```
+
+#### 👉🏻👈🏻 Get User Followings and Followers
+
+```python
+user_id = api.get_user_id_from_username('junhoyeo')
+
+# 💡 Uses current credentials
+api.get_followings(user_id)
+api.get_followers(user_id)
+```
+
+#### ➕ Get Suggested Users
+
+```python
+# 💡 Uses current credentials
+api.get_suggested_users()
+# or
+api.get_suggested_users(count=5)
+# or
+api.get_suggested_users(paging=3)
+# or
+api.get_suggested_users(count=5, paging=2)
+# "count" and "paging" parameters are optional
+# default: count = 15 "paging" are optional
+# default: paging = None
+```
+
+
 ## [<img src="./.github/emojis/pushpin.png" width="30" height="30" />](https://github.com/junhoyeo) Roadmap
 
 - [x] ✅ Read public data
   - [x] ✅ Fetch UserID(`314216`) via username(`zuck`)
   - [ ] 🚧 Read timeline feed
   - [x] ✅ Read User Profile Info
   - [x] ✅ Read list of User Threads
     - [ ] 🚧 With Pagination (If auth provided)
   - [x] ✅ Read list of User Replies
     - [ ] 🚧 With Pagination (If auth provided)
   - [x] ✅ Fetch PostID(`3140957200974444958`) via ThreadID(`CuW6-7KyXme`) or PostURL(`https://www.threads.net/t/CuW6-7KyXme`)
   - [x] ✅ Read Threads via PostID
   - [x] ✅ Read Likers in Thread via PostID
-  - [ ] 🚧 Read User Followers
-  - [ ] 🚧 Read User Followings
 - [ ] 🚧 LangChain Agent (`threadspy.ai`)
   - [ ] 🚧 Threads Tool for LangChain
   - [ ] 📌 Link Threads & LLaMa ([@Mineru98](https://github.com/Mineru98))
   - [ ] 📌 Provide statistical analysis of posts in Threads ([@Mineru98](https://github.com/Mineru98))
-- [x] ✅ Write data (i.e. write automated Threads)
-  - [x] ✅ Create new Thread with text
-    - [x] ✅ Make link previews to get shown
-  - [x] ✅ Create new Thread with media
+- [x] ✅ Read user private data
+  - [x] ✅ Get suggested users
+  - [x] ✅ Read User Followers
+  - [x] ✅ Read User Followings
+- [ ] 🚧 Write data (i.e. write automated Threads)
+  - [ ] 🚧 Create new Thread with text
+    - [ ] 🚧 Make link previews to get shown
+  - [ ] 🚧 Create new Thread with media
   - [ ] 🚧 Create new Thread with multiple images
-  - [x] ✅ Reply to existing Thread
+  - [ ] 🚧 Reply to existing Thread
   - [ ] 🚧 Quote Thread
   - [ ] 🚧 Delete Thread
 - [x] ✅ Friendships
   - [x] ✅ Follow User
   - [x] ✅ Unfollow User
+  - [x] ✅ Block User
+  - [x] ✅ Unblock User
+  - [x] ✅ Mute User
+  - [x] ✅ Unmute User
+  - [x] ✅ Restrict User
+  - [x] ✅ Unrestrict User
+  - [x] ✅ Check FriendshipStatus with a User
 - [x] ✅ Interactions
   - [x] ✅ Like Thread
   - [x] ✅ Unlike Thread
 
 ## License
 
 <p align="center">
```

