# Comparing `tmp/deta-1.1.0a3.tar.gz` & `tmp/deta-1.2.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deta-1.1.0a3.tar", last modified: Tue Mar  1 13:53:56 2022, max compression
+gzip compressed data, was "deta-1.2.0rc0.tar", last modified: Tue Jul 18 15:10:02 2023, max compression
```

## Comparing `deta-1.1.0a3.tar` & `deta-1.2.0rc0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 sif        (501) staff       (20)        0 2022-03-01 13:53:56.727410 deta-1.1.0a3/
--rw-r--r--   0 sif        (501) staff       (20)      383 2022-03-01 13:53:56.727245 deta-1.1.0a3/PKG-INFO
--rw-r--r--   0 sif        (501) staff       (20)      444 2021-09-17 09:09:22.000000 deta-1.1.0a3/README.md
-drwxr-xr-x   0 sif        (501) staff       (20)        0 2022-03-01 13:53:56.725937 deta-1.1.0a3/deta/
--rw-r--r--   0 sif        (501) staff       (20)     1937 2022-03-01 13:53:44.000000 deta-1.1.0a3/deta/__init__.py
-drwxr-xr-x   0 sif        (501) staff       (20)        0 2022-03-01 13:53:56.726915 deta-1.1.0a3/deta/_async/
--rw-r--r--   0 sif        (501) staff       (20)        0 2021-12-06 14:30:01.000000 deta-1.1.0a3/deta/_async/__init__.py
--rw-r--r--   0 sif        (501) staff       (20)     5725 2022-03-01 13:51:04.000000 deta-1.1.0a3/deta/_async/client.py
--rw-r--r--   0 sif        (501) staff       (20)     8331 2022-03-01 13:51:04.000000 deta-1.1.0a3/deta/base.py
--rw-r--r--   0 sif        (501) staff       (20)     6002 2022-03-01 13:51:04.000000 deta-1.1.0a3/deta/drive.py
--rw-r--r--   0 sif        (501) staff       (20)     3745 2022-03-01 13:51:04.000000 deta-1.1.0a3/deta/service.py
--rw-r--r--   0 sif        (501) staff       (20)      432 2022-03-01 13:51:04.000000 deta-1.1.0a3/deta/utils.py
-drwxr-xr-x   0 sif        (501) staff       (20)        0 2022-03-01 13:53:56.726674 deta-1.1.0a3/deta.egg-info/
--rw-r--r--   0 sif        (501) staff       (20)      383 2022-03-01 13:53:56.000000 deta-1.1.0a3/deta.egg-info/PKG-INFO
--rw-r--r--   0 sif        (501) staff       (20)      250 2022-03-01 13:53:56.000000 deta-1.1.0a3/deta.egg-info/SOURCES.txt
--rw-r--r--   0 sif        (501) staff       (20)        1 2022-03-01 13:53:56.000000 deta-1.1.0a3/deta.egg-info/dependency_links.txt
--rw-r--r--   0 sif        (501) staff       (20)        5 2022-03-01 13:53:56.000000 deta-1.1.0a3/deta.egg-info/top_level.txt
--rw-r--r--   0 sif        (501) staff       (20)       38 2022-03-01 13:53:56.727475 deta-1.1.0a3/setup.cfg
--rw-r--r--   0 sif        (501) staff       (20)      513 2022-03-01 13:53:11.000000 deta-1.1.0a3/setup.py
+drwxr-xr-x   0 sif        (501) staff       (20)        0 2023-07-18 15:10:02.245989 deta-1.2.0rc0/
+-rw-r--r--   0 sif        (501) staff       (20)      406 2023-07-18 15:10:02.245870 deta-1.2.0rc0/PKG-INFO
+-rw-r--r--   0 sif        (501) staff       (20)      456 2023-07-18 15:00:05.000000 deta-1.2.0rc0/README.md
+drwxr-xr-x   0 sif        (501) staff       (20)        0 2023-07-18 15:10:02.244947 deta-1.2.0rc0/deta/
+-rw-r--r--   0 sif        (501) staff       (20)     2189 2023-07-18 15:09:45.000000 deta-1.2.0rc0/deta/__init__.py
+drwxr-xr-x   0 sif        (501) staff       (20)        0 2023-07-18 15:10:02.245698 deta-1.2.0rc0/deta/_async/
+-rw-r--r--   0 sif        (501) staff       (20)        0 2021-12-06 14:30:01.000000 deta-1.2.0rc0/deta/_async/__init__.py
+-rw-r--r--   0 sif        (501) staff       (20)     5808 2023-07-18 15:09:46.000000 deta-1.2.0rc0/deta/_async/client.py
+-rw-r--r--   0 sif        (501) staff       (20)     8437 2023-07-18 15:09:46.000000 deta-1.2.0rc0/deta/base.py
+-rw-r--r--   0 sif        (501) staff       (20)     6002 2023-07-18 15:09:46.000000 deta-1.2.0rc0/deta/drive.py
+-rw-r--r--   0 sif        (501) staff       (20)     3745 2023-07-18 15:09:46.000000 deta-1.2.0rc0/deta/service.py
+-rw-r--r--   0 sif        (501) staff       (20)      432 2023-07-18 15:09:45.000000 deta-1.2.0rc0/deta/utils.py
+drwxr-xr-x   0 sif        (501) staff       (20)        0 2023-07-18 15:10:02.245490 deta-1.2.0rc0/deta.egg-info/
+-rw-r--r--   0 sif        (501) staff       (20)      406 2023-07-18 15:10:02.000000 deta-1.2.0rc0/deta.egg-info/PKG-INFO
+-rw-r--r--   0 sif        (501) staff       (20)      277 2023-07-18 15:10:02.000000 deta-1.2.0rc0/deta.egg-info/SOURCES.txt
+-rw-r--r--   0 sif        (501) staff       (20)        1 2023-07-18 15:10:02.000000 deta-1.2.0rc0/deta.egg-info/dependency_links.txt
+-rw-r--r--   0 sif        (501) staff       (20)       23 2023-07-18 15:10:02.000000 deta-1.2.0rc0/deta.egg-info/requires.txt
+-rw-r--r--   0 sif        (501) staff       (20)        5 2023-07-18 15:10:02.000000 deta-1.2.0rc0/deta.egg-info/top_level.txt
+-rw-r--r--   0 sif        (501) staff       (20)       38 2023-07-18 15:10:02.246028 deta-1.2.0rc0/setup.cfg
+-rw-r--r--   0 sif        (501) staff       (20)      526 2023-07-18 15:07:03.000000 deta-1.2.0rc0/setup.py
```

### Comparing `deta-1.1.0a3/deta/__init__.py` & `deta-1.2.0rc0/deta/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,20 @@
 try:
     from detalib.app import App
 
     app = App()
 except Exception:
     pass
 
-__version__ = "1.1.0a3"
+try:
+    from ._async.client import AsyncBase
+except ImportError:
+    pass
+
+__version__ = "1.2.0rc0"
 
 
 def Base(name: str):
     project_key, project_id = _get_project_key_id()
     return _Base(name, project_key, project_id)
 
 
@@ -33,14 +38,19 @@
         project_key, project_id = _get_project_key_id(project_key, project_id)
         self.project_key = project_key
         self.project_id = project_id
 
     def Base(self, name: str, host: str = None):
         return _Base(name, self.project_key, self.project_id, host)
 
+    def AsyncBase(self, name: str, host: str = None):
+        from ._async.client import _AsyncBase
+
+        return _AsyncBase(name, self.project_key, self.project_id, host)
+
     def Drive(self, name: str, host: str = None):
         return _Drive(
             name=name,
             project_key=self.project_key,
             project_id=self.project_id,
             host=host,
         )
```

### Comparing `deta-1.1.0a3/deta/_async/client.py` & `deta-1.2.0rc0/deta/_async/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,22 +120,26 @@
 
     async def fetch(
         self,
         query: typing.Union[dict, list] = None,
         *,
         limit: int = 1000,
         last: str = None,
+        desc: bool = False,
     ):
         payload = {}
         if query:
             payload["query"] = query if isinstance(query, list) else [query]
         if limit:
             payload["limit"] = limit
         if last:
             payload["last"] = last
+        if desc:
+            payload["sort"] = "desc"
+
         async with self._session.post(f"{self._base_url}/query", json=payload) as resp:
             resp_json = await resp.json()
             paging = resp_json.get("paging")
             return FetchResponse(paging.get("size"), paging.get("last"), resp_json.get("items"))
 
     async def update(
         self,
```

### Comparing `deta-1.1.0a3/deta/base.py` & `deta-1.2.0rc0/deta/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,39 +172,42 @@
         return res
 
     def _fetch(
         self,
         query: typing.Union[dict, list] = None,
         buffer: int = None,
         last: str = None,
+        desc: bool = False,
     ) -> typing.Optional[typing.Tuple[int, list]]:
         """This is where actual fetch happens."""
         payload = {
             "limit": buffer,
             "last": last if not isinstance(last, bool) else None,
+            "sort": "desc" if desc else "",
         }
 
         if query:
             payload["query"] = query if isinstance(query, list) else [query]
 
         code, res = self._request("/query", "POST", payload, content_type=JSON_MIME)
         return code, res
 
     def fetch(
         self,
         query: typing.Union[dict, list] = None,
         *,
         limit: int = 1000,
         last: str = None,
+        desc: bool = False,
     ):
         """
         fetch items from the database.
             `query` is an optional filter or list of filters. Without filter, it will return the whole db.
         """
-        _, res = self._fetch(query, limit, last)
+        _, res = self._fetch(query, limit, last, desc)
 
         paging = res.get("paging")
 
         return FetchResponse(paging.get("size"), paging.get("last"), res.get("items"))
 
     def update(
         self,
```

### Comparing `deta-1.1.0a3/deta/drive.py` & `deta-1.2.0rc0/deta/drive.py`

 * *Files identical despite different names*

### Comparing `deta-1.1.0a3/deta/service.py` & `deta-1.2.0rc0/deta/service.py`

 * *Files identical despite different names*

### Comparing `deta-1.1.0a3/setup.py` & `deta-1.2.0rc0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup
 
 setup(
     name="deta",
-    version="1.1.0a3",
+    version="1.2.0rc0",
     description="Python SDK for Deta Base & Deta Drive.",
     url="http://github.com/deta/deta-python",
     author="Deta",
     author_email="hello@deta.sh",
     license="MIT",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    packages=["deta"],
-    #extras_require={
-    #    "async": ["aiohttp>=3,<4"],
-    #},
+    packages=["deta", "deta._async"],
+    extras_require={
+        "async": ["aiohttp>=3,<4"],
+    },
 )
```

