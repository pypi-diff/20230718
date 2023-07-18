# Comparing `tmp/yaylib-1.0.2.tar.gz` & `tmp/yaylib-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaylib-1.0.2.tar", last modified: Mon Jul 17 07:00:31 2023, max compression
+gzip compressed data, was "yaylib-1.0.3.tar", last modified: Tue Jul 18 10:33:39 2023, max compression
```

## Comparing `yaylib-1.0.2.tar` & `yaylib-1.0.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 07:00:31.115517 yaylib-1.0.2/
--rw-rw-rw-   0        0        0     1096 2023-07-09 07:25:01.000000 yaylib-1.0.2/LICENSE
--rw-rw-rw-   0        0        0    10834 2023-07-17 07:00:31.115517 yaylib-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     9970 2023-07-16 09:12:13.000000 yaylib-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-17 07:00:31.115517 yaylib-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1552 2023-07-16 09:10:03.000000 yaylib-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 07:00:31.079666 yaylib-1.0.2/tests/
--rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.2/tests/test_call.py
--rw-rw-rw-   0        0        0     1935 2023-07-09 07:25:01.000000 yaylib-1.0.2/tests/test_cassandra.py
--rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.2/tests/test_chat.py
--rw-rw-rw-   0        0        0     1337 2023-07-09 07:25:01.000000 yaylib-1.0.2/tests/test_group.py
--rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.2/tests/test_misc.py
--rw-rw-rw-   0        0        0     3723 2023-07-09 07:25:01.000000 yaylib-1.0.2/tests/test_post.py
--rw-rw-rw-   0        0        0     2028 2023-07-09 07:25:01.000000 yaylib-1.0.2/tests/test_review.py
--rw-rw-rw-   0        0        0     1339 2023-07-09 07:25:01.000000 yaylib-1.0.2/tests/test_thread.py
--rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.2/tests/test_user.py
-drwxrwxrwx   0        0        0        0 2023-07-17 07:00:31.086984 yaylib-1.0.2/yaylib/
--rw-rw-rw-   0        0        0      519 2023-07-09 07:25:01.000000 yaylib-1.0.2/yaylib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 07:00:31.114515 yaylib-1.0.2/yaylib/api/
--rw-rw-rw-   0        0        0      697 2023-07-09 07:25:01.000000 yaylib-1.0.2/yaylib/api/__init__.py
--rw-rw-rw-   0        0        0    10401 2023-07-17 06:36:16.000000 yaylib-1.0.2/yaylib/api/api.py
--rw-rw-rw-   0        0        0     8657 2023-07-16 04:28:15.000000 yaylib-1.0.2/yaylib/api/call.py
--rw-rw-rw-   0        0        0     2699 2023-07-16 08:40:55.000000 yaylib-1.0.2/yaylib/api/cassandra.py
--rw-rw-rw-   0        0        0    14881 2023-07-17 02:44:35.000000 yaylib-1.0.2/yaylib/api/chat.py
--rw-rw-rw-   0        0        0    23695 2023-07-16 04:28:15.000000 yaylib-1.0.2/yaylib/api/group.py
--rw-rw-rw-   0        0        0     8244 2023-07-16 09:33:16.000000 yaylib-1.0.2/yaylib/api/login.py
--rw-rw-rw-   0        0        0     7393 2023-07-17 06:13:19.000000 yaylib-1.0.2/yaylib/api/misc.py
--rw-rw-rw-   0        0        0    33692 2023-07-16 04:28:15.000000 yaylib-1.0.2/yaylib/api/post.py
--rw-rw-rw-   0        0        0     4488 2023-07-16 04:28:15.000000 yaylib-1.0.2/yaylib/api/review.py
--rw-rw-rw-   0        0        0     5945 2023-07-16 04:28:15.000000 yaylib-1.0.2/yaylib/api/thread.py
--rw-rw-rw-   0        0        0    24492 2023-07-17 06:58:52.000000 yaylib-1.0.2/yaylib/api/user.py
--rw-rw-rw-   0        0        0    86196 2023-07-17 02:37:50.000000 yaylib-1.0.2/yaylib/client.py
--rw-rw-rw-   0        0        0    19214 2023-07-17 06:59:15.000000 yaylib-1.0.2/yaylib/config.py
--rw-rw-rw-   0        0        0     2131 2023-07-16 04:28:15.000000 yaylib-1.0.2/yaylib/errors.py
--rw-rw-rw-   0        0        0    53336 2023-07-09 07:25:01.000000 yaylib-1.0.2/yaylib/models.py
--rw-rw-rw-   0        0        0    33222 2023-07-09 07:25:01.000000 yaylib-1.0.2/yaylib/responses.py
--rw-rw-rw-   0        0        0     4600 2023-07-16 09:33:56.000000 yaylib-1.0.2/yaylib/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-17 07:00:31.103398 yaylib-1.0.2/yaylib.egg-info/
--rw-rw-rw-   0        0        0    10834 2023-07-17 07:00:30.000000 yaylib-1.0.2/yaylib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      721 2023-07-17 07:00:31.000000 yaylib-1.0.2/yaylib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 07:00:30.000000 yaylib-1.0.2/yaylib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-07-17 07:00:30.000000 yaylib-1.0.2/yaylib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-17 07:00:30.000000 yaylib-1.0.2/yaylib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 10:33:39.051243 yaylib-1.0.3/
+-rw-rw-rw-   0        0        0     1096 2023-07-09 07:25:01.000000 yaylib-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0    10828 2023-07-18 10:33:39.050242 yaylib-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     9964 2023-07-18 08:52:45.000000 yaylib-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-18 10:33:39.051243 yaylib-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1552 2023-07-16 09:10:03.000000 yaylib-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 10:33:38.998476 yaylib-1.0.3/tests/
+-rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.3/tests/test_call.py
+-rw-rw-rw-   0        0        0     1935 2023-07-09 07:25:01.000000 yaylib-1.0.3/tests/test_cassandra.py
+-rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.3/tests/test_chat.py
+-rw-rw-rw-   0        0        0     1337 2023-07-09 07:25:01.000000 yaylib-1.0.3/tests/test_group.py
+-rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.3/tests/test_misc.py
+-rw-rw-rw-   0        0        0     3723 2023-07-09 07:25:01.000000 yaylib-1.0.3/tests/test_post.py
+-rw-rw-rw-   0        0        0     2028 2023-07-09 07:25:01.000000 yaylib-1.0.3/tests/test_review.py
+-rw-rw-rw-   0        0        0     1339 2023-07-09 07:25:01.000000 yaylib-1.0.3/tests/test_thread.py
+-rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.3/tests/test_user.py
+drwxrwxrwx   0        0        0        0 2023-07-18 10:33:39.011415 yaylib-1.0.3/yaylib/
+-rw-rw-rw-   0        0        0      519 2023-07-09 07:25:01.000000 yaylib-1.0.3/yaylib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 10:33:39.048943 yaylib-1.0.3/yaylib/api/
+-rw-rw-rw-   0        0        0      697 2023-07-09 07:25:01.000000 yaylib-1.0.3/yaylib/api/__init__.py
+-rw-rw-rw-   0        0        0    10255 2023-07-18 08:52:45.000000 yaylib-1.0.3/yaylib/api/api.py
+-rw-rw-rw-   0        0        0     9431 2023-07-18 10:27:35.000000 yaylib-1.0.3/yaylib/api/call.py
+-rw-rw-rw-   0        0        0     2699 2023-07-18 08:52:45.000000 yaylib-1.0.3/yaylib/api/cassandra.py
+-rw-rw-rw-   0        0        0    14881 2023-07-18 08:52:45.000000 yaylib-1.0.3/yaylib/api/chat.py
+-rw-rw-rw-   0        0        0    23695 2023-07-18 08:52:45.000000 yaylib-1.0.3/yaylib/api/group.py
+-rw-rw-rw-   0        0        0     8205 2023-07-18 08:52:45.000000 yaylib-1.0.3/yaylib/api/login.py
+-rw-rw-rw-   0        0        0     7417 2023-07-18 08:52:45.000000 yaylib-1.0.3/yaylib/api/misc.py
+-rw-rw-rw-   0        0        0    33692 2023-07-18 08:52:45.000000 yaylib-1.0.3/yaylib/api/post.py
+-rw-rw-rw-   0        0        0     4488 2023-07-18 08:52:45.000000 yaylib-1.0.3/yaylib/api/review.py
+-rw-rw-rw-   0        0        0     5945 2023-07-18 08:52:45.000000 yaylib-1.0.3/yaylib/api/thread.py
+-rw-rw-rw-   0        0        0    24492 2023-07-18 08:52:45.000000 yaylib-1.0.3/yaylib/api/user.py
+-rw-rw-rw-   0        0        0    86745 2023-07-18 10:29:00.000000 yaylib-1.0.3/yaylib/client.py
+-rw-rw-rw-   0        0        0    19269 2023-07-18 10:33:32.000000 yaylib-1.0.3/yaylib/config.py
+-rw-rw-rw-   0        0        0     2131 2023-07-18 08:52:45.000000 yaylib-1.0.3/yaylib/errors.py
+-rw-rw-rw-   0        0        0    53336 2023-07-09 07:25:01.000000 yaylib-1.0.3/yaylib/models.py
+-rw-rw-rw-   0        0        0    33426 2023-07-18 08:52:45.000000 yaylib-1.0.3/yaylib/responses.py
+-rw-rw-rw-   0        0        0     4472 2023-07-18 08:52:45.000000 yaylib-1.0.3/yaylib/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-18 10:33:39.032985 yaylib-1.0.3/yaylib.egg-info/
+-rw-rw-rw-   0        0        0    10828 2023-07-18 10:33:38.000000 yaylib-1.0.3/yaylib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      721 2023-07-18 10:33:38.000000 yaylib-1.0.3/yaylib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 10:33:38.000000 yaylib-1.0.3/yaylib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-07-18 10:33:38.000000 yaylib-1.0.3/yaylib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-18 10:33:38.000000 yaylib-1.0.3/yaylib.egg-info/top_level.txt
```

### Comparing `yaylib-1.0.2/LICENSE` & `yaylib-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.2/PKG-INFO` & `yaylib-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaylib
-Version: 1.0.2
+Version: 1.0.3
 Summary: This Python package provides an easy-to-use interface for accessing data from Yay! (https://yay.space/). With this API Client, you can retrieve user profiles, posts, comments, and other content from Yay!, as well as perform common tasks like liking and commenting on posts.
 Home-page: https://github.com/qvco/yaylib
 Download-URL: https://github.com/qvco/yaylib
 Author: Qvco, Konn
 Author-email: nikola.desuga@gmail.com
 Maintainer: Qvco, Konn
 Maintainer-email: nikola.desuga@gmail.com
@@ -175,15 +175,15 @@
 
 timeline = api.get_timeline_by_keyword(
     keyword="プログラミング",
     number=15
 )
 
 for post in timeline.posts:
-    response = api.like_posts(post.id)
+    response = api.like(post.id)
     print(post.id, response.data) # 実行結果を出力
 ```
 
 #### ✨ タイムラインのユーザーをフォローする
 
 ```python
 import yaylib
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yaylib Version: 1.0.2 Summary: This Python package
+Metadata-Version: 2.1 Name: yaylib Version: 1.0.3 Summary: This Python package
 provides an easy-to-use interface for accessing data from Yay! (https://
 yay.space/). With this API Client, you can retrieve user profiles, posts,
 comments, and other content from Yay!, as well as perform common tasks like
 liking and commenting on posts. Home-page: https://github.com/qvco/yaylib
 Download-URL: https://github.com/qvco/yaylib Author: Qvco, Konn Author-email:
 nikola.desuga@gmail.com Maintainer: Qvco, Konn Maintainer-email:
 nikola.desuga@gmail.com License: MIT Keywords:
@@ -69,15 +69,15 @@
 print(post.text) # æ¬æ print(post.likes_count) # ããã­æ° print
 (post.reposts_count) # (Â´âï½â©)âageâã®æ° print
 (post.in_reply_to_post_count) # è¿ä¿¡ã®æ° ``` #### â¨
 ã¿ã¤ã ã©ã¤ã³ãã­ã¼ã¯ã¼ãã§æ¤ç´¢ãã¦ãããã­ããã
 ```python import yaylib api = yaylib.Client() api.login
 (email="ã¡ã¼ã«ã¢ãã¬ã¹", password="ãã¹ã¯ã¼ã") timeline =
 api.get_timeline_by_keyword( keyword="ãã­ã°ã©ãã³ã°", number=15 ) for
-post in timeline.posts: response = api.like_posts(post.id) print(post.id,
+post in timeline.posts: response = api.like(post.id) print(post.id,
 response.data) # å®è¡çµæãåºå ``` #### â¨
 ã¿ã¤ã ã©ã¤ã³ã®ã¦ã¼ã¶ã¼ããã©ã­ã¼ãã ```python import yaylib
 api = yaylib.Client() api.login(email="ã¡ã¼ã«ã¢ãã¬ã¹",
 password="ãã¹ã¯ã¼ã") timeline = api.get_timeline(number=15) for post in
 timeline.posts: api.follow_user(post.user.id) ```
 ããè©³ããä½¿ç¨ä¾ã«ã¤ãã¦ã¯ã[ãã¡ã](https://github.com/qvco/
 yaylib/blob/master/examples) ãåç§ãã¦ãã ããã
```

### Comparing `yaylib-1.0.2/README.md` & `yaylib-1.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
 
 timeline = api.get_timeline_by_keyword(
     keyword="プログラミング",
     number=15
 )
 
 for post in timeline.posts:
-    response = api.like_posts(post.id)
+    response = api.like(post.id)
     print(post.id, response.data) # 実行結果を出力
 ```
 
 #### ✨ タイムラインのユーザーをフォローする
 
 ```python
 import yaylib
```

#### html2text {}

```diff
@@ -57,15 +57,15 @@
 print(post.text) # æ¬æ print(post.likes_count) # ããã­æ° print
 (post.reposts_count) # (Â´âï½â©)âageâã®æ° print
 (post.in_reply_to_post_count) # è¿ä¿¡ã®æ° ``` #### â¨
 ã¿ã¤ã ã©ã¤ã³ãã­ã¼ã¯ã¼ãã§æ¤ç´¢ãã¦ãããã­ããã
 ```python import yaylib api = yaylib.Client() api.login
 (email="ã¡ã¼ã«ã¢ãã¬ã¹", password="ãã¹ã¯ã¼ã") timeline =
 api.get_timeline_by_keyword( keyword="ãã­ã°ã©ãã³ã°", number=15 ) for
-post in timeline.posts: response = api.like_posts(post.id) print(post.id,
+post in timeline.posts: response = api.like(post.id) print(post.id,
 response.data) # å®è¡çµæãåºå ``` #### â¨
 ã¿ã¤ã ã©ã¤ã³ã®ã¦ã¼ã¶ã¼ããã©ã­ã¼ãã ```python import yaylib
 api = yaylib.Client() api.login(email="ã¡ã¼ã«ã¢ãã¬ã¹",
 password="ãã¹ã¯ã¼ã") timeline = api.get_timeline(number=15) for post in
 timeline.posts: api.follow_user(post.user.id) ```
 ããè©³ããä½¿ç¨ä¾ã«ã¤ãã¦ã¯ã[ãã¡ã](https://github.com/qvco/
 yaylib/blob/master/examples) ãåç§ãã¦ãã ããã
```

### Comparing `yaylib-1.0.2/setup.py` & `yaylib-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.2/tests/test_call.py` & `yaylib-1.0.3/tests/test_call.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.2/tests/test_cassandra.py` & `yaylib-1.0.3/tests/test_cassandra.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.2/tests/test_chat.py` & `yaylib-1.0.3/tests/test_chat.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.2/tests/test_group.py` & `yaylib-1.0.3/tests/test_group.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.2/tests/test_misc.py` & `yaylib-1.0.3/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.2/tests/test_post.py` & `yaylib-1.0.3/tests/test_post.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.2/tests/test_review.py` & `yaylib-1.0.3/tests/test_review.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.2/tests/test_thread.py` & `yaylib-1.0.3/tests/test_thread.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.2/tests/test_user.py` & `yaylib-1.0.3/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.2/yaylib/__init__.py` & `yaylib-1.0.3/yaylib/__init__.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.2/yaylib/api/__init__.py` & `yaylib-1.0.3/yaylib/api/__init__.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.2/yaylib/api/api.py` & `yaylib-1.0.3/yaylib/api/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -140,29 +140,27 @@
 
             response = self.session.request(
                 method, endpoint, params=params, json=payload, headers=headers
             )
 
             if self.save_session is True and response.status_code == 401:
                 if "/api/v1/oauth/token" in endpoint:
-                    os.remove(self.base_path + "credentials.json")
+                    os.remove(self.base_path + "session.json")
                     message = "Refresh token expired. Try logging in again."
                     raise AuthenticationError(message)
 
                 auth_retry_count += 1
                 self.logger.debug("Access token expired. Refreshing tokens...")
 
                 if auth_retry_count < max_auth_retries:
-                    credentials = load_session(base_path=self.base_path)
+                    session = load_session(base_path=self.base_path)
 
-                    if credentials is not None and self.fernet is not None:
-                        credentials = decrypt(
-                            fernet=self.fernet, credentials=credentials
-                        )
-                        refresh_token = credentials["refresh_token"]
+                    if session is not None and self.fernet is not None:
+                        session = decrypt(fernet=self.fernet, session=session)
+                        refresh_token = session["refresh_token"]
                         response = get_token(
                             self,
                             grant_type="refresh_token",
                             refresh_token=refresh_token,
                         )
                         save_session(
                             base_path=self.base_path,
@@ -173,15 +171,15 @@
                         )
                         self.session.headers[
                             "Authorization"
                         ] = f"Bearer {response.access_token}"
                         continue
 
                 else:
-                    os.remove(self.base_path + "credentials.json")
+                    os.remove(self.base_path + "session.json")
                     message = (
                         "Maximum authentication retries exceeded. Try logging in again."
                     )
                     raise AuthenticationError(message)
 
             if response.status_code not in self.retry_statuses:
                 break
@@ -242,32 +240,31 @@
 
     def _check_authorization(self, access_token) -> None:
         if self.session.headers.get("Authorization") is None and access_token is None:
             message = "Authorization is not present in the header."
             raise AuthenticationError(message)
 
     def _handle_response(self, response, formatted_response):
-        translated_response = formatted_response
         if isinstance(formatted_response, dict):
-            translated_response = self._translate_error_message(formatted_response)
+            formatted_response = self._translate_error_message(formatted_response)
 
         if response.status_code == 400:
-            raise BadRequestError(translated_response)
+            raise BadRequestError(formatted_response)
         if response.status_code == 401:
-            raise AuthenticationError(translated_response)
+            raise AuthenticationError(formatted_response)
         if response.status_code == 403:
-            raise ForbiddenError(translated_response)
+            raise ForbiddenError(formatted_response)
         if response.status_code == 404:
-            raise NotFoundError(translated_response)
+            raise NotFoundError(formatted_response)
         if response.status_code == 429:
-            raise RateLimitError(translated_response)
+            raise RateLimitError(formatted_response)
         if response.status_code == 500:
-            raise YayServerError(translated_response)
+            raise YayServerError(formatted_response)
         if response.status_code and not 200 <= response.status_code < 300:
-            raise HTTPError(translated_response)
+            raise HTTPError(formatted_response)
         return formatted_response
 
     def _translate_error_message(self, response):
         if self.err_lang == "ja":
             try:
                 error_code = response.get("error_code", None)
                 if error_code is not None:
```

### Comparing `yaylib-1.0.2/yaylib/api/call.py` & `yaylib-1.0.3/yaylib/api/call.py`

 * *Files 9% similar despite different names*

```diff
@@ -284,14 +284,35 @@
         data_type=ConferenceCallResponse,
         access_token=access_token,
     ).conference_call
     self.logger.info("Joined the call.")
     return response
 
 
+def start_anonymous_call(self, conference_id: int, agora_uid: str) -> ConferenceCall:
+    response = self._make_request(
+        "POST",
+        endpoint=f"{Endpoints.ANONYMOUS_CALLS_V1}/start_conference_call",
+        payload={"conference_id": conference_id, "agora_uid": agora_uid},
+        data_type=ConferenceCallResponse,
+    ).conference_call
+    self.logger.info("Joined the call.")
+    return response
+
+
+def stop__anonymous_call(self, conference_id: int, agora_uid: str = None):
+    response = self._make_request(
+        "POST",
+        endpoint=f"{Endpoints.ANONYMOUS_CALLS_V1}/leave_conference_call",
+        payload={"conference_id": conference_id, "agora_uid": agora_uid},
+    )
+    self.logger.info("Left the call.")
+    return response
+
+
 def stop_call(self, conference_id: int, call_sid: str = None, access_token: str = None):
     response = self._make_request(
         "POST",
         endpoint=f"{Endpoints.CALLS_V1}/leave_conference_call",
         payload={"conference_id": conference_id, "call_sid": call_sid},
         access_token=access_token,
     )
```

### Comparing `yaylib-1.0.2/yaylib/api/cassandra.py` & `yaylib-1.0.3/yaylib/api/cassandra.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.2/yaylib/api/chat.py` & `yaylib-1.0.3/yaylib/api/chat.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.2/yaylib/api/group.py` & `yaylib-1.0.3/yaylib/api/group.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.2/yaylib/api/login.py` & `yaylib-1.0.3/yaylib/api/login.py`

 * *Files 4% similar despite different names*

```diff
@@ -111,26 +111,26 @@
         return False
 
 
 def login_with_email(
     self, email: str, password: str, secret_key: str = None
 ) -> LoginUserResponse:
     if self.save_session:
-        credentials = load_session(base_path=self.base_path, check_email=email)
-        if credentials is not None and secret_key is not None:
+        session = load_session(base_path=self.base_path, check_email=email)
+        if session is not None and secret_key is not None:
             self.secret_key = secret_key
             self.fernet = Fernet(secret_key)
-            credentials = decrypt(fernet=self.fernet, credentials=credentials)
+            session = decrypt(fernet=self.fernet, session=session)
             self.session.headers.setdefault(
-                "Authorization", f"Bearer {credentials['access_token']}"
+                "Authorization", f"Bearer {session['access_token']}"
             )
-            self.logger.info(f"Successfully logged in as '{credentials['user_id']}'")
-            return credentials
-        elif credentials is not None:
-            message = f"{Colors.WARNING}Credential file found. The 'secret_key' must be provided to decrypt the credentials.{Colors.RESET}"
+            self.logger.info(f"Successfully logged in as '{session['user_id']}'")
+            return session
+        elif session is not None:
+            message = f"{Colors.WARNING}Session file found. The 'secret_key' must be provided to decrypt the credentials.{Colors.RESET}"
             console_print(message)
 
     response = self._make_request(
         "POST",
         endpoint=f"{Endpoints.USERS_V3}/login_with_email",
         payload={
             "api_key": self.api_key,
```

### Comparing `yaylib-1.0.2/yaylib/api/misc.py` & `yaylib-1.0.3/yaylib/api/misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,17 @@
     self.logger.info("SNS thumbnail generated.")
     return response
 
 
 def send_verification_code(self, email: str):
     response = self._make_request(
         "POST",
-        endpoint=self.get_email_verification_presigned_url(email=email, locale="ja"),
+        endpoint=self.get_email_verification_presigned_url(
+            email=email, locale="ja"
+        ).url,
         payload={"locale": "ja", "email": email},
     )
     self.logger.info(f"Verification code successfully sent to '{email}'.")
     return response
 
 
 def get_email_grant_token(self, code: int, email: str) -> EmailGrantTokenResponse:
@@ -101,15 +103,15 @@
             "device_uuid": self.device_uuid,
             "email": email,
             "locale": locale,
             "intent": intent,
         },
         data_type=EmailVerificationPresignedUrlResponse,
         access_token=access_token,
-    ).url
+    )
 
 
 def get_file_upload_presigned_urls(
     self, file_names: List[str], access_token: str = None
 ) -> List[PresignedUrl]:
     return self._make_request(
         "GET",
```

### Comparing `yaylib-1.0.2/yaylib/api/post.py` & `yaylib-1.0.3/yaylib/api/post.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.2/yaylib/api/review.py` & `yaylib-1.0.3/yaylib/api/review.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.2/yaylib/api/thread.py` & `yaylib-1.0.3/yaylib/api/thread.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.2/yaylib/api/user.py` & `yaylib-1.0.3/yaylib/api/user.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.2/yaylib/client.py` & `yaylib-1.0.3/yaylib/client.py`

 * *Files identical despite different names*

```diff
@@ -38,15 +38,17 @@
     invite_to_call_bulk,
     invite_users_to_call,
     invite_users_to_chat_call,
     kick_and_ban_from_call,
     set_call,
     set_user_role,
     start_call,
+    start_anonymous_call,
     stop_call,
+    stop__anonymous_call
 )
 from .api.cassandra import (
     get_user_activities,
     get_user_merged_activities,
     received_notification,
 )
 from .api.chat import (
@@ -335,24 +337,24 @@
         - access_token: str - (optional)
         - proxy: str - (optional)
         - max_retries: int - (optional)
         - backoff_factor: float - (optional)
         - timeout: int - (optional)
         - err_lang: str - (optional)
         - base_path: str - (optional)
-        - loglevel_stream: int - (optional)
-        - host: str - (optional)
+        - save_session: bool - (optional)
+        - loglevel: int - (optional)
 
     <https://github.com/qvco/yaylib>
 
     ---
 
     ### Yay! (nanameue, Inc.) API Client
 
-    Copyright (c) 2023 Qvco, Konn
+    Copyright (c) 2023-present Qvco, Konn
 
     """
 
     # -CALL
 
     def get_user_active_call(self, user_id: int, access_token: str = None) -> Post:
         """
@@ -539,24 +541,42 @@
         """
 
         通話に参加します
 
         """
         return start_call(self, conference_id, call_sid, access_token)
 
+    def join_call_as_anonymous(
+        self, conference_id: int, agora_uid: str
+    ) -> ConferenceCall:
+        """
+
+        無名くんとして通話に参加します
+
+        """
+        return start_anonymous_call(self, conference_id, agora_uid)
+
     def leave_call(
         self, conference_id: int, call_sid: str = None, access_token: str = None
     ) -> dict:
         """
 
         通話から退出します
 
         """
         return stop_call(self, conference_id, call_sid, access_token)
 
+    def leave_call_as_anonymous(self, conference_id: int, agora_uid: str = None):
+        """
+
+        通話から退出します
+
+        """
+        return stop__anonymous_call(self, conference_id, agora_uid)
+
     # -CASSANDRA
 
     def get_activities(self, access_token: str = None, **params) -> ActivitiesResponse:
         """
 
         通知を取得します
```

### Comparing `yaylib-1.0.2/yaylib/config.py` & `yaylib-1.0.3/yaylib/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,21 +22,22 @@
 SOFTWARE.
 """
 
 from enum import Enum
 
 
 class Configs:
-    YAYLIB_VERSION = "1.0.2"
-    YAY_API_VERSION = "3.16"
-    YAY_VERSION_NAME = "3.16.1"
-    YAY_API_VERSION_KEY = "e83a1d2588918c2061280427c88e6f56"
+    YAYLIB_VERSION = "1.0.3"
+    YAY_API_VERSION = "3.20"
+    YAY_VERSION_NAME = "3.20.1"
+    YAY_API_VERSION_KEY = "d4420f4943bebe2831c20b2b4cb4a8c1"
     YAY_API_KEY = "ccd59ee269c01511ba763467045c115779fcae3050238a252f1bd1a4b65cfec6"
     YAY_SHARED_KEY = "yayZ1"
     YAY_STORE_KEY = "yayZ1payment"
+    AGORA_APP_ID = "79046b8c9be54945b7f10a4d128d5395"
     ID_CARD_CHECK_SECRET_KEY = "4aa6d1c301a97154bc1098c2"
     YAY_REVIEW_HOST_1 = "review.yay.space"
     YAY_REVIEW_HOST_2 = "cas-stg.yay.space"
     YAY_STAGING_HOST_1 = "stg.yay.space"
     YAY_STAGING_HOST_2 = "cas.yay.space"
     YAY_PRODUCTION_HOST = "api.yay.space"
     YAY_API_URL = "https://" + YAY_PRODUCTION_HOST
```

### Comparing `yaylib-1.0.2/yaylib/errors.py` & `yaylib-1.0.3/yaylib/errors.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.2/yaylib/models.py` & `yaylib-1.0.3/yaylib/models.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.2/yaylib/responses.py` & `yaylib-1.0.3/yaylib/responses.py`

 * *Files 0% similar despite different names*

```diff
@@ -361,19 +361,22 @@
         self.email_grant_token = data.get("email_grant_token")
 
     def __repr__(self):
         return f"EmailGrantTokenResponse(data={self.data})"
 
 
 class EmailVerificationPresignedUrlResponse:
-    __slots__ = ("data", "url")
+    __slots__ = ("data", "url", "presigned_url", "expires_at", "method_type")
 
     def __init__(self, data):
         self.data = data
         self.url = data.get("url")
+        self.presigned_url = data.get("presigned_url")
+        self.expires_at = data.get("expires_at")
+        self.method_type = data.get("method_type")
 
     def __repr__(self):
         return f"EmailVerificationPresignedUrlResponse(data={self.data})"
 
 
 class PresignedUrlResponse:
     __slots__ = ("data", "presigned_url")
```

### Comparing `yaylib-1.0.2/yaylib/utils.py` & `yaylib-1.0.3/yaylib/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -60,82 +60,82 @@
 
 def parse_datetime(timestamp: int) -> str:
     if timestamp is not None:
         return str(datetime.fromtimestamp(timestamp))
     return timestamp
 
 
-def encrypt(fernet, credentials: dict):
-    credentials.update(
+def encrypt(fernet, session: dict):
+    session.update(
         {
             "access_token": fernet.encrypt(
-                credentials.get("access_token").encode()
+                session.get("access_token").encode()
             ).decode(),
             "refresh_token": fernet.encrypt(
-                credentials.get("refresh_token").encode()
+                session.get("refresh_token").encode()
             ).decode(),
         }
     )
-    return credentials
+    return session
 
 
-def decrypt(fernet, credentials: dict):
-    credentials.update(
+def decrypt(fernet, session: dict):
+    session.update(
         {
-            "access_token": fernet.decrypt(credentials.get("access_token")).decode(),
-            "refresh_token": fernet.decrypt(credentials.get("refresh_token")).decode(),
+            "access_token": fernet.decrypt(session.get("access_token")).decode(),
+            "refresh_token": fernet.decrypt(session.get("refresh_token")).decode(),
         }
     )
-    return credentials
+    return session
 
 
 def save_session(
     base_path: str,
     fernet,
     access_token: str,
     refresh_token: str,
     user_id: int,
     email: str = None,
 ):
-    credentials = load_session(base_path=base_path)
-    updated_credentials = {
+    session = load_session(base_path=base_path)
+    updated_session = {
         "access_token": access_token,
         "refresh_token": refresh_token,
         "user_id": user_id,
         "email": email,
     }
     if email is None:
-        updated_credentials["email"] = credentials.get("email")
+        updated_session["email"] = session.get("email")
 
-    updated_credentials = encrypt(fernet, updated_credentials)
+    updated_session = encrypt(fernet, updated_session)
 
-    with open(base_path + "credentials.json", "w") as f:
-        json.dump(updated_credentials, f)
+    with open(base_path + "session.json", "w") as f:
+        json.dump(updated_session, f)
 
 
 def load_session(base_path: str, fernet=None, check_email: str = None):
-    if not os.path.exists(base_path + "credentials.json"):
+    if not os.path.exists(base_path + "session.json"):
         return None
 
-    with open(base_path + "credentials.json", "r") as f:
-        credentials = json.load(f)
+    with open(base_path + "session.json", "r") as f:
+        session = json.load(f)
 
     result = all(
-        key in credentials
+        key in session
         for key in ("access_token", "refresh_token", "user_id", "email")
     )
-    credentials = None if result is False else credentials
+    session = None if result is False else session
 
-    if check_email is not None and credentials is not None:
-        credentials = None if check_email != credentials["email"] else credentials
+    if check_email is not None and session is not None:
+        session = None if check_email != session["email"] else session
 
-    if fernet is not None and credentials is not None:
-        credentials = decrypt(fernet, credentials)
+    if fernet is not None and session is not None:
+        session = decrypt(fernet, session)
 
-    return credentials
+    return session
 
 
 def signed_info_calculating(uuid: str, timestamp: int, shared_key: bool = False) -> str:
     """
     Pass the device_uuid when shared_key is False.
     """
     shared_key = Configs.YAY_SHARED_KEY if shared_key is True else ""
```

### Comparing `yaylib-1.0.2/yaylib.egg-info/PKG-INFO` & `yaylib-1.0.3/yaylib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaylib
-Version: 1.0.2
+Version: 1.0.3
 Summary: This Python package provides an easy-to-use interface for accessing data from Yay! (https://yay.space/). With this API Client, you can retrieve user profiles, posts, comments, and other content from Yay!, as well as perform common tasks like liking and commenting on posts.
 Home-page: https://github.com/qvco/yaylib
 Download-URL: https://github.com/qvco/yaylib
 Author: Qvco, Konn
 Author-email: nikola.desuga@gmail.com
 Maintainer: Qvco, Konn
 Maintainer-email: nikola.desuga@gmail.com
@@ -175,15 +175,15 @@
 
 timeline = api.get_timeline_by_keyword(
     keyword="プログラミング",
     number=15
 )
 
 for post in timeline.posts:
-    response = api.like_posts(post.id)
+    response = api.like(post.id)
     print(post.id, response.data) # 実行結果を出力
 ```
 
 #### ✨ タイムラインのユーザーをフォローする
 
 ```python
 import yaylib
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yaylib Version: 1.0.2 Summary: This Python package
+Metadata-Version: 2.1 Name: yaylib Version: 1.0.3 Summary: This Python package
 provides an easy-to-use interface for accessing data from Yay! (https://
 yay.space/). With this API Client, you can retrieve user profiles, posts,
 comments, and other content from Yay!, as well as perform common tasks like
 liking and commenting on posts. Home-page: https://github.com/qvco/yaylib
 Download-URL: https://github.com/qvco/yaylib Author: Qvco, Konn Author-email:
 nikola.desuga@gmail.com Maintainer: Qvco, Konn Maintainer-email:
 nikola.desuga@gmail.com License: MIT Keywords:
@@ -69,15 +69,15 @@
 print(post.text) # æ¬æ print(post.likes_count) # ããã­æ° print
 (post.reposts_count) # (Â´âï½â©)âageâã®æ° print
 (post.in_reply_to_post_count) # è¿ä¿¡ã®æ° ``` #### â¨
 ã¿ã¤ã ã©ã¤ã³ãã­ã¼ã¯ã¼ãã§æ¤ç´¢ãã¦ãããã­ããã
 ```python import yaylib api = yaylib.Client() api.login
 (email="ã¡ã¼ã«ã¢ãã¬ã¹", password="ãã¹ã¯ã¼ã") timeline =
 api.get_timeline_by_keyword( keyword="ãã­ã°ã©ãã³ã°", number=15 ) for
-post in timeline.posts: response = api.like_posts(post.id) print(post.id,
+post in timeline.posts: response = api.like(post.id) print(post.id,
 response.data) # å®è¡çµæãåºå ``` #### â¨
 ã¿ã¤ã ã©ã¤ã³ã®ã¦ã¼ã¶ã¼ããã©ã­ã¼ãã ```python import yaylib
 api = yaylib.Client() api.login(email="ã¡ã¼ã«ã¢ãã¬ã¹",
 password="ãã¹ã¯ã¼ã") timeline = api.get_timeline(number=15) for post in
 timeline.posts: api.follow_user(post.user.id) ```
 ããè©³ããä½¿ç¨ä¾ã«ã¤ãã¦ã¯ã[ãã¡ã](https://github.com/qvco/
 yaylib/blob/master/examples) ãåç§ãã¦ãã ããã
```

### Comparing `yaylib-1.0.2/yaylib.egg-info/SOURCES.txt` & `yaylib-1.0.3/yaylib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

