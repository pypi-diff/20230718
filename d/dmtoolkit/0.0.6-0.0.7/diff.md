# Comparing `tmp/dmtoolkit-0.0.6.tar.gz` & `tmp/dmtoolkit-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmtoolkit-0.0.6.tar", last modified: Thu Jul 13 19:41:51 2023, max compression
+gzip compressed data, was "dmtoolkit-0.0.7.tar", last modified: Tue Jul 18 15:53:30 2023, max compression
```

## Comparing `dmtoolkit-0.0.6.tar` & `dmtoolkit-0.0.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-13 19:41:51.988709 dmtoolkit-0.0.6/
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1076 2023-06-20 14:10:02.000000 dmtoolkit-0.0.6/LICENSE
--rw-r--r--   0 samoore   (1000) samoore   (1000)     3453 2023-07-13 19:41:51.988709 dmtoolkit-0.0.6/PKG-INFO
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1745 2023-07-11 14:31:39.000000 dmtoolkit-0.0.6/README.md
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1230 2023-07-13 14:23:33.000000 dmtoolkit-0.0.6/pyproject.toml
--rw-r--r--   0 samoore   (1000) samoore   (1000)      339 2023-07-11 13:56:07.000000 dmtoolkit-0.0.6/requirements.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)       38 2023-07-13 19:41:51.988709 dmtoolkit-0.0.6/setup.cfg
--rw-r--r--   0 samoore   (1000) samoore   (1000)      835 2023-07-11 13:31:00.000000 dmtoolkit-0.0.6/setup.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-13 19:41:51.986709 dmtoolkit-0.0.6/src/
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-13 19:41:51.986709 dmtoolkit-0.0.6/src/dmtoolkit/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       52 2023-07-13 19:25:24.000000 dmtoolkit-0.0.6/src/dmtoolkit/__init__.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-13 19:41:51.987709 dmtoolkit-0.0.6/src/dmtoolkit/apis/
--rw-r--r--   0 samoore   (1000) samoore   (1000)      176 2023-07-13 19:03:53.000000 dmtoolkit-0.0.6/src/dmtoolkit/apis/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     8736 2023-07-11 11:33:46.000000 dmtoolkit-0.0.6/src/dmtoolkit/apis/dndbeyondapi.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      132 2023-06-22 17:00:22.000000 dmtoolkit-0.0.6/src/dmtoolkit/apis/foundryapi.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     5935 2023-07-13 19:16:15.000000 dmtoolkit-0.0.6/src/dmtoolkit/apis/open5eapi.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      727 2023-06-22 16:55:29.000000 dmtoolkit-0.0.6/src/dmtoolkit/apis/wikijsapi.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)    12497 2023-07-13 13:55:05.000000 dmtoolkit-0.0.6/src/dmtoolkit/dmtools.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-13 19:41:51.988709 dmtoolkit-0.0.6/src/dmtoolkit/models/
--rw-r--r--   0 samoore   (1000) samoore   (1000)      148 2023-06-28 13:29:24.000000 dmtoolkit-0.0.6/src/dmtoolkit/models/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1958 2023-07-13 16:05:59.000000 dmtoolkit-0.0.6/src/dmtoolkit/models/dndcharacter.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1311 2023-07-13 19:17:53.000000 dmtoolkit-0.0.6/src/dmtoolkit/models/dnditem.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2187 2023-07-13 19:17:18.000000 dmtoolkit-0.0.6/src/dmtoolkit/models/dndmonster.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1461 2023-07-13 19:04:40.000000 dmtoolkit-0.0.6/src/dmtoolkit/models/dndobject.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1092 2023-07-05 17:46:30.000000 dmtoolkit-0.0.6/src/dmtoolkit/models/dndshop.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1414 2023-07-13 19:17:37.000000 dmtoolkit-0.0.6/src/dmtoolkit/models/dndspell.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-13 19:41:51.987709 dmtoolkit-0.0.6/src/dmtoolkit.egg-info/
--rw-r--r--   0 samoore   (1000) samoore   (1000)     3453 2023-07-13 19:41:51.000000 dmtoolkit-0.0.6/src/dmtoolkit.egg-info/PKG-INFO
--rw-r--r--   0 samoore   (1000) samoore   (1000)      692 2023-07-13 19:41:51.000000 dmtoolkit-0.0.6/src/dmtoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)        1 2023-07-13 19:41:51.000000 dmtoolkit-0.0.6/src/dmtoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)      108 2023-07-13 19:41:51.000000 dmtoolkit-0.0.6/src/dmtoolkit.egg-info/requires.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)       10 2023-07-13 19:41:51.000000 dmtoolkit-0.0.6/src/dmtoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-18 15:53:30.877596 dmtoolkit-0.0.7/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1076 2023-06-20 14:10:02.000000 dmtoolkit-0.0.7/LICENSE
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     3453 2023-07-18 15:53:30.876596 dmtoolkit-0.0.7/PKG-INFO
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1745 2023-07-11 14:31:39.000000 dmtoolkit-0.0.7/README.md
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1230 2023-07-13 14:23:33.000000 dmtoolkit-0.0.7/pyproject.toml
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      339 2023-07-11 13:56:07.000000 dmtoolkit-0.0.7/requirements.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       38 2023-07-18 15:53:30.877596 dmtoolkit-0.0.7/setup.cfg
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      835 2023-07-11 13:31:00.000000 dmtoolkit-0.0.7/setup.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-18 15:53:30.864596 dmtoolkit-0.0.7/src/
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-18 15:53:30.869596 dmtoolkit-0.0.7/src/dmtoolkit/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       52 2023-07-18 15:53:15.000000 dmtoolkit-0.0.7/src/dmtoolkit/__init__.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-18 15:53:30.872596 dmtoolkit-0.0.7/src/dmtoolkit/apis/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      176 2023-07-13 19:03:53.000000 dmtoolkit-0.0.7/src/dmtoolkit/apis/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     8736 2023-07-11 11:33:46.000000 dmtoolkit-0.0.7/src/dmtoolkit/apis/dndbeyondapi.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      132 2023-06-22 17:00:22.000000 dmtoolkit-0.0.7/src/dmtoolkit/apis/foundryapi.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     6051 2023-07-18 15:47:28.000000 dmtoolkit-0.0.7/src/dmtoolkit/apis/open5eapi.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      727 2023-06-22 16:55:29.000000 dmtoolkit-0.0.7/src/dmtoolkit/apis/wikijsapi.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)    12497 2023-07-13 13:55:05.000000 dmtoolkit-0.0.7/src/dmtoolkit/dmtools.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-18 15:53:30.875596 dmtoolkit-0.0.7/src/dmtoolkit/models/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      148 2023-06-28 13:29:24.000000 dmtoolkit-0.0.7/src/dmtoolkit/models/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1794 2023-07-18 14:56:37.000000 dmtoolkit-0.0.7/src/dmtoolkit/models/dndcharacter.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      927 2023-07-18 15:06:01.000000 dmtoolkit-0.0.7/src/dmtoolkit/models/dnditem.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1803 2023-07-18 15:05:51.000000 dmtoolkit-0.0.7/src/dmtoolkit/models/dndmonster.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1421 2023-07-18 15:26:03.000000 dmtoolkit-0.0.7/src/dmtoolkit/models/dndobject.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1092 2023-07-05 17:46:30.000000 dmtoolkit-0.0.7/src/dmtoolkit/models/dndshop.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1030 2023-07-18 15:05:41.000000 dmtoolkit-0.0.7/src/dmtoolkit/models/dndspell.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-18 15:53:30.871596 dmtoolkit-0.0.7/src/dmtoolkit.egg-info/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     3453 2023-07-18 15:53:30.000000 dmtoolkit-0.0.7/src/dmtoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      692 2023-07-18 15:53:30.000000 dmtoolkit-0.0.7/src/dmtoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)        1 2023-07-18 15:53:30.000000 dmtoolkit-0.0.7/src/dmtoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      108 2023-07-18 15:53:30.000000 dmtoolkit-0.0.7/src/dmtoolkit.egg-info/requires.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       10 2023-07-18 15:53:30.000000 dmtoolkit-0.0.7/src/dmtoolkit.egg-info/top_level.txt
```

### Comparing `dmtoolkit-0.0.6/LICENSE` & `dmtoolkit-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.6/PKG-INFO` & `dmtoolkit-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmtoolkit
-Version: 0.0.6
+Version: 0.0.7
 Summary: A collection of AI based tools for D&D5e gMs.
 Author-email: Steven A Moore <samoore@binghamton.edu>
 License: MIT License
         
         Copyright (c) [2022] Steven Allen Moore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dmtoolkit-0.0.6/README.md` & `dmtoolkit-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.6/pyproject.toml` & `dmtoolkit-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.6/setup.py` & `dmtoolkit-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.6/src/dmtoolkit/apis/dndbeyondapi.py` & `dmtoolkit-0.0.7/src/dmtoolkit/apis/dndbeyondapi.py`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.6/src/dmtoolkit/apis/open5eapi.py` & `dmtoolkit-0.0.7/src/dmtoolkit/apis/open5eapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,22 @@
         results = response["results"]
         while response.get("next"):
             response = requests.get(response["next"]).json()
             results += response["results"]
         return [cls._build(r) for r in results]
 
     @classmethod
-    def search(cls, term, key="search", endpoint=""):
-        api_url = f"{cls.api_url}/{endpoint}"
-        response = requests.get(f"{api_url}?{key}={term}").json()
-        return [cls._build(r) for r in response["results"]]
+    def search(cls, terms, key="search", endpoint=""):
+        if not isinstance(terms, list):
+            terms = [terms]
+
+        for term in terms:
+            api_url = f"{cls.api_url}/{endpoint}"
+            response = requests.get(f"{api_url}?{key}={term}").json()
+            return [cls._build(r) for r in response["results"]]
 
     @classmethod
     def get(cls, url=None):
         if url:
             results = requests.get(url).json()
             return cls._build(results)
 
@@ -31,21 +35,21 @@
 class Open5eMonster(Open5e):
     @classmethod
     def all(cls):
         return super().all(endpoint="monsters")
 
     @classmethod
     def search(cls, term, key="search"):
-        return super().search(term=term, key=key, endpoint="monsters")
+        return super().search(terms=term, key=key, endpoint="monsters")
 
     @classmethod
     def _build(cls, data):
         obj = {}
         obj["name"] = data["name"]
-        obj["type"] = data["type"]
+        obj["type"] = data.get("type")
         obj["image"] = {"url": data.get("img_main"), "asset_id": 0, "raw": None}
         obj["size"] = data.get("size")
         obj["subtype"] = data.get("subtype")
         obj["alignment"] = data.get("alignment")
         obj["armor_class"] = data.get("armor_class")
         obj["armor_desc"] = data.get("armor_desc")
         obj["hit_points"] = data.get("hit_points")
@@ -92,15 +96,15 @@
 class Open5eSpell(Open5e):
     @classmethod
     def all(cls):
         return super().all(endpoint="spells")
 
     @classmethod
     def search(cls, term, key="search"):
-        return super().search(term=term, key=key, endpoint="spells")
+        return super().search(terms=term, key=key, endpoint="spells")
 
     @classmethod
     def _build(cls, data):
         obj = {}
         obj["name"] = data["name"]
         obj["school"] = data["school"]
         obj["desc"] = data["desc"]
@@ -154,9 +158,9 @@
             results += super().all(endpoint)
         return results
 
     @classmethod
     def search(cls, term, key="search"):
         results = []
         for endpoint in ["armor/", "weapons/", "magicitems/"]:
-            results += super().search(term=term, key=key, endpoint=endpoint)
+            results += super().search(terms=term, key=key, endpoint=endpoint)
         return results
```

### Comparing `dmtoolkit-0.0.6/src/dmtoolkit/apis/wikijsapi.py` & `dmtoolkit-0.0.7/src/dmtoolkit/apis/wikijsapi.py`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.6/src/dmtoolkit/dmtools.py` & `dmtoolkit-0.0.7/src/dmtoolkit/dmtools.py`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.6/src/dmtoolkit/models/dndcharacter.py` & `dmtoolkit-0.0.7/src/dmtoolkit/models/dndcharacter.py`

 * *Files 14% similar despite different names*

```diff
@@ -44,26 +44,19 @@
         else:
             data = DnDBeyondAPI.getcharacter(self.dnd_id)
 
             if results := self.table().find(dnd_id=self.dnd_id):
                 self.pk = results["pk"]
 
             if data["image"]["url"] and data["image"]["url"] != self.image.get("url"):
-                self.image = CloudinaryStorage().save(
-                    data["image"]["url"], folder=f"dnd/players/{slugify(self.name)}"
-                )
+                self.image = CloudinaryStorage().save(data["image"]["url"], folder=f"dnd/players/{slugify(self.name)}")
 
             del data["image"]
 
             self.__dict__.update(data)
             # log(self)
             self.save()
         return data
 
     def get_image_prompt(self):
         if self.image.get("url"):
             return f"A full color modern realism style portrait of a {self.race} character from Dungeons and Dragons aged {self.age} and described as {self.desc}"
-
-    @classmethod
-    def _update_db(cls, api=None):
-        for c in Character.search(npc=False):
-            c.updateinfo()
```

### Comparing `dmtoolkit-0.0.6/src/dmtoolkit/models/dnditem.py` & `dmtoolkit-0.0.7/src/dmtoolkit/models/dnditem.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from dmtoolkit.models.dndobject import DnDObject
 from dmtoolkit.apis import item_api
 from autonomous import log
 import markdown
 
 
 class Item(DnDObject):
+    search_api = item_api
     attributes = {
         "name": "",
         "image": {"url": "", "asset_id": 0, "raw": None},
         "desc": "",
         "rarity": "",
         "cost": 0,
         "attunement": False,
@@ -21,23 +22,10 @@
         "properties": [],
         "tables": [],
     }
 
     def __init__(self, **kwargs):
         self.desc_md = markdown.markdown(self.desc)
 
-    @classmethod
-    def search(cls, **kwargs):
-        results = super().search(**kwargs)
-        term = list(kwargs.values())[0]
-        api_results = item_api.search(term)
-        for r in api_results:
-            cc = filter(lambda x: r["slug"] == x.slug, results)
-            if not cc:
-                obj = cls(**r)
-                obj.save()
-                results.append(obj)
-        return results
-
     def get_image_prompt(self):
         description = self.__dict__.get("desc", "on display in the shop")
         return f"A full color Rusted Pixel style image of an item from Dungeons and Dragons 5e called {self.name}. Additional details:  {description}"
```

### Comparing `dmtoolkit-0.0.6/src/dmtoolkit/models/dndmonster.py` & `dmtoolkit-0.0.7/src/dmtoolkit/models/dndmonster.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from dmtoolkit.models.dndobject import DnDObject
 from dmtoolkit.apis import monster_api
 from autonomous import log
 import random
 
 
 class Monster(DnDObject):
+    search_api = monster_api
     attributes = {
         "name": "",
         "image": {"url": "", "asset_id": 0, "raw": None},
         "desc": "",
         "type": "",
         "size": "",
         "subtype": "",
@@ -40,27 +41,14 @@
         "challenge_rating": 0,
         "actions": [],
         "reactions": [],
         "special_abilities": [],
         "spell_list": [],
     }
 
-    @classmethod
-    def search(cls, **kwargs):
-        results = super().search(**kwargs)
-        term = list(kwargs.values())[0]
-        api_results = monster_api.search(term)
-        for r in api_results:
-            cc = filter(lambda x: r["slug"] == x.slug, results)
-            if not cc:
-                obj = cls(**r)
-                obj.save()
-                results.append(obj)
-        return results
-
     def get_image_prompt(self):
         description = self.__dict__.get("desc") or random.choice(
             [
                 "A renaissance portrait",
                 "An action movie poster",
                 "Readying for battle",
             ]
```

### Comparing `dmtoolkit-0.0.6/src/dmtoolkit/models/dndobject.py` & `dmtoolkit-0.0.7/src/dmtoolkit/models/dndobject.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,41 +6,39 @@
 from autonomous import log
 
 from slugify import slugify
 
 
 class DnDObject(AutoModel):
     _storage = CloudinaryStorage()
+    search_api = None
 
     @property
     def slug(self):
         return slugify(self.name)
 
     def save(self):
         if self.image.get("raw"):
             folder = f"dnd/{self.__class__.__name__.lower()}s/{self.slug}"
             self.image = self._storage.save(self.image["raw"], folder=folder)
         return super().save()
 
+    @classmethod
+    def search(cls, **kwargs):
+        results = super().search(**kwargs)
+        if cls.search_api:
+            names = {obj.name for obj in results}
+            api_results = cls.search_api.search(list(kwargs.values()))
+            results = [obj for obj in api_results if obj["name"] not in names and cls(**obj).save()]
+        return results
+
     def generate_image(self):
         resp = OpenAI().generate_image(
             self.get_image_prompt(),
             n=1,
         )
         folder = f"dnd/{self.__class__.__name__.lower()}s"
         self.image = self._storage.save(resp[0], folder=folder)
         return self.save()
 
     def get_image_prompt(self):
         return f"A full color portrait of a {self.name} from Dungeons and Dragons 5e - {self.desc}"
-
-    @classmethod
-    def _update_db(cls, api=None):
-        if api:
-            for updated_record in api.all():
-                if record := cls.find(slug=slugify(updated_record["name"])):
-                    record.__dict__.update(updated_record)
-                else:
-                    record = cls(**updated_record)
-
-                if not record.save():
-                    raise Exception(f"Failed to save {record}")
```

### Comparing `dmtoolkit-0.0.6/src/dmtoolkit/models/dndshop.py` & `dmtoolkit-0.0.7/src/dmtoolkit/models/dndshop.py`

 * *Files identical despite different names*

### Comparing `dmtoolkit-0.0.6/src/dmtoolkit.egg-info/PKG-INFO` & `dmtoolkit-0.0.7/src/dmtoolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmtoolkit
-Version: 0.0.6
+Version: 0.0.7
 Summary: A collection of AI based tools for D&D5e gMs.
 Author-email: Steven A Moore <samoore@binghamton.edu>
 License: MIT License
         
         Copyright (c) [2022] Steven Allen Moore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dmtoolkit-0.0.6/src/dmtoolkit.egg-info/SOURCES.txt` & `dmtoolkit-0.0.7/src/dmtoolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

