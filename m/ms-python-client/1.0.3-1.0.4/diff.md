# Comparing `tmp/ms_python_client-1.0.3.tar.gz` & `tmp/ms_python_client-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_python_client-1.0.3.tar", max compression
+gzip compressed data, was "ms_python_client-1.0.4.tar", max compression
```

## Comparing `ms_python_client-1.0.3.tar` & `ms_python_client-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1100 2023-07-11 13:57:42.923031 ms_python_client-1.0.3/LICENSE
--rw-r--r--   0        0        0     5593 2023-07-11 13:57:42.923031 ms_python_client-1.0.3/README.md
--rw-r--r--   0        0        0        0 2023-07-11 13:57:42.923031 ms_python_client-1.0.3/ms_python_client/__init__.py
--rw-r--r--   0        0        0     5551 2023-07-11 13:57:42.923031 ms_python_client-1.0.3/ms_python_client/api_client.py
--rw-r--r--   0        0        0     1380 2023-07-11 13:57:42.923031 ms_python_client-1.0.3/ms_python_client/cern_ms_api_client.py
--rw-r--r--   0        0        0        0 2023-07-11 13:57:42.923031 ms_python_client-1.0.3/ms_python_client/components/__init__.py
--rw-r--r--   0        0        0        0 2023-07-11 13:57:42.923031 ms_python_client-1.0.3/ms_python_client/components/events/__init__.py
--rw-r--r--   0        0        0     4145 2023-07-11 13:57:42.923031 ms_python_client-1.0.3/ms_python_client/components/events/cern_events_component.py
--rw-r--r--   0        0        0     3100 2023-07-11 13:57:42.923031 ms_python_client-1.0.3/ms_python_client/components/events/events_component.py
--rw-r--r--   0        0        0        0 2023-07-11 13:57:42.923031 ms_python_client-1.0.3/ms_python_client/components/users/__init__.py
--rw-r--r--   0        0        0      874 2023-07-11 13:57:42.923031 ms_python_client-1.0.3/ms_python_client/components/users/users_component.py
--rw-r--r--   0        0        0     5695 2023-07-11 13:57:42.923031 ms_python_client-1.0.3/ms_python_client/ms_api_client.py
--rw-r--r--   0        0        0     1312 2023-07-11 13:57:42.923031 ms_python_client-1.0.3/ms_python_client/ms_client_interface.py
--rw-r--r--   0        0        0        0 2023-07-11 13:57:42.923031 ms_python_client-1.0.3/ms_python_client/utils/__init__.py
--rw-r--r--   0        0        0      383 2023-07-11 13:57:42.923031 ms_python_client-1.0.3/ms_python_client/utils/error.py
--rw-r--r--   0        0        0     4967 2023-07-11 13:57:42.923031 ms_python_client-1.0.3/ms_python_client/utils/event_generator.py
--rw-r--r--   0        0        0       97 2023-07-11 13:57:42.923031 ms_python_client-1.0.3/ms_python_client/utils/file_system.py
--rw-r--r--   0        0        0     1276 2023-07-11 13:57:42.923031 ms_python_client-1.0.3/ms_python_client/utils/init_from_env.py
--rw-r--r--   0        0        0      729 2023-07-11 13:57:42.923031 ms_python_client-1.0.3/ms_python_client/utils/logger.py
--rw-r--r--   0        0        0     1000 2023-07-11 13:57:42.923031 ms_python_client-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     6337 1970-01-01 00:00:00.000000 ms_python_client-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1100 2023-07-18 12:56:08.247956 ms_python_client-1.0.4/LICENSE
+-rw-r--r--   0        0        0     5624 2023-07-18 12:56:08.247956 ms_python_client-1.0.4/README.md
+-rw-r--r--   0        0        0        0 2023-07-18 12:56:08.251956 ms_python_client-1.0.4/ms_python_client/__init__.py
+-rw-r--r--   0        0        0     5551 2023-07-18 12:56:08.251956 ms_python_client-1.0.4/ms_python_client/api_client.py
+-rw-r--r--   0        0        0     1380 2023-07-18 12:56:08.251956 ms_python_client-1.0.4/ms_python_client/cern_ms_api_client.py
+-rw-r--r--   0        0        0        0 2023-07-18 12:56:08.251956 ms_python_client-1.0.4/ms_python_client/components/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 12:56:08.251956 ms_python_client-1.0.4/ms_python_client/components/events/__init__.py
+-rw-r--r--   0        0        0     4827 2023-07-18 12:56:08.251956 ms_python_client-1.0.4/ms_python_client/components/events/cern_events_component.py
+-rw-r--r--   0        0        0     3201 2023-07-18 12:56:08.251956 ms_python_client-1.0.4/ms_python_client/components/events/events_component.py
+-rw-r--r--   0        0        0        0 2023-07-18 12:56:08.251956 ms_python_client-1.0.4/ms_python_client/components/users/__init__.py
+-rw-r--r--   0        0        0      874 2023-07-18 12:56:08.251956 ms_python_client-1.0.4/ms_python_client/components/users/users_component.py
+-rw-r--r--   0        0        0     5695 2023-07-18 12:56:08.251956 ms_python_client-1.0.4/ms_python_client/ms_api_client.py
+-rw-r--r--   0        0        0     1312 2023-07-18 12:56:08.251956 ms_python_client-1.0.4/ms_python_client/ms_client_interface.py
+-rw-r--r--   0        0        0        0 2023-07-18 12:56:08.251956 ms_python_client-1.0.4/ms_python_client/utils/__init__.py
+-rw-r--r--   0        0        0      383 2023-07-18 12:56:08.251956 ms_python_client-1.0.4/ms_python_client/utils/error.py
+-rw-r--r--   0        0        0     4967 2023-07-18 12:56:08.251956 ms_python_client-1.0.4/ms_python_client/utils/event_generator.py
+-rw-r--r--   0        0        0       97 2023-07-18 12:56:08.251956 ms_python_client-1.0.4/ms_python_client/utils/file_system.py
+-rw-r--r--   0        0        0     1276 2023-07-18 12:56:08.251956 ms_python_client-1.0.4/ms_python_client/utils/init_from_env.py
+-rw-r--r--   0        0        0      729 2023-07-18 12:56:08.251956 ms_python_client-1.0.4/ms_python_client/utils/logger.py
+-rw-r--r--   0        0        0     1010 2023-07-18 12:56:08.251956 ms_python_client-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     6368 1970-01-01 00:00:00.000000 ms_python_client-1.0.4/PKG-INFO
```

### Comparing `ms_python_client-1.0.3/LICENSE` & `ms_python_client-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_python_client-1.0.3/README.md` & `ms_python_client-1.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -136,14 +136,15 @@
 #### **events**:
 
 1. get all events
 2. get a single event using zoom id
 3. create an event
 4. update an event using zoom id
 5. delete an event using zoom id
+6. get the zoom id of an event
 
 You will find useful the `EventParameters` and `PartialEventParameters` classes, which will help you to create the events.
 
 - `ZOOM_ID` is the id of the zoom meeting, which can be found inside the url of a meeting link. This is **mandatory** to create an event.
 - `USER_ID` is the email of the Zoom Room.
 
 ```python
```

### Comparing `ms_python_client-1.0.3/ms_python_client/api_client.py` & `ms_python_client-1.0.4/ms_python_client/api_client.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-1.0.3/ms_python_client/cern_ms_api_client.py` & `ms_python_client-1.0.4/ms_python_client/cern_ms_api_client.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-1.0.3/ms_python_client/components/events/cern_events_component.py` & `ms_python_client-1.0.4/ms_python_client/components/events/cern_events_component.py`

 * *Files 11% similar despite different names*

```diff
@@ -77,14 +77,38 @@
                 "Found %s events with zoom id %s. Returning the first one.",
                 count,
                 zoom_id,
             )
 
         return response.get("value", [])[0]
 
+    def get_event_zoom_id(
+        self,
+        user_id: str,
+        event_id: str,
+        extra_headers: Optional[Mapping[str, str]] = None,
+    ) -> str:
+        """Get the zoom id of an event of a user
+
+        Args:
+            event_id (str): The event id
+
+        Returns:
+            str: The zoom id of the event
+        """
+        parameters = {
+            "$expand": f"singleValueExtendedProperties($filter=id eq \
+                '{ZOOM_ID_EXTENDED_PROPERTY_ID}')",
+        }
+        response = self.events_component.get_event(
+            user_id, event_id, parameters, extra_headers
+        )
+
+        return response["singleValueExtendedProperties"][0]["value"]
+
     def create_event(
         self,
         user_id: str,
         event: EventParameters,
         extra_headers: Optional[Mapping[str, str]] = None,
     ) -> dict:
         """Create an event for a user
```

### Comparing `ms_python_client-1.0.3/ms_python_client/components/events/events_component.py` & `ms_python_client-1.0.4/ms_python_client/components/events/events_component.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,27 +27,30 @@
         )
         return response.json()
 
     def get_event(
         self,
         user_id: str,
         event_id: str,
+        parameters: Optional[Mapping[str, str]] = None,
         extra_headers: Optional[Mapping[str, str]] = None,
     ) -> dict:
         """Get an event of a user
 
         Args:
             user_id (str): The user id
             event_id (str): The event id
 
         Returns:
             dict: The response of the request
         """
         api_path = f"/users/{user_id}/calendar/events/{event_id}"
-        response = self.client.make_get_request(api_path, extra_headers=extra_headers)
+        response = self.client.make_get_request(
+            api_path, parameters=parameters, extra_headers=extra_headers
+        )
         return response.json()
 
     def create_event(
         self,
         user_id: str,
         json: Mapping[str, Any],
         extra_headers: Optional[Mapping[str, str]] = None,
```

### Comparing `ms_python_client-1.0.3/ms_python_client/components/users/users_component.py` & `ms_python_client-1.0.4/ms_python_client/components/users/users_component.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-1.0.3/ms_python_client/ms_api_client.py` & `ms_python_client-1.0.4/ms_python_client/ms_api_client.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-1.0.3/ms_python_client/ms_client_interface.py` & `ms_python_client-1.0.4/ms_python_client/ms_client_interface.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-1.0.3/ms_python_client/utils/event_generator.py` & `ms_python_client-1.0.4/ms_python_client/utils/event_generator.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-1.0.3/ms_python_client/utils/init_from_env.py` & `ms_python_client-1.0.4/ms_python_client/utils/init_from_env.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-1.0.3/ms_python_client/utils/logger.py` & `ms_python_client-1.0.4/ms_python_client/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-1.0.3/pyproject.toml` & `ms_python_client-1.0.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [tool.poetry]
 name = "ms-python-client"
-version = "1.0.3"
+version = "1.0.4"
 exclude = ["tests*", "example*", ".github*", ".git*", ".vscode*"]
 description = "This package is used to interact with the microsoft graph API"
 authors = ["Samuel Guillemet <samuel.guillemet@telecom-sudparis.eu>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "ms_python_client"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 python-dotenv = "^1.0.0"
 msal = "^1.22.0"
 requests = "^2.31.0"
 
 [tool.poetry.group.dev.dependencies]
-black = "23.7.0"
-flake8 = "6.0.0"
-isort = "5.12.0"
-pre-commit = "3.3.3"
-mypy = "1.4.1"
-mypy-extensions = "1.0.0"
-pylint = "2.17.4"
-pytest = "7.4.0"
-pytest-cov = "4.1.0"
-responses = "0.23.1"
+black = "^23.7.0"
+flake8 = "^6.0.0"
+isort = "^5.12.0"
+pre-commit = "^3.3.3"
+mypy = "^1.4.1"
+mypy-extensions = "^1.0.0"
+pylint = "^2.17.4"
+pytest = "^7.4.0"
+pytest-cov = "^4.1.0"
+responses = "^0.23.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/cern-vc/ms-python-client/issues"
```

### Comparing `ms_python_client-1.0.3/PKG-INFO` & `ms_python_client-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-python-client
-Version: 1.0.3
+Version: 1.0.4
 Summary: This package is used to interact with the microsoft graph API
 License: MIT
 Author: Samuel Guillemet
 Author-email: samuel.guillemet@telecom-sudparis.eu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -155,14 +155,15 @@
 #### **events**:
 
 1. get all events
 2. get a single event using zoom id
 3. create an event
 4. update an event using zoom id
 5. delete an event using zoom id
+6. get the zoom id of an event
 
 You will find useful the `EventParameters` and `PartialEventParameters` classes, which will help you to create the events.
 
 - `ZOOM_ID` is the id of the zoom meeting, which can be found inside the url of a meeting link. This is **mandatory** to create an event.
 - `USER_ID` is the email of the Zoom Room.
 
 ```python
```

