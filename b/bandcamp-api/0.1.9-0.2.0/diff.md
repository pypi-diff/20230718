# Comparing `tmp/bandcamp_api-0.1.9.tar.gz` & `tmp/bandcamp_api-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bandcamp_api-0.1.9.tar", last modified: Thu Jul  7 18:13:16 2022, max compression
+gzip compressed data, was "bandcamp_api-0.2.0.tar", last modified: Tue Jul 18 19:07:04 2023, max compression
```

## Comparing `bandcamp_api-0.1.9.tar` & `bandcamp_api-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0     1026 users      (100)        0 2022-07-07 18:13:15.992032 bandcamp_api-0.1.9/
--rwxrwxrwx   0     1026 users      (100)    35149 2022-07-07 18:13:02.459947 bandcamp_api-0.1.9/LICENSE
--rwxrwxrwx   0     1026 users      (100)      263 2022-07-07 18:13:15.991032 bandcamp_api-0.1.9/PKG-INFO
--rwxrwxrwx   0     1026 users      (100)      691 2022-07-07 18:11:51.000000 bandcamp_api-0.1.9/README.md
-drwxrwxrwx   0     1026 users      (100)        0 2022-07-07 18:13:15.935032 bandcamp_api-0.1.9/bandcamp_api/
--rwxrwxrwx   0     1026 users      (100)       34 2022-07-04 18:23:51.000000 bandcamp_api-0.1.9/bandcamp_api/__init__.py
--rwxrwxrwx   0     1026 users      (100)     9181 2022-07-07 17:13:49.000000 bandcamp_api-0.1.9/bandcamp_api/album.py
--rwxrwxrwx   0     1026 users      (100)     4363 2022-07-07 18:05:43.000000 bandcamp_api-0.1.9/bandcamp_api/artist.py
--rwxrwxrwx   0     1026 users      (100)     5271 2022-07-07 15:14:46.000000 bandcamp_api-0.1.9/bandcamp_api/bandcamp_api.py
--rwxrwxrwx   0     1026 users      (100)     1615 2022-06-12 16:16:10.000000 bandcamp_api-0.1.9/bandcamp_api/bandcampjson.py
--rwxrwxrwx   0     1026 users      (100)    10654 2022-07-04 18:35:21.000000 bandcamp_api-0.1.9/bandcamp_api/daily.py
--rwxrwxrwx   0     1026 users      (100)     1843 2022-07-04 18:35:44.000000 bandcamp_api-0.1.9/bandcamp_api/genres.py
--rwxrwxrwx   0     1026 users      (100)    14002 2022-07-05 04:36:54.000000 bandcamp_api-0.1.9/bandcamp_api/homepage.py
--rwxrwxrwx   0     1026 users      (100)     4660 2022-07-07 18:07:22.000000 bandcamp_api-0.1.9/bandcamp_api/label.py
--rwxrwxrwx   0     1026 users      (100)     6742 2022-07-04 16:05:29.000000 bandcamp_api-0.1.9/bandcamp_api/search.py
--rwxrwxrwx   0     1026 users      (100)     5138 2022-07-06 23:38:10.000000 bandcamp_api-0.1.9/bandcamp_api/track.py
-drwxrwxrwx   0     1026 users      (100)        0 2022-07-07 18:13:15.983032 bandcamp_api-0.1.9/bandcamp_api.egg-info/
--rwxrwxrwx   0     1026 users      (100)      263 2022-07-07 18:13:15.000000 bandcamp_api-0.1.9/bandcamp_api.egg-info/PKG-INFO
--rwxrwxrwx   0     1026 users      (100)      505 2022-07-07 18:13:15.000000 bandcamp_api-0.1.9/bandcamp_api.egg-info/SOURCES.txt
--rwxrwxrwx   0     1026 users      (100)        1 2022-07-07 18:13:15.000000 bandcamp_api-0.1.9/bandcamp_api.egg-info/dependency_links.txt
--rwxrwxrwx   0     1026 users      (100)        1 2022-07-07 18:13:02.000000 bandcamp_api-0.1.9/bandcamp_api.egg-info/not-zip-safe
--rwxrwxrwx   0     1026 users      (100)       38 2022-07-07 18:13:15.000000 bandcamp_api-0.1.9/bandcamp_api.egg-info/requires.txt
--rwxrwxrwx   0     1026 users      (100)       13 2022-07-07 18:13:15.000000 bandcamp_api-0.1.9/bandcamp_api.egg-info/top_level.txt
--rwxrwxrwx   0     1026 users      (100)       38 2022-07-07 18:13:15.994032 bandcamp_api-0.1.9/setup.cfg
--rwxrwxrwx   0     1026 users      (100)      378 2022-07-07 18:12:29.000000 bandcamp_api-0.1.9/setup.py
+drwxr-xr-x   0 rin        (501) staff       (20)        0 2023-07-18 19:07:04.022663 bandcamp_api-0.2.0/
+-rwxr-xr-x   0 rin        (501) staff       (20)    35149 2023-05-26 17:47:35.000000 bandcamp_api-0.2.0/LICENSE
+-rw-r--r--   0 rin        (501) staff       (20)      218 2023-07-18 19:07:04.022485 bandcamp_api-0.2.0/PKG-INFO
+-rwxr-xr-x   0 rin        (501) staff       (20)      678 2023-07-18 18:48:37.000000 bandcamp_api-0.2.0/README.md
+drwxr-xr-x   0 rin        (501) staff       (20)        0 2023-07-18 19:07:04.021474 bandcamp_api-0.2.0/bandcamp_api/
+-rwxr-xr-x   0 rin        (501) staff       (20)       34 2023-05-26 17:47:35.000000 bandcamp_api-0.2.0/bandcamp_api/__init__.py
+-rw-r--r--   0 rin        (501) staff       (20)     9181 2023-07-18 18:48:37.000000 bandcamp_api-0.2.0/bandcamp_api/album.py
+-rw-r--r--   0 rin        (501) staff       (20)     1363 2023-07-18 18:48:37.000000 bandcamp_api-0.2.0/bandcamp_api/artist.py
+-rw-r--r--   0 rin        (501) staff       (20)     7118 2023-07-18 18:48:37.000000 bandcamp_api-0.2.0/bandcamp_api/bandcamp_api.py
+-rwxr-xr-x   0 rin        (501) staff       (20)     1615 2023-05-26 17:47:35.000000 bandcamp_api-0.2.0/bandcamp_api/bandcampjson.py
+-rwxr-xr-x   0 rin        (501) staff       (20)    10654 2023-05-26 17:47:35.000000 bandcamp_api-0.2.0/bandcamp_api/daily.py
+-rwxr-xr-x   0 rin        (501) staff       (20)     1846 2023-07-18 18:48:37.000000 bandcamp_api-0.2.0/bandcamp_api/genres.py
+-rwxr-xr-x   0 rin        (501) staff       (20)    14004 2023-07-18 18:48:37.000000 bandcamp_api-0.2.0/bandcamp_api/homepage.py
+-rwxr-xr-x   0 rin        (501) staff       (20)     2618 2023-07-18 18:48:37.000000 bandcamp_api-0.2.0/bandcamp_api/label.py
+-rw-r--r--   0 rin        (501) staff       (20)     6226 2023-07-18 18:48:37.000000 bandcamp_api-0.2.0/bandcamp_api/search.py
+-rwxr-xr-x   0 rin        (501) staff       (20)     5540 2023-07-18 18:48:37.000000 bandcamp_api-0.2.0/bandcamp_api/track.py
+drwxr-xr-x   0 rin        (501) staff       (20)        0 2023-07-18 19:07:04.022274 bandcamp_api-0.2.0/bandcamp_api.egg-info/
+-rw-r--r--   0 rin        (501) staff       (20)      218 2023-07-18 19:07:03.000000 bandcamp_api-0.2.0/bandcamp_api.egg-info/PKG-INFO
+-rw-r--r--   0 rin        (501) staff       (20)      505 2023-07-18 19:07:03.000000 bandcamp_api-0.2.0/bandcamp_api.egg-info/SOURCES.txt
+-rw-r--r--   0 rin        (501) staff       (20)        1 2023-07-18 19:07:03.000000 bandcamp_api-0.2.0/bandcamp_api.egg-info/dependency_links.txt
+-rw-r--r--   0 rin        (501) staff       (20)        1 2023-07-18 19:07:03.000000 bandcamp_api-0.2.0/bandcamp_api.egg-info/not-zip-safe
+-rw-r--r--   0 rin        (501) staff       (20)       58 2023-07-18 19:07:03.000000 bandcamp_api-0.2.0/bandcamp_api.egg-info/requires.txt
+-rw-r--r--   0 rin        (501) staff       (20)       13 2023-07-18 19:07:03.000000 bandcamp_api-0.2.0/bandcamp_api.egg-info/top_level.txt
+-rw-r--r--   0 rin        (501) staff       (20)       38 2023-07-18 19:07:04.022704 bandcamp_api-0.2.0/setup.cfg
+-rwxr-xr-x   0 rin        (501) staff       (20)      401 2023-07-18 19:06:41.000000 bandcamp_api-0.2.0/setup.py
```

### Comparing `bandcamp_api-0.1.9/LICENSE` & `bandcamp_api-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bandcamp_api-0.1.9/README.md` & `bandcamp_api-0.2.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -11,11 +11,11 @@
 ```python
 from bandcamp_api import Bandcamp
 
 bc = Bandcamp()
 
 album = bc.get_album(album_url="https://c418.bandcamp.com/album/minecraft-volume-alpha")
 
-print("Album title: " + album.album_title)
+print("Album title:", album.album_title)
 ```
 
-For more information on the functions available see the [functions wiki](https://github.com/RustyRin/bandcamp-api/wiki/Bandcamp-api-Objects) or the [object wiki](https://github.com/RustyRin/bandcamp-api/wiki/Bandcamp-api-Objects)
+For more information on the functions available see the [functions wiki](https://github.com/RustyRin/bandcamp-api/wiki/Functions) or the [object wiki](https://github.com/RustyRin/bandcamp-api/wiki/Bandcamp-api-Objects)
```

### Comparing `bandcamp_api-0.1.9/bandcamp_api/album.py` & `bandcamp_api-0.2.0/bandcamp_api/daily.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,266 +1,290 @@
-import json
 import requests
-from bs4 import BeautifulSoup
-from bs4 import FeatureNotFound
-from datetime import datetime
-import time
-
+from bs4 import BeautifulSoup, FeatureNotFound
 import logging
-
+import json
 from .bandcampjson import BandcampJSON
-from .track import Track
-
-class Album:
-
-    def __init__(self, album_url, debugging: bool = False, skip_track_scrape: bool = False):
-        self.album_title = ""
-        self.artist_title = ""
-        self.tracks = []
-        self.art_url = ""
-        self.album_url = ""
-        self.artist_url = ""
-        self.all_songs_available = False
-        self.price = {}
-        self.keywords = []
-        self.publisher_title = ""
-        self.preorder = False
+from datetime import datetime
+import time
 
-        # need to do
-        self.album_bio = ""
+def string_clean(input_string):
+    return ' '.join(input_string.split())
 
-        self.date_released = 0    # utc unixtime
-        self.date_published = 0  # utc unixtime
+class Daily():
+    def __init__(Bandcamp):
+       """Bandcamp Daily"""
+
+    def search_latest(self, num_to_get: int):
+        """Gets the latests stories form the Bandcamp Daily
+        :param num_to_get: The number of BCDaily posts to return. Will allways return an array of article links."""
+        page = 1
+        url = "https://daily.bandcamp.com/latest?page="
+        posts_obtained = []
+        header = {'User-Agent': 'bandcamp-api/0 (https://github.com/RustyRin/bandcamp-api)'}
+        while True:
+            try:
+                response = requests.get(url=url + str(page), headers=header)
+            except requests.exceptions.MissingSchema as Err:
+                return Err
+            
+            try:
+                soup = BeautifulSoup(response.text, "lxml")
+            except FeatureNotFound:
+                soup = BeautifulSoup(response.text, "html.parser")
+
+            articles = soup.find("articles-list")
+            try:
+                articles = articles.find_all('div', {"class": "title-wrapper"})
+                #list = []
+
+                for article in articles:
+                    if len(posts_obtained) < num_to_get:
+                        posts_obtained.append("https://daily.bandcamp.com" + article.find('a').get('href'))
+                    else:
+                        return posts_obtained
+            except:
+                return posts_obtained
+
+            page += 1
+
+    def search_best_of(self, section_slug: str, num_to_get: int):
+        """Seach for BCDaily posts in the Best Of section.
+        :param section_slug: The URL slug of the section you want. Example for Best of 2016: 'best-of-2016'
+        :param num_to_get: The number of BCDaily posts to return. Will allways return an array of article links."""
+        header = {'User-Agent': 'bandcamp-api/0 (https://github.com/RustyRin/bandcamp-api)'}
+        url = "https://daily.bandcamp.com/"
+        page = 1
+        posts_obtained = []
+
+        while True:
+            try:
+                response = requests.get(url=url + section_slug  + '?page=' + str(page), headers=header)
+            except requests.exceptions.MissingSchema:
+                return ""
+            
+            try:
+                soup = BeautifulSoup(response.text, "lxml")
+            except FeatureNotFound:
+                soup = BeautifulSoup(response.text, "html.parser")
+
+            articles = soup.find("articles-list")
+            try:
+                articles = articles.find_all('div', {"class": "title-wrapper"})
+
+                for article in articles:
+                    if len(posts_obtained) < num_to_get:
+                        posts_obtained.append("https://daily.bandcamp.com" + article.find('a').get('href'))
+                    else:
+                        return posts_obtained
+            except:
+                return posts_obtained
+
+            page += 1
+            print("Going to page " + str(page))
+                
+
+
+
+    def search_franchises(self, section_slug: str, num_to_get: int):
+        """Seach the BCDaily in the Franchises section.
+        :param section_slug: The URL slug of the section you want. Example for Album Of The Day: album-of-the-day
+        :param num_to_get: The number of BCDaily posts to return. Will allways return an array of article links."""
+        header = {'User-Agent': 'bandcamp-api/0 (https://github.com/RustyRin/bandcamp-api)'}
+        url = "https://daily.bandcamp.com/"
+        page = 1
+        posts_obtained = []
+
+        while True:
+            try:
+                response = requests.get(url=url + section_slug  + '?page=' + str(page), headers=header)
+            except requests.exceptions.MissingSchema:
+                return ""
+            
+            try:
+                soup = BeautifulSoup(response.text, "lxml")
+            except FeatureNotFound:
+                soup = BeautifulSoup(response.text, "html.parser")
+
+            articles = soup.find("articles-list")
+            try:
+                articles = articles.find_all('div', {"class": "title-wrapper"})
+
+                for article in articles:
+                    if len(posts_obtained) < num_to_get:
+                        posts_obtained.append("https://daily.bandcamp.com" + article.find('a').get('href'))
+                    else:
+                        return posts_obtained
+            except:
+                return posts_obtained
+
+            page += 1
+
+    def search_genre(self, genre_slug: str, num_to_get: int):
+        """Search the BCDail in the Genre section.
+        :param genre_slug: The URL slug of the genre you want. Example for R&B/Soul: r-b-soul
+        :param num_to_get: The number of BCDaily posts to return. Will allways return an array of article links."""
+        header = {'User-Agent': 'bandcamp-api/0 (https://github.com/RustyRin/bandcamp-api)'}
+        url = "https://daily.bandcamp.com/genres/"
+        page = 1
+        posts_obtained = []
+
+        while True:
+            try:
+                response = requests.get(url=url + genre_slug  + '?page=' + str(page), headers=header)
+            except requests.exceptions.MissingSchema:
+                return ""
+            
+            try:
+                soup = BeautifulSoup(response.text, "lxml")
+            except FeatureNotFound:
+                soup = BeautifulSoup(response.text, "html.parser")
+
+            try:
+                articles = soup.find("articles-list")
+                articles = articles.find_all('div', {"class": "title-wrapper"})
+                list = []
+
+                for article in articles:
+                    if len(posts_obtained) < num_to_get:
+                        posts_obtained.append("https://daily.bandcamp.com/genres" + article.find('a').get('href'))
+                    else:
+                        return posts_obtained
+            except:
+                return posts_obtained
+
+            page += 1        
+
+def get_json(url, debugging: bool = False):
+
+    header = {'User-Agent': f'bandcamp-api/0 (https://github.com/RustyRin/bandcamp-api)'}
+
+    try:
+        response = requests.get(url, headers=header)
+    except requests.exceptions.MissingSchema:
+        return ""
+    
+    try:
+        soup = BeautifulSoup(response.text, "lxml")
+    except FeatureNotFound:
+        soup = BeautifulSoup(response.text, "html.parser")
+
+    logging.debug(" Generating JSON...")
+
+    bandcamp_json = BandcampJSON(soup, debugging).generate()
+    page_json = {}
+    for entry in bandcamp_json:
+        page_json = {**page_json, **json.loads(entry)}
+
+    logging.debug(' Bandcamp JSON generated...')
+
+    return page_json
+
+class Story():
+    def __init__(self, story_url: str):
+        self.title = ""
+        self.author = ""
+        self.description = ""
+        self.headline = ""
+        self.main_image_url = ""
+        self.story_type = ""
+        self.linked_in_text = []
+        self.linked_media = []
+        self.text = ""
+        self.date_published = 0
         self.date_last_modified = 0
+        self.images = []        # look for story with multiple images
+        self.tags = []
 
-        # extra, ignore
-        self.soup = None
-
-        # This stuff seems *minor* so I'm just
-        # going to use a dict, if this is a problem
-        # for you I'm sure you're smart enough to
-        # fix it or make it better
-        self.advanced = {
-            "copyright": "",
-            "ids": {
-                "artist_id": 0,
-                "album_id": 0,
-                "art_id": 0,
-                "seller_id": 0,
-            },
-            "featured_track": 0,
-            "email_required": False,
-            "reviews": [],
-            "supporters": []
-        }
+        response = requests.get(story_url)
 
         try:
-            page_json = self.get_json(url = album_url)
-
+            page_json = get_json(url = story_url)
         except Exception as err:
             print(err)
-            raise AttributeError("Either the album URL given is either private, deleted or the link is malformed.")
-
-        self.artist_title = page_json['artist']
-        self.artist_title = ' '.join(self.artist_title.split())
-
-        try:
-            self.album_title = page_json['current']['title']
-            self.album_title = ' '.join(self.album_title.split())
-        except:
-            self.album_title = page_json['trackinfo'][0]['title']
-
-        self.album_url = album_url
-
-        # getting artist url
-        if 'track' in page_json['url']:
-            self.artist_url = page_json['url'].rpartition('/track/')[0]
-        else:
-            self.artist_url = page_json['url'].rpartition('/album')[0]
-
-        if skip_track_scrape == False:
-            for trackjson in page_json['trackinfo']:
-                try:
-                    track = Track(str(self.artist_url + trackjson['title_link']))
-                    self.tracks.append(track)
-                except:
-                    pass
-        else: 
-            for trackjson in page_json['trackinfo']:
-                try:
-                    self.tracks.append(str(self.artist_url + trackjson['title_link']))
-                except:
-                    pass
-
-        self.all_songs_available = self.are_all_songs_available(page_json['trackinfo'])
-
-        self.art_url = 'https://f4.bcbits.com/img/a' + str(page_json['current']['art_id']) + '_0.jpg'
-
-        self.keywords = page_json['keywords']
-
-        self.publisher = page_json['publisher']['@id']
-
-        if page_json['current']['about'] != None:
-            self.album_bio = page_json['current']['about']
-
-        # currently some albums get a time of 0, need to look if there are
-        # some other places to find the released and publish times.
-        try:
-            self.date_released = datetime.strptime(page_json['album_release_date'], '%d %b %Y %H:%M:%S %Z')
-            self.date_released = int(time.mktime(self.date_released.timetuple()))
-        except:
-            self.date_released = 0
+            raise AttributeError("Either the Artist URL gicen is either private, deleted or the link is malformed")
         
         try:
-            self.date_published = datetime.strptime(page_json['datePublished'], '%d %b %Y %H:%M:%S %Z')
-            self.date_published = int(time.mktime(self.date_published.timetuple()))
-        except:
-            self.date_published = 0
-
+            soup = BeautifulSoup(response.text, "lxml")
+        except FeatureNotFound:
+            soup = BeautifulSoup(response.text, "html.parser")
+        
         try:
-            self.price['amount'] = float(page_json["current"]["minimum_price"])
-            self.price['currency'] = page_json['albumRelease'][0]['offers']['priceCurrency']
-        except:
-            self.price = None
+            soup = BeautifulSoup(response.text, "lxml")
+        except FeatureNotFound:
+            soup = BeautifulSoup(response.text, "html5lib")
 
-        try:
-            self.preorder = bool(page_json['album_is_preorder'])
-        except:
-            self.preorder = False
+        self.title = string_clean(soup.find('article-title').text)
 
+        self.author = soup.find('article-credits')
+        self.author = string_clean(self.author.find('a').text)
 
-        # doing the "advanced"
-        try:
-            self.advanced['copyright'] = page_json['copyrightNotice']
-        except:
-            self.advanced['copyright'] = ""
+        self.story_type = string_clean(soup.find('article-type').text.lower())
+        body = soup.find('article')
+        body = body.find_all('p')
 
-        try:
-            self.date_last_modified = datetime.strptime(page_json['dateModified'], '%d %b %Y %H:%M:%S %Z')
-            self.date_last_modified = int(time.mktime(self.date_last_modified.timetuple()))
-        except:
-            self.advanced['last_edited'] = self.date_published
+        for section in body:
+            for link in section.find_all('a'):
+                #self.linked_in_text.append(link.absolute_links.pop())
+                self.linked_in_text.append(link.get('href'))
+            if string_clean(section.text):
+                self.text = self.text + string_clean(section.text) + '\n\n'                
 
-        self.advanced['ids']['artist_id'] = page_json['current']['band_id']
-        self.advanced['ids']['album_id'] = page_json['id']
-        self.advanced['ids']['art_id'] = page_json['current']['art_id']
-        self.advanced['ids']['seller_id'] = page_json['current']['selling_band_id']
-        try:
-            self.advanced['featured_track'] = page_json['additionalProperty'][1]["value"]
-        except:
-            self.advanced['featured_track'] = 0
+        players = soup.find_all("div", {"class": "player-wrapper"})
 
-        if page_json['current']['require_email'] != None:
-            self.advanced['email_required'] = page_json['current']['require_email']
-        else:
-            self.advanced['email_required'] = False
-        
-        try:
-            for review in page_json['comment']:
-                current_review = {}
-                try:
-                    current_review["username"] = str(review['author']['name'])
-                    current_review['username'] =  ' '.join( current_review["username"].split())
-                except:
-                    current_review["username"] = ""
-
-                current_review['profile_url'] = review['author']['url']
-
-                current_review['profile_picture'] = review['author']['image']
-                current_review['profile_picture'] = current_review['profile_picture'].split('_')[0] + '_0.jpg'
-
-                current_review['review'] = str(review['text'][0])
-                current_review['review'] = ' '.join(current_review['review'].split())
-                try:
-                    current_review['favorite_track'] = str(review['text'][1].split(": ")[1])
-                except:
-                    current_review['favorite_track'] = ""
 
-                self.advanced['reviews'].append(current_review)
-        except:
-            pass
+        '''
+        I wanted to make a thing
+        to get songs that were featured
+        in a BCD story, but a large amount
+        of the information is rendered
+        in JS, I tried to get it with
+        requests-html and its render
+        funtion but could not get it
+        to work propery. Sorry.
+        '''
 
         try:
-            for supporter in page_json['sponsor']:
-                try:
-                    current_supporter = {}
-
-                    current_supporter['username'] = supporter['name']
-                    current_supporter['profile_url'] = supporter['url']
-                    current_supporter['profile_picture'] = supporter['image'].split('_')[0] + '_0.jpg'
-
-                    self.advanced['supporters'].append(current_supporter)
-                except:
-                    pass
+            self.date_published = datetime.strptime(page_json['datePublished'], '%Y-%m-%dT%H:%M:%SZ')
+            self.date_published = int(time.mktime(self.date_published.timetuple()))
         except:
-            pass
-    
-    # other methods
-    # need to organize the order of methods
-    @staticmethod
-    def generate_album_url(artist: str, slug: str, page_type: str) -> str:
-        """Generate an album url based on the artist and album name
-
-        :param artist: artist name
-        :param slug: Slug of album/track
-        :param page_type: Type of page album/track
-        :return: url as str
-        """
-        return f"http://{artist}.bandcamp.com/{page_type}/{slug}"
-
-    def get_album_art(self) -> str:
-        """Find and retrieve album art url from page
+            self.published = 0
 
-        :return: url as str
-        """
         try:
-            url = self.soup.find(id='tralbumArt').find_all('a')[0]['href']
-            return url
-        except None:
-            pass
+            self.date_last_modified = datetime.strptime(page_json['dateModified'], '%Y-%m-%dT%H:%M:%SZ')
+            self.date_last_modified = int(time.mktime(self.advanced['last_edited'].timetuple()))
+        except:
+            self.date_last_modified = self.date_published
 
-    def get_json(self, url, debugging: bool = False):
+        self.description = page_json['description']
 
-        headers = {'User-Agent': f'bandcamp-api/0 (https://github.com/RustyRin/bandcamp-api)'}
+        self.headline = page_json['headline']
 
-        try:
-            response = requests.get(url, headers=headers)
-        except requests.exceptions.MissingSchema:
-            return None
+        self.main_image_url = page_json['image']
 
-        try:
-            self.soup = BeautifulSoup(response.text, "lxml")
-        except FeatureNotFound:
-            self.soup = BeautifulSoup(response.text, "html.parser")
-
-        logging.debug(" Generating BandcampJSON..")
-        bandcamp_json = BandcampJSON(self.soup, debugging).generate()
-        page_json = {}
-        for entry in bandcamp_json:
-            page_json = {**page_json, **json.loads(entry)}
-        logging.debug(" BandcampJSON generated..")
-
-        return page_json
-
-    def are_all_songs_available(self, tracks):
-        for track in tracks:
-            if (track['file'] is None or False):
-                return False
+        '''
+        bandcamp does not seem to have a standard way
+        to deal with images
+        sometimes its in a gallery class
+        sometimes its in an inline class
+        sometimes its just laying there
 
-        return True
+        so i am loading the entire article body
+        then deleting all music, artist and merch
+        that is all on the side
+        '''
+        body = soup.find('article')
 
-    def get_track_lyrics(self, track_url = None):
-        track_page = requests.get(track_url, headers=None)
+        artists = body.find_all("mplayer-artist")       # artists
+        for artist in artists:
+            artist.decompose()
+        players = body.find_all('mplayer')              # players
+        for player in players:
+            player.decompose()
+        all_merch = body.find_all('mplayer-sidebar')    # merch
+        for merch in all_merch:
+            merch.decompose()
 
-        try:
-            track_soup = BeautifulSoup(track_page.text, 'lxml')
-        except FeatureNotFound:
-            track_page = BeautifulSoup(track_page.text, 'html.parser')
-        try:
-            track_lyrics = track_soup.find('div', {'class': 'lyricsText'})
-        except:
-            return ''
+        for photo in body.find_all('img'):
+            if photo.get('src') is not None:
+                self.images.append(photo.get('src'))
 
-        if track_lyrics:
-            return track_lyrics.text
-        else:
-            return ''
+        self.tags = page_json['keywords'].split(', ')
```

### Comparing `bandcamp_api-0.1.9/bandcamp_api/bandcampjson.py` & `bandcamp_api-0.2.0/bandcamp_api/bandcampjson.py`

 * *Files identical despite different names*

### Comparing `bandcamp_api-0.1.9/bandcamp_api/genres.py` & `bandcamp_api-0.2.0/bandcamp_api/genres.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from .bandcampjson import BandcampJSON
 from bs4 import BeautifulSoup, FeatureNotFound
 import requests
 import logging
 import json
 
+
 def get_json(url, debugging: bool = False):
 
         headers = {'User-Agent': f'bandcamp-api/0 (https://github.com/RustyRin/bandcamp-api)'}
 
         try:
             response = requests.get(url, headers=headers)
         except requests.exceptions.MissingSchema:
@@ -23,28 +24,30 @@
         page_json = {}
         for entry in bandcamp_json:
             page_json = {**page_json, **json.loads(entry)}
         logging.debug(" BandcampJSON generated..")
 
         return page_json
 
+
 def get_main_genres():
     try:
         page_json = get_json(url="https://intlanthem.bandcamp.com/album/in-these-times")
     except Exception as err:
         print("Error getting the sample album for the genres")
         print(err)
         raise AttributeError
 
     genres = []
     for genre_dict in page_json['signup_params']['genres']:
         genres.append(genre_dict['value'])
 
     return genres
 
+
 def get_subgenres(main_genre: str):
 
     if main_genre == "" or main_genre == None:
         raise Exception('Main genre slug was not provided')
     
     try:
         page_json = get_json(url="https://intlanthem.bandcamp.com/album/in-these-times")
```

### Comparing `bandcamp_api-0.1.9/bandcamp_api/homepage.py` & `bandcamp_api-0.2.0/bandcamp_api/homepage.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     for entry in bandcamp_json:
         page_json = {**page_json, **json.loads(entry)}
 
     logging.debug(' Bandcamp JSON generated...')
 
     return page_json
 
+
 def get_current_new_and_notable_id():
     ping_size = 7          # how many guesses should be do per get/ping, max 60
     check_width = 7        # how many future IDs should be checked if they exist
     highest_known = 1835    # the highest number that got a response
     lowest_unknown = 999999      # the lowest seen number that got a response
     latest_id = None
 
@@ -46,15 +47,14 @@
 
         currently_guessing = []
 
         try:
             currently_guessing = random.sample(range(highest_known, lowest_unknown), ping_size)
         except:
             currently_guessing = random.sample(range(highest_known - check_width, lowest_unknown + check_width), ping_size)
-        
 
         # get information
         id_string = ''
         for id in currently_guessing:
             id_string += str(id) + ','
         r = requests.get('https://bandcamp.com/api/notabletralbum/2/get?id=' + id_string)
 
@@ -83,14 +83,15 @@
             else:
                 # it is empty
                 if id < lowest_unknown:
                     lowest_unknown = id
 
     return latest_id
 
+
 class NewAndNotable():
 
     def __init__(self, num_to_get: int = 5):
         self.albums = []
 
         current_id = get_current_new_and_notable_id()
         #ids = []
@@ -128,61 +129,62 @@
             album.advanced['band_id'] = entry['band_id']
             album.advanced['album_id'] = entry['tralbum_id']
             album.advanced['art_id'] = entry['art_id']
             album.advanced['featured_track_id'] = entry['featured_track_id']
 
             self.albums.append(album)
 
+
 class NewAndNotableAlbum():
     def __init__(self):
 
         self.album_artist = ""
         self.album_title = ""
         self.album_art = ""
         self.album_url = ""
         self.genre = ""
         self.date_published = 0
         self.date_last_modified = 0
         self.description = ""
         self.advanced = {}
 
         
-class Charts():
-
-    def __init__(self, 
-                main_genre: str = "all", 
-                sort: str = "top", 
-                page: int = 0, 
-                format: str = 'all', 
-                subgenre: str = ""):
+class Charts:
+    def __init__(
+            self,
+            main_genre: str = "all",
+            sort: str = "top",
+            page: int = 0,
+            format: str = 'all',
+            subgenre: str = ""):
 
         self.albums = []
 
         if not main_genre:
             main_genre = "all"
 
         if not sort:
             sort = 'top'
 
-        if page == None or not page:
+        if page is None or not page:
             page = 0
 
         if not format:
             format = 'all'
 
         if not subgenre:
             subgenre = ""
 
         arg_string = ""
 
         arg_string += 'g=' + main_genre
 
         arg_string += '&s=' + sort
 
-        if (main_genre) != 'all' and ('rec' not in sort):
+        if main_genre != 'all' and ('rec' not in sort):
             # can contain subgenre
             arg_string += '&t=' + subgenre
 
         if 'rec' not in sort:
             # can contain format
             arg_string += '&f=' + format
         else:
@@ -237,29 +239,29 @@
                 "album_id": current_album['id'],
                 "art_id": current_album['art_id'],
                 "bio_image_id": current_album['bio_image']['image_id']
             }
 
             self.albums.append(album)
 
-class ChartsAlbum():
 
+class ChartsAlbum:
     def __init__(self):
         self.album_artist = ""
         self.album_title = ""
         self.artist_url = ""
         self.album_url = ""
         self.genre = ""
         self.artist_location = ""
         self.date_published = 0
         self.featured_track = {}
         self.advanced = {}
 
-class SaleFeed():
 
+class SaleFeed:
     def __init__(self, time: int = 0):
 
         self.sold_time = 0.00000
         #self.artist = ""
         self.purchases = []
         if time == 0:
             # looks like they didnt give a start time
@@ -303,32 +305,35 @@
                 else:
                     item.image_url = "https://f4.bcbits.com/img/a" + str(current_item['art_id']) +"_0.jpg"
                 bought_items.append(item)
 
             self.purchases.append(bought_items)
 
         
-class Item():
+class Item:
     def __init__(self):
         self.price = {}
-            # paid
-            # price
-            # currency
+        # {
+        #   "price": 0.00,
+        #   "paid": 0.00,
+        #   "currency": "USD"
+        # }
         self.image_url = ""
 
         self.description = ""
 
         self.type = ""
-            # t for track
-            # p seems to be for physical
-            # a for album
-            # b is full disco
+        # t for track
+        # p seems to be for physical
+        # a for album
+        # b is full disco
 
         self.url = ""
 
+
 class BandcampWeekly():
 
     def __init__(self):
 
         # time
         self.date_released = 0
         self.date_published = 0
@@ -425,14 +430,15 @@
             
             track_object.start_timecode = track['timecode']
 
             self.tracks.append(track_object)
 
         return self
 
+
 class BandcampWeeklyTrack():
 
     def __init__(self):
         self.art_url = ""
         self.album_title = ""
         self.label_title = ""
         self.price = {}
```

