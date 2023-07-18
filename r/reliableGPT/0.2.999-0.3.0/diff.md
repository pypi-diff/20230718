# Comparing `tmp/reliableGPT-0.2.999.tar.gz` & `tmp/reliableGPT-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliableGPT-0.2.999.tar", last modified: Fri Jul 14 04:20:24 2023, max compression
+gzip compressed data, was "reliableGPT-0.3.0.tar", last modified: Fri Jul 14 04:42:11 2023, max compression
```

## Comparing `reliableGPT-0.2.999.tar` & `reliableGPT-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-14 04:20:24.373581 reliableGPT-0.2.999/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.999/LICENSE
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-07-14 04:20:24.373478 reliableGPT-0.2.999/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     8826 2023-07-14 01:03:18.000000 reliableGPT-0.2.999/README.md
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      497 2023-06-28 20:45:06.000000 reliableGPT-0.2.999/pyproject.toml
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-14 04:20:24.372142 reliableGPT-0.2.999/reliableGPT.egg-info/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-07-14 04:20:24.000000 reliableGPT-0.2.999/reliableGPT.egg-info/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      361 2023-07-14 04:20:24.000000 reliableGPT-0.2.999/reliableGPT.egg-info/SOURCES.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-07-14 04:20:24.000000 reliableGPT-0.2.999/reliableGPT.egg-info/dependency_links.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       74 2023-07-14 04:20:24.000000 reliableGPT-0.2.999/reliableGPT.egg-info/requires.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-07-14 04:20:24.000000 reliableGPT-0.2.999/reliableGPT.egg-info/top_level.txt
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-14 04:20:24.373205 reliableGPT-0.2.999/reliablegpt/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     3148 2023-07-14 01:03:18.000000 reliableGPT-0.2.999/reliablegpt/Alerting.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)    23059 2023-07-14 04:20:02.000000 reliableGPT-0.2.999/reliablegpt/IndividualRequest.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1286 2023-07-02 02:49:46.000000 reliableGPT-0.2.999/reliablegpt/Model.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       58 2023-07-10 15:34:25.000000 reliableGPT-0.2.999/reliablegpt/__init__.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     5281 2023-07-14 01:20:06.000000 reliableGPT-0.2.999/reliablegpt/main.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-07-14 04:20:24.373614 reliableGPT-0.2.999/setup.cfg
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      440 2023-07-14 04:20:15.000000 reliableGPT-0.2.999/setup.py
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-14 04:42:11.311621 reliableGPT-0.3.0/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.3.0/LICENSE
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      218 2023-07-14 04:42:11.311488 reliableGPT-0.3.0/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     8826 2023-07-14 01:03:18.000000 reliableGPT-0.3.0/README.md
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      497 2023-06-28 20:45:06.000000 reliableGPT-0.3.0/pyproject.toml
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-14 04:42:11.309997 reliableGPT-0.3.0/reliableGPT.egg-info/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      218 2023-07-14 04:42:11.000000 reliableGPT-0.3.0/reliableGPT.egg-info/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      361 2023-07-14 04:42:11.000000 reliableGPT-0.3.0/reliableGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-07-14 04:42:11.000000 reliableGPT-0.3.0/reliableGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       74 2023-07-14 04:42:11.000000 reliableGPT-0.3.0/reliableGPT.egg-info/requires.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-07-14 04:42:11.000000 reliableGPT-0.3.0/reliableGPT.egg-info/top_level.txt
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-14 04:42:11.311282 reliableGPT-0.3.0/reliablegpt/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     3148 2023-07-14 01:03:18.000000 reliableGPT-0.3.0/reliablegpt/Alerting.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)    23172 2023-07-14 04:39:51.000000 reliableGPT-0.3.0/reliablegpt/IndividualRequest.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1286 2023-07-02 02:49:46.000000 reliableGPT-0.3.0/reliablegpt/Model.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       58 2023-07-10 15:34:25.000000 reliableGPT-0.3.0/reliablegpt/__init__.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     5281 2023-07-14 04:21:08.000000 reliableGPT-0.3.0/reliablegpt/main.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-07-14 04:42:11.311669 reliableGPT-0.3.0/setup.cfg
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      440 2023-07-14 04:42:03.000000 reliableGPT-0.3.0/setup.py
```

### Comparing `reliableGPT-0.2.999/LICENSE` & `reliableGPT-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.999/README.md` & `reliableGPT-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.999/reliablegpt/Alerting.py` & `reliableGPT-0.3.0/reliablegpt/Alerting.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.999/reliablegpt/IndividualRequest.py` & `reliableGPT-0.3.0/reliablegpt/IndividualRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -382,14 +382,16 @@
         new_kwargs['prompt'] = " ".join(
           [message["content"] for message in new_kwargs['messages']])
         new_kwargs.pop('messages',
                        None)  # remove messages for completion models
         return completion_model(**new_kwargs)
     except Exception as e:
       self.print_verbose(colored(f"ReliableGPT: Got 2nd AGAIN Error {e}", "red"))
+      msg = (f'error: {e} kwargs: {str(new_kwargs)}\n')
+      send_alert("[reliableGPT] Got 2nd error \n" + msg)
       raise ValueError(e)
 
   def api_key_handler(self, args, kwargs, fallback_strategy, user_email,
                       user_token):
     try:
       url = f"https://reliable-gpt-backend-9gus.zeet-berri.zeet.app/get_keys?user_email={user_email}&user_token={user_token}"
       response = requests.get(url)
```

### Comparing `reliableGPT-0.2.999/reliablegpt/Model.py` & `reliableGPT-0.3.0/reliablegpt/Model.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.999/reliablegpt/main.py` & `reliableGPT-0.3.0/reliablegpt/main.py`

 * *Files identical despite different names*

