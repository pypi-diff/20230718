# Comparing `tmp/autocensus-2.1.1.tar.gz` & `tmp/autocensus-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autocensus-2.1.1.tar", max compression
+gzip compressed data, was "autocensus-2.1.2.tar", max compression
```

## Comparing `autocensus-2.1.1.tar` & `autocensus-2.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1068 2021-09-22 22:54:10.226921 autocensus-2.1.1/LICENSE
--rw-r--r--   0        0        0      529 2023-01-19 19:59:43.875349 autocensus-2.1.1/autocensus/__init__.py
--rw-r--r--   0        0        0     9145 2023-01-19 19:59:43.876128 autocensus-2.1.1/autocensus/api.py
--rw-r--r--   0        0        0      816 2022-10-26 20:35:26.719424 autocensus-2.1.1/autocensus/constants.py
--rw-r--r--   0        0        0      612 2021-09-22 22:54:10.228116 autocensus-2.1.1/autocensus/errors.py
--rw-r--r--   0        0        0     6227 2023-01-19 19:59:43.876840 autocensus-2.1.1/autocensus/geography.py
--rw-r--r--   0        0        0    19446 2023-01-19 19:59:43.877574 autocensus-2.1.1/autocensus/query.py
--rw-r--r--   0        0        0      891 2021-09-22 22:54:10.229244 autocensus-2.1.1/autocensus/resources/annotations.csv
--rw-r--r--   0        0        0     1675 2022-02-17 21:20:37.407429 autocensus-2.1.1/autocensus/resources/columns.csv
--rw-r--r--   0        0        0      396 2022-02-17 21:20:37.407669 autocensus-2.1.1/autocensus/resources/gazetteer_codes.csv
--rw-r--r--   0        0        0      729 2022-10-26 20:35:26.722906 autocensus-2.1.1/autocensus/resources/geo_codes.csv
--rw-r--r--   0        0        0      514 2022-02-17 21:20:37.407934 autocensus-2.1.1/autocensus/resources/geo_ids.csv
--rw-r--r--   0        0        0      182 2022-02-17 21:20:37.408243 autocensus-2.1.1/autocensus/resources/names.csv
--rw-r--r--   0        0        0     7840 2023-01-19 19:59:43.878208 autocensus-2.1.1/autocensus/socrata.py
--rw-r--r--   0        0        0     4674 2023-01-19 19:59:43.878938 autocensus-2.1.1/autocensus/utilities.py
--rw-r--r--   0        0        0     1419 2023-01-19 19:59:43.881475 autocensus-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     9230 2023-01-19 19:59:43.882239 autocensus-2.1.1/readme.md
--rw-r--r--   0        0        0    10517 1970-01-01 00:00:00.000000 autocensus-2.1.1/setup.py
--rw-r--r--   0        0        0    10484 1970-01-01 00:00:00.000000 autocensus-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-05-26 17:48:20.875192 autocensus-2.1.2/LICENSE
+-rw-r--r--   0        0        0      529 2023-05-26 17:13:48.315169 autocensus-2.1.2/autocensus/__init__.py
+-rw-r--r--   0        0        0     9145 2023-05-26 17:40:01.903953 autocensus-2.1.2/autocensus/api.py
+-rw-r--r--   0        0        0      805 2023-05-26 17:48:20.877001 autocensus-2.1.2/autocensus/constants.py
+-rw-r--r--   0        0        0      612 2021-09-22 22:54:10.228116 autocensus-2.1.2/autocensus/errors.py
+-rw-r--r--   0        0        0     6227 2023-04-12 21:16:03.490748 autocensus-2.1.2/autocensus/geography.py
+-rw-r--r--   0        0        0    19446 2023-04-12 21:11:50.620541 autocensus-2.1.2/autocensus/query.py
+-rw-r--r--   0        0        0      891 2021-09-22 22:54:10.229244 autocensus-2.1.2/autocensus/resources/annotations.csv
+-rw-r--r--   0        0        0     1675 2022-02-17 21:20:37.407429 autocensus-2.1.2/autocensus/resources/columns.csv
+-rw-r--r--   0        0        0      396 2022-02-17 21:20:37.407669 autocensus-2.1.2/autocensus/resources/gazetteer_codes.csv
+-rw-r--r--   0        0        0      729 2022-10-26 20:35:26.722906 autocensus-2.1.2/autocensus/resources/geo_codes.csv
+-rw-r--r--   0        0        0      514 2022-02-17 21:20:37.407934 autocensus-2.1.2/autocensus/resources/geo_ids.csv
+-rw-r--r--   0        0        0      182 2022-02-17 21:20:37.408243 autocensus-2.1.2/autocensus/resources/names.csv
+-rw-r--r--   0        0        0     7840 2023-01-19 19:59:43.878208 autocensus-2.1.2/autocensus/socrata.py
+-rw-r--r--   0        0        0     4674 2023-01-19 19:59:43.878938 autocensus-2.1.2/autocensus/utilities.py
+-rw-r--r--   0        0        0     1414 2023-05-26 17:48:20.881555 autocensus-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6731 2023-05-26 17:48:20.883041 autocensus-2.1.2/readme.md
+-rw-r--r--   0        0        0     8005 1970-01-01 00:00:00.000000 autocensus-2.1.2/setup.py
+-rw-r--r--   0        0        0     7983 1970-01-01 00:00:00.000000 autocensus-2.1.2/PKG-INFO
```

### Comparing `autocensus-2.1.1/LICENSE` & `autocensus-2.1.2/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) [year] [fullname]
+Copyright (c) 2023 Christopher Setzer
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `autocensus-2.1.1/autocensus/__init__.py` & `autocensus-2.1.2/autocensus/__init__.py`

 * *Files identical despite different names*

### Comparing `autocensus-2.1.1/autocensus/api.py` & `autocensus-2.1.2/autocensus/api.py`

 * *Files identical despite different names*

### Comparing `autocensus-2.1.1/autocensus/constants.py` & `autocensus-2.1.2/autocensus/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Dict, List, Optional, Tuple, Union
 
 from appdirs import user_cache_dir
 from pandas import DataFrame
 from typing_extensions import Literal
 
 # Cache directory path
-CACHE_DIRECTORY_PATH = Path(user_cache_dir('autocensus', 'socrata'))
+CACHE_DIRECTORY_PATH = Path(user_cache_dir('autocensus'))
 
 # Query parameters
 ESTIMATES = [1, 3, 5]
 QueryEstimate = Literal[1, 3, 5]
 GEOMETRIES = ['points', 'polygons']
 QueryGeometry = Literal['points', 'polygons']
 RESOLUTIONS = ['500k', '5m', '20m']
```

### Comparing `autocensus-2.1.1/autocensus/errors.py` & `autocensus-2.1.2/autocensus/errors.py`

 * *Files identical despite different names*

### Comparing `autocensus-2.1.1/autocensus/geography.py` & `autocensus-2.1.2/autocensus/geography.py`

 * *Files identical despite different names*

### Comparing `autocensus-2.1.1/autocensus/query.py` & `autocensus-2.1.2/autocensus/query.py`

 * *Files identical despite different names*

### Comparing `autocensus-2.1.1/autocensus/resources/annotations.csv` & `autocensus-2.1.2/autocensus/resources/annotations.csv`

 * *Files identical despite different names*

### Comparing `autocensus-2.1.1/autocensus/resources/columns.csv` & `autocensus-2.1.2/autocensus/resources/columns.csv`

 * *Files identical despite different names*

### Comparing `autocensus-2.1.1/autocensus/resources/geo_codes.csv` & `autocensus-2.1.2/autocensus/resources/geo_codes.csv`

 * *Files identical despite different names*

### Comparing `autocensus-2.1.1/autocensus/resources/geo_ids.csv` & `autocensus-2.1.2/autocensus/resources/geo_ids.csv`

 * *Files identical despite different names*

### Comparing `autocensus-2.1.1/autocensus/socrata.py` & `autocensus-2.1.2/autocensus/socrata.py`

 * *Files identical despite different names*

### Comparing `autocensus-2.1.1/autocensus/utilities.py` & `autocensus-2.1.2/autocensus/utilities.py`

 * *Files identical despite different names*

### Comparing `autocensus-2.1.1/pyproject.toml` & `autocensus-2.1.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 [tool.poetry]
 name = "autocensus"
-version = "2.1.1"
+version = "2.1.2"
 description = "A tool for collecting ACS and geospatial data from the Census API"
 license = "MIT"
-authors = ["Christopher Setzer <chris.setzer@socrata.com>"]
+authors = ["Christopher Setzer <cmsetzer.github@gmail.com>"]
 readme = "readme.md"
 homepage = "https://github.com/socrata/autocensus"
-keywords = ["census", "acs", "api", "data", "socrata"]
+keywords = ["census", "acs", "api", "data"]
 classifiers = [
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research"
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 appdirs = "^1.4.4"
-fiona = "^1.8.22"
-geopandas = "^0.12.2"
-httpx = "^0.23.3"
+fiona = "^1.9.4.post1"
+geopandas = "^0.13.0"
+httpx = "^0.24.1"
 nest-asyncio = "^1.5.6"
-pandas = "^1.5.3"
-shapely = "^2.0.0"
+pandas = "^2.0.1"
+shapely = "^2.0.1"
 socrata-py = "^1.1.13"
-tenacity = "^8.1.0"
-typing-extensions = "^4.4.0"
+tenacity = "^8.2.2"
+typing-extensions = "^4.6.2"
 us = "^2.0.2"
-yarl = "^1.8.2"
+yarl = "^1.9.2"
 
 [tool.poetry.group.dev.dependencies]
-black = "^22.12.0"
-mypy = "^0.991"
+black = "^23.3.0"
+mypy = "^1.3.0"
 pyinstrument = "^4.4.0"
-pytest = "^7.2.1"
-pytest-cov = "^4.0.0"
-ruff = "^0.0.226"
+pytest = "^7.3.1"
+pytest-cov = "^4.1.0"
+ruff = "^0.0.270"
+
 
 [tool.black]
 line-length = 99
 target-version = ["py38", "py39", "py310"]
 skip-string-normalization = true
 
 [tool.coverage.run]
```

### Comparing `autocensus-2.1.1/readme.md` & `autocensus-2.1.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,68 @@
+Metadata-Version: 2.1
+Name: autocensus
+Version: 2.1.2
+Summary: A tool for collecting ACS and geospatial data from the Census API
+Home-page: https://github.com/socrata/autocensus
+License: MIT
+Keywords: census,acs,api,data
+Author: Christopher Setzer
+Author-email: cmsetzer.github@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: appdirs (>=1.4.4,<2.0.0)
+Requires-Dist: fiona (>=1.9.4.post1,<2.0.0)
+Requires-Dist: geopandas (>=0.13.0,<0.14.0)
+Requires-Dist: httpx (>=0.24.1,<0.25.0)
+Requires-Dist: nest-asyncio (>=1.5.6,<2.0.0)
+Requires-Dist: pandas (>=2.0.1,<3.0.0)
+Requires-Dist: shapely (>=2.0.1,<3.0.0)
+Requires-Dist: socrata-py (>=1.1.13,<2.0.0)
+Requires-Dist: tenacity (>=8.2.2,<9.0.0)
+Requires-Dist: typing-extensions (>=4.6.2,<5.0.0)
+Requires-Dist: us (>=2.0.2,<3.0.0)
+Requires-Dist: yarl (>=1.9.2,<2.0.0)
+Description-Content-Type: text/markdown
+
 # autocensus
 
 A Python package for collecting American Community Survey (ACS) data and associated geometry from the [Census API] in a [pandas] dataframe.
 
 [Census API]: https://www.census.gov/developers
 [pandas]: https://pandas.pydata.org
 
 ## Contents
 
-* [Installation](#installation)
-* [Quickstart](#quickstart)
-* [Geometry](#geometry)
-  + [Points](#points)
-  + [Polygons](#polygons)
+- [Installation](#installation)
+- [Quickstart](#quickstart)
+- [Geometry](#geometry)
+  - [Points](#points)
+  - [Polygons](#polygons)
     - [Shapefile resolution](#shapefile-resolution)
     - [Shapefile caching](#shapefile-caching)
-* [Publishing to Socrata](#publishing-to-socrata)
-  + [Credentials](#credentials)
-  + [Example: Create a new dataset](#example-create-a-new-dataset)
-  + [Example: Replace rows in an existing dataset](#example-replace-rows-in-an-existing-dataset)
-  + [Example: Create a new dataset from multiple queries](#example-create-a-new-dataset-from-multiple-queries)
-* [Troubleshooting](#troubleshooting)
-  + [Clearing the cache](#clearing-the-cache)
 
 ## Installation
 
 autocensus requires Python 3.8 or higher. Install as follows:
 
 ```sh
 pip install autocensus
 ```
 
 To run autocensus, you must specify a [Census API key] via either the `census_api_key` keyword argument (as shown in the example below) or by setting the environment variable `CENSUS_API_KEY`.
 
+[Census API key]: https://api.census.gov/data/key_signup.html
+
 ## Quickstart
 
 ```python
 from autocensus import Query
 
 # Configure query
 query = Query(
@@ -53,48 +80,46 @@
 # Run query and collect output in dataframe
 dataframe = query.run()
 ```
 
 Output:
 
 | name                    | geo_id         | geo_type | year | date       | variable_code  | variable_label                                                                             | variable_concept                                  | annotation |  value | geometry  |
-|:------------------------|:---------------|:---------|-----:|:-----------|:---------------|:-------------------------------------------------------------------------------------------|:--------------------------------------------------|-----------:|-------:|:----------|
+| :---------------------- | :------------- | :------- | ---: | :--------- | :------------- | :----------------------------------------------------------------------------------------- | :------------------------------------------------ | ---------: | -----: | :-------- |
 | King County, Washington | 0500000US53033 | county   | 2017 | 2017-12-31 | DP03_0025E     | Estimate!!COMMUTING TO WORK!!Mean travel time to work (minutes)                            | SELECTED ECONOMIC CHARACTERISTICS                 |            |   30.0 | POINT (…) |
 | King County, Washington | 0500000US53033 | county   | 2018 | 2018-12-31 | DP03_0025E     | Estimate!!COMMUTING TO WORK!!Workers 16 years and over!!Mean travel time to work (minutes) | SELECTED ECONOMIC CHARACTERISTICS                 |            |   30.2 | POINT (…) |
 | King County, Washington | 0500000US53033 | county   | 2017 | 2017-12-31 | S0103_C01_104E | Total!!Estimate!!GROSS RENT!!Median gross rent (dollars)                                   | POPULATION 65 YEARS AND OVER IN THE UNITED STATES |            | 1555.0 | POINT (…) |
 | King County, Washington | 0500000US53033 | county   | 2018 | 2018-12-31 | S0103_C01_104E | Estimate!!Total!!Renter-occupied housing units!!GROSS RENT!!Median gross rent (dollars)    | POPULATION 65 YEARS AND OVER IN THE UNITED STATES |            | 1674.0 | POINT (…) |
 
-[Census API key]: https://api.census.gov/data/key_signup.html
-
 ## Geometry
 
 autocensus supports point- and polygon-based geometry data for many years and geographies by way of the Census Bureau's [Gazetteer Files] and [Cartographic Boundary Files].
 
 Here's how to add geometry to your data:
 
 [Gazetteer Files]: https://www.census.gov/geographies/reference-files/time-series/geo/gazetteer-files.html
 [Cartographic Boundary Files]: https://www.census.gov/geographies/mapping-files/time-series/geo/carto-boundary-file.html
 
 ### Points
 
 Point data from the Census Bureau's Gazetteer Files is generally available for years from 2012 on in the following geographies:
 
-* Nation-level
-  + `urban area`
-  + `zip code tabulation area`
-  + `county`
-  + `congressional district`
-  + `metropolitan statistical area/micropolitan statistical area`
-  + `american indian area/alaska native area/hawaiian home land`
-* State-level
-  + `county subdivision`
-  + `tract`
-  + `place`
-  + `state legislative district (upper chamber)`
-  + `state legislative district (lower chamber)`
+- Nation-level
+  - `urban area`
+  - `zip code tabulation area`
+  - `county`
+  - `congressional district`
+  - `metropolitan statistical area/micropolitan statistical area`
+  - `american indian area/alaska native area/hawaiian home land`
+- State-level
+  - `county subdivision`
+  - `tract`
+  - `place`
+  - `state legislative district (upper chamber)`
+  - `state legislative district (lower chamber)`
 
 Example:
 
 ```python
 from autocensus import Query
 
 query = Query(
@@ -108,36 +133,36 @@
 dataframe = query.run()
 ```
 
 ### Polygons
 
 Polygon data from the Census Bureau's Cartographic Boundary Shapefiles is generally available for years from 2013 on in the following geographies:
 
-* Nation-level
-  + `nation`
-  + `region`
-  + `division`
-  + `state`
-  + `urban area`
-  + `zip code tabulation area`
-  + `county`
-  + `congressional district`
-  + `metropolitan statistical area/micropolitan statistical area`
-  + `combined statistical area`
-  + `american indian area/alaska native area/hawaiian home land`
-  + `new england city and town area`
-* State-level
-  + `alaska native regional corporation`
-  + `block group`
-  + `county subdivision`
-  + `tract`
-  + `place`
-  + `public use microdata area`
-  + `state legislative district (upper chamber)`
-  + `state legislative district (lower chamber)`
+- Nation-level
+  - `nation`
+  - `region`
+  - `division`
+  - `state`
+  - `urban area`
+  - `zip code tabulation area`
+  - `county`
+  - `congressional district`
+  - `metropolitan statistical area/micropolitan statistical area`
+  - `combined statistical area`
+  - `american indian area/alaska native area/hawaiian home land`
+  - `new england city and town area`
+- State-level
+  - `alaska native regional corporation`
+  - `block group`
+  - `county subdivision`
+  - `tract`
+  - `place`
+  - `public use microdata area`
+  - `state legislative district (upper chamber)`
+  - `state legislative district (lower chamber)`
 
 Example:
 
 ```python
 from autocensus import Query
 
 query = Query(
@@ -170,78 +195,19 @@
 )
 ```
 
 Setting a specific resolution is only supported for polygon-based geometry.
 
 #### Shapefile caching
 
-To improve performance across queries that include polygon-based geometry data, autocensus caches shapefiles on disk by default. The cache location varies by platform:
-
-* Linux: `/home/{username}/.cache/autocensus`
-* Mac: `/Users/{username}/Library/Application Support/Caches/autocensus`
-* Windows: `C:\Users\{username}\AppData\Local\socrata\autocensus`
-
-You can clear the cache by manually deleting the cache directory or by executing the `autocensus.clear_cache` function. See the section [Troubleshooting: Clearing the cache] for more details.
-
-[Troubleshooting: Clearing the cache]: #clearing-the-cache
-
-## Publishing to Socrata
-
-If you have publishing permissions on a Socrata domain, you can publish your query results directly to Socrata via the method `Query.to_socrata`. This method uses [socrata-py] to upload your dataframe with the appropriate field types, formatting, and metadata.
-
-**Note:** autocensus will drop built-in support for Socrata uploads in a future version. Please see the [socrata-py] docs for guidance on dataframe ingress.
-
-[socrata-py]: https://github.com/socrata/socrata-py
-
-### Credentials
-
-You must have a Socrata account with appropriate permissions on the domain to which you are publishing. By default, autocensus will look up your Socrata account credentials under the following pairs of common environment variables:
-
-* `SOCRATA_KEY_ID`, `SOCRATA_KEY_SECRET`
-* `SOCRATA_USERNAME`, `SOCRATA_PASSWORD`
-* `MY_SOCRATA_USERNAME`, `MY_SOCRATA_PASSWORD`
-* `SODA_USERNAME`, `SODA_PASSWORD`
-
-Alternatively, you can supply credentials explicitly by way of the `auth` keyword argument:
+To improve performance across queries that include polygon-based geometry data, autocensus will cache Census shapefiles on disk by default. The cache directory location depends on your OS; you can look it up from `autocensus.constants.CACHE_DIRECTORY_PATH` like so:
 
-```python
-auth = (os.environ['MY_SOCRATA_KEY'], os.environ['MY_SOCRATA_KEY_SECRET'])
-query.to_socrata(
-    'some-domain.data.socrata.com',
-    auth=auth
-)
-```
-
-### Example: Create a new dataset
-
-```python
-# Run query and publish results as a new dataset on Socrata domain
-query.to_socrata(
-    'some-domain.data.socrata.com',
-    name='Median Commute Time by Colorado County, 2013–2017',  # Optional
-    description='1-year estimates from the American Community Survey'  # Optional
-)
-```
-
-### Example: Replace rows in an existing dataset
-
-```python
-# Run query and publish results to an existing dataset on Socrata domain
-query.to_socrata(
-    'some-domain.data.socrata.com',
-    dataset_id='xxxx-xxxx'
-)
+```shell
+python -c "import autocensus; print(autocensus.constants.CACHE_DIRECTORY_PATH)"
 ```
 
-## Troubleshooting
-
-### Clearing the cache
-
-Sometimes it is useful to clear the [cache directory] that autocensus uses to store downloaded shapefiles for future queries, especially if you're running into `BadZipFile: File is not a zip file` errors or other shapefile-related problems. Clear your cache like so:
-
-```python
-import autocensus
+Sometimes it is useful to clear this cache directory, especially if you're running into persistent shapefile-related problems. You can clear the cache by manually deleting the cache directory or by executing the `autocensus.clear_cache` function:
 
-autocensus.clear_cache()
+```shell
+python -c "import autocensus; autocensus.clear_cache()"
 ```
 
-[cache directory]: #shapefile-caching
```

