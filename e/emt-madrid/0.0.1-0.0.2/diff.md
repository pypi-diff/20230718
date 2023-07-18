# Comparing `tmp/emt_madrid-0.0.1.tar.gz` & `tmp/emt_madrid-0.0.2.tar.gz`

## Comparing `emt_madrid-0.0.1.tar` & `emt_madrid-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,31 @@
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 emt_madrid-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 emt_madrid-0.0.1/requirements.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 emt_madrid-0.0.1/.github/dependabot.yml
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 emt_madrid-0.0.1/.github/workflows/tests.yml
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 emt_madrid-0.0.1/emt_madrid/__init__.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 emt_madrid-0.0.1/emt_madrid/const.py
--rw-r--r--   0        0        0     8748 2020-02-02 00:00:00.000000 emt_madrid-0.0.1/emt_madrid/emt_api.py
--rw-r--r--   0        0        0     4469 2020-02-02 00:00:00.000000 emt_madrid-0.0.1/emt_madrid/parser.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 emt_madrid-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 emt_madrid-0.0.1/tests/conftest.py
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 emt_madrid-0.0.1/tests/test_concurrency.py
--rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 emt_madrid-0.0.1/tests/test_emt_api.py
--rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 emt_madrid-0.0.1/tests/test_parser.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 emt_madrid-0.0.1/tests/response_examples/API_LIMIT.json
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 emt_madrid-0.0.1/tests/response_examples/LOGIN_INVALID_PASSWORD.json
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 emt_madrid-0.0.1/tests/response_examples/LOGIN_INVALID_USER.json
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 emt_madrid-0.0.1/tests/response_examples/LOGIN_OK.json
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 emt_madrid-0.0.1/tests/response_examples/STOP_ARRIVAL_INVALID_STOP.json
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 emt_madrid-0.0.1/tests/response_examples/STOP_ARRIVAL_INVALID_TOKEN.json
--rw-r--r--   0        0        0     6520 2020-02-02 00:00:00.000000 emt_madrid-0.0.1/tests/response_examples/STOP_ARRIVAL_OK.json
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 emt_madrid-0.0.1/tests/response_examples/STOP_DETAIL_INVALID_STOP.json
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 emt_madrid-0.0.1/tests/response_examples/STOP_DETAIL_INVALID_TOKEN.json
--rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 emt_madrid-0.0.1/tests/response_examples/STOP_DETAIL_OK.json
--rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 emt_madrid-0.0.1/tests/response_examples/STOP_INFO.json
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 emt_madrid-0.0.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 emt_madrid-0.0.1/LICENSE
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 emt_madrid-0.0.1/README.md
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 emt_madrid-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 emt_madrid-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 emt_madrid-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 emt_madrid-0.0.2/requirements.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 emt_madrid-0.0.2/.github/dependabot.yml
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 emt_madrid-0.0.2/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 emt_madrid-0.0.2/emt_madrid/__init__.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 emt_madrid-0.0.2/emt_madrid/const.py
+-rw-r--r--   0        0        0     9715 2020-02-02 00:00:00.000000 emt_madrid-0.0.2/emt_madrid/emt_api.py
+-rw-r--r--   0        0        0     5785 2020-02-02 00:00:00.000000 emt_madrid-0.0.2/emt_madrid/parser.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 emt_madrid-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     6138 2020-02-02 00:00:00.000000 emt_madrid-0.0.2/tests/conftest.py
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 emt_madrid-0.0.2/tests/test_concurrency.py
+-rw-r--r--   0        0        0     6372 2020-02-02 00:00:00.000000 emt_madrid-0.0.2/tests/test_emt_api.py
+-rw-r--r--   0        0        0     5248 2020-02-02 00:00:00.000000 emt_madrid-0.0.2/tests/test_parser.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 emt_madrid-0.0.2/tests/response_examples/API_LIMIT.json
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 emt_madrid-0.0.2/tests/response_examples/LOGIN_INVALID_PASSWORD.json
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 emt_madrid-0.0.2/tests/response_examples/LOGIN_INVALID_USER.json
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 emt_madrid-0.0.2/tests/response_examples/LOGIN_OK.json
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 emt_madrid-0.0.2/tests/response_examples/STOPS_AROUND_STOP_OK.json
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 emt_madrid-0.0.2/tests/response_examples/STOP_ARRIVAL_INVALID_STOP.json
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 emt_madrid-0.0.2/tests/response_examples/STOP_ARRIVAL_INVALID_TOKEN.json
+-rw-r--r--   0        0        0     6520 2020-02-02 00:00:00.000000 emt_madrid-0.0.2/tests/response_examples/STOP_ARRIVAL_OK.json
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 emt_madrid-0.0.2/tests/response_examples/STOP_DETAIL_INVALID_STOP.json
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 emt_madrid-0.0.2/tests/response_examples/STOP_DETAIL_INVALID_TOKEN.json
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 emt_madrid-0.0.2/tests/response_examples/STOP_DETAIL_NOT_FOUND.json
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 emt_madrid-0.0.2/tests/response_examples/STOP_DETAIL_OK.json
+-rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 emt_madrid-0.0.2/tests/response_examples/STOP_INFO.json
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 emt_madrid-0.0.2/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 emt_madrid-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 emt_madrid-0.0.2/README.md
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 emt_madrid-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 emt_madrid-0.0.2/PKG-INFO
```

### Comparing `emt_madrid-0.0.1/.pre-commit-config.yaml` & `emt_madrid-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `emt_madrid-0.0.1/.github/workflows/tests.yml` & `emt_madrid-0.0.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `emt_madrid-0.0.1/emt_madrid/emt_api.py` & `emt_madrid-0.0.2/emt_madrid/emt_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -177,33 +177,58 @@
         self._token = token
 
     @property
     def token(self) -> str:
         """Return API token."""
         return self._token
 
+    async def _update_stop_info_around_stop(self) -> Optional[Dict[str, Any]]:
+        """Update information about a bus stop using the stops around stop endpoint."""
+        endpoint = f"v2/transport/busemtmad/stops/arroundstop/{self._stop_id}/0/"
+        headers = {"accessToken": self._token}
+        url = self._base_url + endpoint
+
+        try:
+            async with async_timeout.timeout(DEFAULT_TIMEOUT):
+                response = await self._get_data(url, headers, "GET")
+
+            if response is None:
+                return None
+
+            parsed_stop_info = parse_stop_info(response, self._stop_info)
+
+            return parsed_stop_info
+
+        except asyncio.TimeoutError:
+            _LOGGER.warning("Timeout error fetching data from %s", url)
+            return None
+
     async def update_stop_info(self) -> None:
         """Update information about a bus stop."""
         endpoint = f"v1/transport/busemtmad/stops/{self._stop_id}/detail/"
         headers = {"accessToken": self._token}
         url = self._base_url + endpoint
 
         try:
             async with async_timeout.timeout(DEFAULT_TIMEOUT):
                 response = await self._get_data(url, headers, "GET")
 
             if response is None:
                 return None
+            print(response)
 
-            parsed_stop_info = parse_stop_info(response, self._stop_info)
+            if response.get("code", {}) == "81":
+                parsed_stop_info = await self._update_stop_info_around_stop()
+            else:
+                parsed_stop_info = parse_stop_info(response, self._stop_info)
 
             if parsed_stop_info is None:
                 return None
 
-            if parsed_stop_info.get("error") == "Invalid token":
+            if parsed_stop_info.get("error", None) is not None:
                 return None
 
             async with self._update_semaphore:
                 self._stop_info = parsed_stop_info
 
         except asyncio.TimeoutError:
             _LOGGER.warning("Timeout error fetching data from %s", url)
```

### Comparing `emt_madrid-0.0.1/emt_madrid/parser.py` & `emt_madrid-0.0.2/emt_madrid/parser.py`

 * *Files 25% similar despite different names*

```diff
@@ -38,64 +38,91 @@
 def parse_stop_info(
     response: Dict[str, Any], stop_info: Dict[str, Any]
 ) -> Optional[Dict[str, Any]]:
     """Parse the stop info from the API response."""
     assert stop_info is not None
     try:
         response_code = response.get("code")
-        if response_code in ("90", "81"):
+        if response_code == "90":
             raise BusStopDisabled
         if response_code == "80":
             raise InvalidToken
         if response_code == "98":
             raise APILimitReached
 
-        response_stop = response["data"][0]["stops"][0]
-        stop_info.update(
-            {
-                "stop_id": response_stop["stop"],
-                "stop_name": response_stop["name"],
-                "stop_coordinates": response_stop["geometry"]["coordinates"],
-                "stop_address": response_stop["postalAddress"],
-                "lines": parse_lines(response_stop["dataLine"]),
-            }
-        )
+        if "stopName" in response["data"][0]:
+            response_stop = response["data"][0]
+            stop_info.update(
+                {
+                    "stop_id": str(response_stop["stopId"]),
+                    "stop_name": response_stop["stopName"].rstrip(),
+                    "stop_coordinates": response_stop["geometry"]["coordinates"],
+                    "stop_address": response_stop["address"].rstrip(),
+                    "lines": parse_lines(response_stop["lines"], "basic"),
+                }
+            )
+
+        else:
+            response_stop = response["data"][0]["stops"][0]
+            stop_info.update(
+                {
+                    "stop_id": response_stop["stop"],
+                    "stop_name": response_stop["name"].rstrip(),
+                    "stop_coordinates": response_stop["geometry"]["coordinates"],
+                    "stop_address": response_stop["postalAddress"].rstrip(),
+                    "lines": parse_lines(response_stop["dataLine"], "full"),
+                }
+            )
         return stop_info
 
     except BusStopDisabled:
         _LOGGER.warning("Bus Stop disabled or does not exist")
-        return None
+        return {"error": "Bus Stop disabled", "error_code": response.get("code")}
     except InvalidToken:
         _LOGGER.warning("Invalid or expired token")
-        return {"error": "Invalid token"}
+        return {"error": "Invalid token", "error_code": response.get("code")}
     except APILimitReached:
         _LOGGER.warning("Maximum daily API usage has been exceeded.")
-        return None
+        return {
+            "error": "Maximum daily API usage reached",
+            "error_code": response.get("code"),
+        }
 
 
-def parse_lines(lines: List[Dict[str, Any]]) -> Dict[str, Any]:
+def parse_lines(lines: List[Dict[str, Any]], mode: str) -> Dict[str, Any]:
     """Parse the line info from the API response."""
     line_info: Dict[str, Any] = {}
-    for line in lines:
-        line_number = str(line.get("label"))
-        line_info[line_number] = {
-            "destination": line.get("headerA")
-            if line.get("direction") == "A"
-            else line.get("headerB"),
-            "origin": line.get("headerA")
-            if line.get("direction") == "B"
-            else line.get("headerB"),
-            "max_freq": int(line.get("maxFreq") or 0),
-            "min_freq": int(line.get("minFreq") or 0),
-            "start_time": line.get("startTime"),
-            "end_time": line.get("stopTime"),
-            "day_type": line.get("dayType"),
-            "distance": [],
-            "arrivals": [],
-        }
+    if mode == "full":
+        for line in lines:
+            line_number = str(line.get("label"))
+            line_info[line_number] = {
+                "destination": line.get("headerA")
+                if line.get("direction") == "A"
+                else line.get("headerB"),
+                "origin": line.get("headerA")
+                if line.get("direction") == "B"
+                else line.get("headerB"),
+                "max_freq": int(line.get("maxFreq") or 0),
+                "min_freq": int(line.get("minFreq") or 0),
+                "start_time": line.get("startTime"),
+                "end_time": line.get("stopTime"),
+                "day_type": line.get("dayType"),
+                "distance": [],
+                "arrivals": [],
+            }
+    elif mode == "basic":
+        line_info = {}
+        for line in lines:
+            line_number = line["label"]
+            line_info[line_number] = {
+                "destination": line["nameA"] if line["to"] == "A" else line["nameB"],
+                "origin": line["nameA"] if line["to"] == "B" else line["nameB"],
+                "distance": [],
+                "arrivals": [],
+            }
     return line_info
 
 
 def parse_arrivals(
     response: Dict[str, Any], stop_info: Dict[str, Any]
 ) -> Optional[Dict[str, Any]]:
     """Parse the arrival times and distance from the API response."""
```

### Comparing `emt_madrid-0.0.1/tests/conftest.py` & `emt_madrid-0.0.2/tests/conftest.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 """EMT Madrid API tests configuration."""
 
 import json
 import pathlib
 from typing import Any, Dict, Optional
 
 TEST_EXAMPLES_PATH = pathlib.Path(__file__).parent / "response_examples"
+_FIXTURE_STOP_INFO = "STOP_INFO.json"
 
 _FIXTURE_LOGIN_OK = "LOGIN_OK.json"
 _FIXTURE_LOGIN_INVALID_USER = "LOGIN_INVALID_USER.json"
 _FIXTURE_LOGIN_INVALID_PASSWORD = "LOGIN_INVALID_PASSWORD.json"
 _FIXTURE_STOP_DETAIL_OK = "STOP_DETAIL_OK.json"
 _FIXTURE_STOP_DETAIL_INVALID_STOP = "STOP_DETAIL_INVALID_STOP.json"
 _FIXTURE_STOP_DETAIL_INVALID_TOKEN = "STOP_DETAIL_INVALID_TOKEN.json"
 _FIXTURE_STOP_ARRIVAL_OK = "STOP_ARRIVAL_OK.json"
 _FIXTURE_STOP_ARRIVAL_INVALID_STOP = "STOP_ARRIVAL_INVALID_STOP.json"
+_FIXTURE_STOP_DETAIL_NOT_FOUND = "STOP_DETAIL_NOT_FOUND.json"
 _FIXTURE_STOP_ARRIVAL_INVALID_TOKEN = "STOP_ARRIVAL_INVALID_TOKEN.json"
 _FIXTURE_API_LIMIT = "API_LIMIT.json"
-_FIXTURE_STOP_INFO = "STOP_INFO.json"
+_FIXTURE_STOPS_AROUND_STOP_OK = "STOPS_AROUND_STOP_OK.json"
 
 
 class MockAsyncSession:
     """Mock GET requests to esios API."""
 
     status: int = 200
     _counter: int = 0
@@ -47,41 +49,57 @@
     async def json(self, *_args, **_kwargs):
         """Dumb response."""
         return self._raw_response
 
     async def get(self, url: str, headers: Dict[str, Any], *_args, **_kwargs):
         """Dumb get method."""
         self._counter += 1
-        if self.exc:
+        if self.exc and not ("detail" in url and "stop_not_found" in url):
             raise self.exc
+
         if "user/login/" in url:
-            if headers["email"] == "invalid_email":
-                self._raw_response = load_fixture(_FIXTURE_LOGIN_INVALID_USER)
-            elif headers["password"] == "invalid_password":
-                self._raw_response = load_fixture(_FIXTURE_LOGIN_INVALID_PASSWORD)
-            elif headers["password"] == "api_limit":
-                self._raw_response = load_fixture(_FIXTURE_API_LIMIT)
-            else:
-                self._raw_response = load_fixture(_FIXTURE_LOGIN_OK)
+            self._raw_response = self._handle_login_request(headers)
+        elif "detail" in url:
+            self._raw_response = self._handle_detail_request(url, headers)
+        elif "arroundstop" in url:
+            self._raw_response = self._handle_arroundstop_request(headers)
 
-        elif "stops" in url and "detail" in url:
-            stop_id = url.split("/")[-3]
-            if (
-                headers["accessToken"] == "invalid_token"
-                or headers["accessToken"] is None
-            ):
-                self._raw_response = load_fixture(_FIXTURE_STOP_DETAIL_INVALID_TOKEN)
-            elif headers["accessToken"] == "api_limit":
-                self._raw_response = load_fixture(_FIXTURE_API_LIMIT)
-            elif stop_id in ("invalid_stop_id", "None"):
-                self._raw_response = load_fixture(_FIXTURE_STOP_DETAIL_INVALID_STOP)
-            else:
-                self._raw_response = load_fixture(_FIXTURE_STOP_DETAIL_OK)
         return self
 
+    def _handle_login_request(self, headers: Dict[str, Any]):
+        """Handle the login request based on the provided headers."""
+        if headers["email"] == "invalid_email":
+            return load_fixture(_FIXTURE_LOGIN_INVALID_USER)
+        if headers["password"] == "invalid_password":
+            return load_fixture(_FIXTURE_LOGIN_INVALID_PASSWORD)
+        if headers["password"] == "api_limit":
+            return load_fixture(_FIXTURE_API_LIMIT)
+
+        return load_fixture(_FIXTURE_LOGIN_OK)
+
+    def _handle_detail_request(self, url: str, headers: Dict[str, Any]):
+        """Handle the detail request based on the provided URL and headers."""
+        stop_id = url.split("/")[-3]
+        if headers["accessToken"] == "invalid_token" or headers["accessToken"] is None:
+            return load_fixture(_FIXTURE_STOP_DETAIL_INVALID_TOKEN)
+        if headers["accessToken"] == "api_limit" and stop_id != "stop_not_found":
+            return load_fixture(_FIXTURE_API_LIMIT)
+        if stop_id in ("invalid_stop_id", "None"):
+            return load_fixture(_FIXTURE_STOP_DETAIL_INVALID_STOP)
+        if stop_id in ("stop_not_found"):
+            return load_fixture(_FIXTURE_STOP_DETAIL_NOT_FOUND)
+
+        return load_fixture(_FIXTURE_STOP_DETAIL_OK)
+
+    def _handle_arroundstop_request(self, headers: Dict[str, Any]):
+        """Handle the 'arroundstop' request."""
+        if headers["accessToken"] == "api_limit":
+            return load_fixture(_FIXTURE_API_LIMIT)
+        return load_fixture(_FIXTURE_STOPS_AROUND_STOP_OK)
+
     async def post(self, url: str, headers: Dict[str, Any], *_args, **_kwargs):
         """Dumb post method."""
         self._counter += 1
         if self.exc:
             raise self.exc
         if "stops" in url and "arrives" in url:
             if headers["accessToken"] == "invalid_token":
@@ -102,21 +120,36 @@
 
 
 def load_fixture(filename: str):
     """Load stored example for EMT API response."""
     return json.loads((TEST_EXAMPLES_PATH / filename).read_text())
 
 
-def check_stop_info(stop_info, distance=0, arrivals=0):
+def check_stop_info(stop_info, distance=0, arrivals=0, code="00"):
     """Verify that the stop_info is correct."""
-    lines = stop_info.get("lines")
-    assert len(lines) == 12
-    line = lines.get("27")
-    assert line.get("destination") == "PLAZA CASTILLA"
-    assert line.get("origin") == "EMBAJADORES"
-    assert line.get("max_freq") == 11
-    assert line.get("min_freq") == 3
-    assert line.get("start_time") == "05:35"
-    assert line.get("end_time") == "00:01"
-    assert line.get("day_type") == "LA"
-    assert len(line.get("distance")) == distance
-    assert len(line.get("arrivals")) == arrivals
+    if code == "00":
+        lines = stop_info.get("lines")
+        assert len(lines) == 12
+        line = lines.get("27")
+        assert line.get("destination") == "PLAZA CASTILLA"
+        assert line.get("origin") == "EMBAJADORES"
+        assert line.get("max_freq") == 11
+        assert line.get("min_freq") == 3
+        assert line.get("start_time") == "05:35"
+        assert line.get("end_time") == "00:01"
+        assert line.get("day_type") == "LA"
+        assert len(line.get("distance")) == distance
+        assert len(line.get("arrivals")) == arrivals
+
+    if code == "81":
+        lines = stop_info.get("lines")
+        assert len(lines) == 2
+        line = lines.get("172")
+        assert line.get("destination") == "LAS TABLAS"
+        assert line.get("origin") == "TELEFONICA"
+        assert line.get("max_freq") is None
+        assert line.get("min_freq") is None
+        assert line.get("start_time") is None
+        assert line.get("end_time") is None
+        assert line.get("day_type") is None
+        assert len(line.get("distance")) == distance
+        assert len(line.get("arrivals")) == arrivals
```

### Comparing `emt_madrid-0.0.1/tests/test_concurrency.py` & `emt_madrid-0.0.2/tests/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `emt_madrid-0.0.1/tests/test_emt_api.py` & `emt_madrid-0.0.2/tests/test_emt_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -58,14 +58,37 @@
         emt_api = EMTAPIBusStop(session=mock_session, token=token, stop_id="72")
         await emt_api.update_stop_info()
         assert len(caplog.messages) == num_log_msgs
         assert mock_session.call_count == call_count
 
 
 @pytest.mark.parametrize(
+    "token, stop_id, status, exception, num_log_msgs, call_count",
+    (
+        ("token", "stop_not_found", 200, None, 0, 2),
+        ("api_limit", "stop_not_found", 200, None, 1, 2),
+        ("token", "stop_not_found", 200, asyncio.TimeoutError, 1, 2),
+        ("token", "stop_not_found", 200, TimeoutError, 1, 2),
+        ("token", "stop_not_found", 200, ClientError, 1, 2),
+    ),
+)
+@pytest.mark.asyncio
+async def test_update_stop_info_alternative_method(
+    token, stop_id, status, exception, num_log_msgs, call_count, caplog
+):  # pylint: disable=too-many-arguments
+    """Test update_stop_info method."""
+    mock_session = MockAsyncSession(status=status, exc=exception)
+    with caplog.at_level(logging.WARNING):
+        emt_api = EMTAPIBusStop(session=mock_session, token=token, stop_id=stop_id)
+        await emt_api.update_stop_info()
+        assert len(caplog.messages) == num_log_msgs
+        assert mock_session.call_count == call_count
+
+
+@pytest.mark.parametrize(
     "token, stop_info, status, exception, num_log_msgs, call_count",
     (
         ("token", {}, 200, None, 0, 2),
         ("token", PRE_LOADED_STOP_INFO, 200, None, 0, 1),
         ("api_limit", {}, 200, None, 1, 2),
         ("api_limit", PRE_LOADED_STOP_INFO, 200, None, 1, 1),
         ("invalid_token", PRE_LOADED_STOP_INFO, 200, None, 1, 1),
```

### Comparing `emt_madrid-0.0.1/tests/test_parser.py` & `emt_madrid-0.0.2/tests/test_parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -75,14 +75,44 @@
             )
             assert len(stop_info.get("stop_coordinates")) == 2
 
             check_stop_info(stop_info)
 
 
 @pytest.mark.parametrize(
+    "token, stop_id, num_log_msgs",
+    (
+        ("token", "stop_not_found", 0),
+        ("api_limit", "stop_not_found", 1),
+    ),
+)
+@pytest.mark.asyncio
+async def test_parse_stop_alternative__method(token, stop_id, num_log_msgs, caplog):
+    """Test parse_stop and parse_lines functions when using the alternative method."""
+    mock_session = MockAsyncSession()
+    with caplog.at_level(logging.WARNING):
+        emt_api_bus_stop = EMTAPIBusStop(
+            session=mock_session, token=token, stop_id=stop_id
+        )
+        await emt_api_bus_stop.update_stop_info()
+        stop_info = emt_api_bus_stop.get_stop_info()
+        assert len(caplog.messages) == num_log_msgs
+        if token == "token" and stop_id == "stop_not_found":
+            assert stop_info is not None
+            assert stop_info.get("stop_id") == "4490"
+            assert stop_info.get("stop_name") == "Camino de Santiago-Valcarlos"
+            assert (
+                stop_info.get("stop_address") == "Valcarlos con Av. Camino de Santiago"
+            )
+            assert len(stop_info.get("stop_coordinates")) == 2
+
+            check_stop_info(stop_info, code="81")
+
+
+@pytest.mark.parametrize(
     "token, stop_id, stop_info, num_log_msgs",
     (
         ("token", "72", {}, 0),
         ("token", "72", PRE_LOADED_STOP_INFO, 0),
         ("api_limit", "72", {}, 1),
         ("api_limit", "72", PRE_LOADED_STOP_INFO, 1),
         ("token", "invalid_stop_id", PRE_LOADED_STOP_INFO, 1),
```

### Comparing `emt_madrid-0.0.1/tests/response_examples/LOGIN_OK.json` & `emt_madrid-0.0.2/tests/response_examples/LOGIN_OK.json`

 * *Files identical despite different names*

### Comparing `emt_madrid-0.0.1/tests/response_examples/STOP_ARRIVAL_OK.json` & `emt_madrid-0.0.2/tests/response_examples/STOP_ARRIVAL_OK.json`

 * *Files identical despite different names*

### Comparing `emt_madrid-0.0.1/tests/response_examples/STOP_DETAIL_OK.json` & `emt_madrid-0.0.2/tests/response_examples/STOP_DETAIL_OK.json`

 * *Files identical despite different names*

### Comparing `emt_madrid-0.0.1/tests/response_examples/STOP_INFO.json` & `emt_madrid-0.0.2/tests/response_examples/STOP_INFO.json`

 * *Files identical despite different names*

### Comparing `emt_madrid-0.0.1/.gitignore` & `emt_madrid-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `emt_madrid-0.0.1/LICENSE` & `emt_madrid-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `emt_madrid-0.0.1/README.md` & `emt_madrid-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `emt_madrid-0.0.1/pyproject.toml` & `emt_madrid-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "emt_madrid"
-version = "0.0.1"
+version = "0.0.2"
 description = "Python wrapper for the Madrid EMT (Empresa Municipal de Transportes) API"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
     "aiohttp >= 3.8.4",
     "async-timeout >= 4.0.2"
 ]
```

### Comparing `emt_madrid-0.0.1/PKG-INFO` & `emt_madrid-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emt_madrid
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python wrapper for the Madrid EMT (Empresa Municipal de Transportes) API
 Project-URL: Homepage, https://github.com/fermartv/EMTMadrid
 Project-URL: Bug Tracker, https://github.com/fermartv/EMTMadrid/issues
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

