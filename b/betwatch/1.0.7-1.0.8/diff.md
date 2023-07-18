# Comparing `tmp/betwatch-1.0.7.tar.gz` & `tmp/betwatch-1.0.8.tar.gz`

## Comparing `betwatch-1.0.7.tar` & `betwatch-1.0.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 betwatch-1.0.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 betwatch-1.0.7/Makefile
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 betwatch-1.0.7/.github/dependabot.yml
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 betwatch-1.0.7/.github/workflows/test.yml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 betwatch-1.0.7/betwatch/__about__.py
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 betwatch-1.0.7/betwatch/__init__.py
--rw-r--r--   0        0        0     8765 2020-02-02 00:00:00.000000 betwatch-1.0.7/betwatch/client.py
--rw-r--r--   0        0        0    27637 2020-02-02 00:00:00.000000 betwatch-1.0.7/betwatch/client_async.py
--rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 betwatch-1.0.7/betwatch/queries.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 betwatch-1.0.7/betwatch/types/__init__.py
--rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 betwatch-1.0.7/betwatch/types/bookmakers.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 betwatch-1.0.7/betwatch/types/exceptions.py
--rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 betwatch-1.0.7/betwatch/types/filters.py
--rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 betwatch-1.0.7/betwatch/types/markets.py
--rw-r--r--   0        0        0    12482 2020-02-02 00:00:00.000000 betwatch-1.0.7/betwatch/types/race.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 betwatch-1.0.7/betwatch/types/updates.py
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 betwatch-1.0.7/examples/get_race_prices.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 betwatch-1.0.7/examples/get_race_prices_async.py
--rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 betwatch-1.0.7/examples/get_races.py
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 betwatch-1.0.7/examples/get_races_async.py
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 betwatch-1.0.7/examples/subscriptions.py
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 betwatch-1.0.7/examples/update_rated_prices.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 betwatch-1.0.7/tests/__init__.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 betwatch-1.0.7/tests/test_check_last_updated.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 betwatch-1.0.7/tests/test_get_race.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 betwatch-1.0.7/tests/test_get_race_async.py
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 betwatch-1.0.7/tests/test_get_races.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 betwatch-1.0.7/tests/test_get_races_async.py
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 betwatch-1.0.7/.gitignore
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 betwatch-1.0.7/LICENSE.txt
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 betwatch-1.0.7/README.md
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 betwatch-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 betwatch-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 betwatch-1.0.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 betwatch-1.0.8/Makefile
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 betwatch-1.0.8/.github/dependabot.yml
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 betwatch-1.0.8/.github/workflows/test.yml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 betwatch-1.0.8/betwatch/__about__.py
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 betwatch-1.0.8/betwatch/__init__.py
+-rw-r--r--   0        0        0     8765 2020-02-02 00:00:00.000000 betwatch-1.0.8/betwatch/client.py
+-rw-r--r--   0        0        0    27637 2020-02-02 00:00:00.000000 betwatch-1.0.8/betwatch/client_async.py
+-rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 betwatch-1.0.8/betwatch/queries.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 betwatch-1.0.8/betwatch/types/__init__.py
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 betwatch-1.0.8/betwatch/types/bookmakers.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 betwatch-1.0.8/betwatch/types/exceptions.py
+-rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 betwatch-1.0.8/betwatch/types/filters.py
+-rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 betwatch-1.0.8/betwatch/types/markets.py
+-rw-r--r--   0        0        0    12482 2020-02-02 00:00:00.000000 betwatch-1.0.8/betwatch/types/race.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 betwatch-1.0.8/betwatch/types/updates.py
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 betwatch-1.0.8/examples/get_race_prices.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 betwatch-1.0.8/examples/get_race_prices_async.py
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 betwatch-1.0.8/examples/get_races.py
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 betwatch-1.0.8/examples/get_races_async.py
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 betwatch-1.0.8/examples/subscriptions.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 betwatch-1.0.8/examples/update_rated_prices.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 betwatch-1.0.8/tests/__init__.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 betwatch-1.0.8/tests/test_check_last_updated.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 betwatch-1.0.8/tests/test_get_race.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 betwatch-1.0.8/tests/test_get_race_async.py
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 betwatch-1.0.8/tests/test_get_races.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 betwatch-1.0.8/tests/test_get_races_async.py
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 betwatch-1.0.8/.gitignore
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 betwatch-1.0.8/LICENSE.txt
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 betwatch-1.0.8/README.md
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 betwatch-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 betwatch-1.0.8/PKG-INFO
```

### Comparing `betwatch-1.0.7/.github/workflows/test.yml` & `betwatch-1.0.8/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.7/betwatch/__init__.py` & `betwatch-1.0.8/betwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.7/betwatch/client.py` & `betwatch-1.0.8/betwatch/client.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.7/betwatch/client_async.py` & `betwatch-1.0.8/betwatch/client_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.7/betwatch/queries.py` & `betwatch-1.0.8/betwatch/queries.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.7/betwatch/types/bookmakers.py` & `betwatch-1.0.8/betwatch/types/bookmakers.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,14 +67,15 @@
     TRACKBET = "Trackbet"
     WOODCOCKRACING = "Woodcockracing"
     VIPBETTINGSERVICES = "Vipbettingservices"
     DAVEBET = "Davebet"
     GALLOPBET = "Gallopbet"
     RIVERBET = "Riverbet"
     BARRINGTONBOOKMAKING = "Barringtonbookmaking"
+    BUSHBET = "Bushbet"
     TOPODDS = "Topodds"
     BEAZABET = "Beazabet"
     PUNTONDOGS = "PuntOnDogs"
     PICKLEBET = "Picklebet"
     BETGALAXY = "Betgalaxy"
     DIAMONDBET = "Diamondbet"
     BITWINNING = "Bitwinning"
```

### Comparing `betwatch-1.0.7/betwatch/types/filters.py` & `betwatch-1.0.8/betwatch/types/filters.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.7/betwatch/types/markets.py` & `betwatch-1.0.8/betwatch/types/markets.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.7/betwatch/types/race.py` & `betwatch-1.0.8/betwatch/types/race.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.7/examples/get_race_prices.py` & `betwatch-1.0.8/examples/get_race_prices.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.7/examples/get_race_prices_async.py` & `betwatch-1.0.8/examples/get_race_prices_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.7/examples/get_races.py` & `betwatch-1.0.8/examples/get_races.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.7/examples/get_races_async.py` & `betwatch-1.0.8/examples/get_races_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.7/examples/subscriptions.py` & `betwatch-1.0.8/examples/subscriptions.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.7/examples/update_rated_prices.py` & `betwatch-1.0.8/examples/update_rated_prices.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.7/tests/test_get_race.py` & `betwatch-1.0.8/tests/test_get_race.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.7/tests/test_get_race_async.py` & `betwatch-1.0.8/tests/test_get_race_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.7/tests/test_get_races.py` & `betwatch-1.0.8/tests/test_get_races.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.7/tests/test_get_races_async.py` & `betwatch-1.0.8/tests/test_get_races_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.7/.gitignore` & `betwatch-1.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.7/LICENSE.txt` & `betwatch-1.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.7/README.md` & `betwatch-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.7/pyproject.toml` & `betwatch-1.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.7/PKG-INFO` & `betwatch-1.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: betwatch
-Version: 1.0.7
+Version: 1.0.8
 Summary: A Python package for interacting with the Betwatch.com API
 Project-URL: Documentation, https://github.com/betwatch/betwatch-sdk-python#readme
 Project-URL: Issues, https://github.com/betwatch/betwatch-sdk-python/issues
 Project-URL: Source, https://github.com/betwatch/betwatch-sdk-python
 Project-URL: Betwatch.com, https://betwatch.com
 Author-email: Jamie Watts <jamie@betwatch.com>
+License-Expression: MIT
 License-File: LICENSE.txt
 Keywords: api,betting,betwatch,sdk,sports
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

