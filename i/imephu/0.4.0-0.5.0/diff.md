# Comparing `tmp/imephu-0.4.0.tar.gz` & `tmp/imephu-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imephu-0.4.0.tar", max compression
+gzip compressed data, was "imephu-0.5.0.tar", max compression
```

## Comparing `imephu-0.4.0.tar` & `imephu-0.5.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1102 2023-07-10 14:47:42.674953 imephu-0.4.0/LICENSE
--rw-r--r--   0        0        0     1015 2023-07-10 14:47:42.675169 imephu-0.4.0/README.md
--rw-r--r--   0        0        0      991 2023-07-14 17:06:28.688837 imephu-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      235 2023-07-12 17:32:34.546165 imephu-0.4.0/src/imephu/__init__.py
--rw-r--r--   0        0        0     1550 2023-07-10 14:47:42.735797 imephu-0.4.0/src/imephu/annotation/__init__.py
--rw-r--r--   0        0        0      746 2023-07-10 14:47:42.736360 imephu-0.4.0/src/imephu/annotation/general/__init__.py
--rw-r--r--   0        0        0     4480 2023-07-10 14:47:42.736748 imephu-0.4.0/src/imephu/annotation/general/arrow.py
--rw-r--r--   0        0        0     3879 2023-07-10 14:47:42.737079 imephu-0.4.0/src/imephu/annotation/general/circle.py
--rw-r--r--   0        0        0     2581 2023-07-10 14:47:42.737385 imephu-0.4.0/src/imephu/annotation/general/crosshairs.py
--rw-r--r--   0        0        0     1646 2023-07-10 14:47:42.737673 imephu-0.4.0/src/imephu/annotation/general/empty.py
--rw-r--r--   0        0        0     3021 2023-07-10 14:47:42.738079 imephu-0.4.0/src/imephu/annotation/general/group.py
--rw-r--r--   0        0        0     4428 2023-07-10 14:47:42.738417 imephu-0.4.0/src/imephu/annotation/general/line_path.py
--rw-r--r--   0        0        0     4425 2023-07-10 14:47:42.738680 imephu-0.4.0/src/imephu/annotation/general/rectangle.py
--rw-r--r--   0        0        0     5316 2023-07-10 14:47:42.738939 imephu-0.4.0/src/imephu/annotation/general/text.py
--rw-r--r--   0        0        0     9170 2023-07-10 14:47:42.739226 imephu-0.4.0/src/imephu/annotation/motion.py
--rw-r--r--   0        0        0    12400 2023-07-14 17:06:28.689624 imephu-0.4.0/src/imephu/cli.py
--rw-r--r--   0        0        0    12907 2023-07-10 14:47:42.739791 imephu-0.4.0/src/imephu/finder_chart.py
--rw-r--r--   0        0        0     9710 2023-07-10 14:47:42.740083 imephu-0.4.0/src/imephu/geometry.py
--rw-r--r--   0        0        0        0 2023-07-10 14:47:42.740215 imephu-0.4.0/src/imephu/py.typed
--rw-r--r--   0        0        0        0 2023-07-10 14:47:42.740669 imephu-0.4.0/src/imephu/salt/annotation/__init__.py
--rw-r--r--   0        0        0    12623 2023-07-12 17:32:34.547738 imephu-0.4.0/src/imephu/salt/annotation/nir.py
--rw-r--r--   0        0        0     4365 2023-07-14 17:06:28.691527 imephu-0.4.0/src/imephu/salt/annotation/rss.py
--rw-r--r--   0        0        0     1195 2023-07-10 14:47:42.741408 imephu-0.4.0/src/imephu/salt/annotation/salticam.py
--rw-r--r--   0        0        0     9004 2023-07-10 14:47:42.741632 imephu-0.4.0/src/imephu/salt/annotation/telescope.py
--rw-r--r--   0        0        0    15615 2023-07-14 17:06:28.692233 imephu-0.4.0/src/imephu/salt/finder_chart.py
--rw-r--r--   0        0        0     4859 2023-07-10 14:47:42.742110 imephu-0.4.0/src/imephu/salt/utils.py
--rw-r--r--   0        0        0    10500 2023-07-14 17:06:28.692870 imephu-0.4.0/src/imephu/schema.json
--rw-r--r--   0        0        0     9472 2023-07-10 14:47:42.742725 imephu-0.4.0/src/imephu/service/horizons.py
--rw-r--r--   0        0        0    15225 2023-07-10 14:47:42.742998 imephu-0.4.0/src/imephu/service/survey.py
--rw-r--r--   0        0        0     3680 2023-07-10 14:47:42.743218 imephu-0.4.0/src/imephu/utils.py
--rw-r--r--   0        0        0     1876 1970-01-01 00:00:00.000000 imephu-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1102 2023-07-10 14:47:42.674953 imephu-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1015 2023-07-10 14:47:42.675169 imephu-0.5.0/README.md
+-rw-r--r--   0        0        0      991 2023-07-18 15:32:46.998895 imephu-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      235 2023-07-12 17:32:34.546165 imephu-0.5.0/src/imephu/__init__.py
+-rw-r--r--   0        0        0     1550 2023-07-10 14:47:42.735797 imephu-0.5.0/src/imephu/annotation/__init__.py
+-rw-r--r--   0        0        0      746 2023-07-10 14:47:42.736360 imephu-0.5.0/src/imephu/annotation/general/__init__.py
+-rw-r--r--   0        0        0     4480 2023-07-10 14:47:42.736748 imephu-0.5.0/src/imephu/annotation/general/arrow.py
+-rw-r--r--   0        0        0     3879 2023-07-10 14:47:42.737079 imephu-0.5.0/src/imephu/annotation/general/circle.py
+-rw-r--r--   0        0        0     2581 2023-07-10 14:47:42.737385 imephu-0.5.0/src/imephu/annotation/general/crosshairs.py
+-rw-r--r--   0        0        0     1646 2023-07-10 14:47:42.737673 imephu-0.5.0/src/imephu/annotation/general/empty.py
+-rw-r--r--   0        0        0     3021 2023-07-10 14:47:42.738079 imephu-0.5.0/src/imephu/annotation/general/group.py
+-rw-r--r--   0        0        0     4428 2023-07-10 14:47:42.738417 imephu-0.5.0/src/imephu/annotation/general/line_path.py
+-rw-r--r--   0        0        0     4425 2023-07-10 14:47:42.738680 imephu-0.5.0/src/imephu/annotation/general/rectangle.py
+-rw-r--r--   0        0        0     5316 2023-07-10 14:47:42.738939 imephu-0.5.0/src/imephu/annotation/general/text.py
+-rw-r--r--   0        0        0     9170 2023-07-10 14:47:42.739226 imephu-0.5.0/src/imephu/annotation/motion.py
+-rw-r--r--   0        0        0    12400 2023-07-14 17:06:28.689624 imephu-0.5.0/src/imephu/cli.py
+-rw-r--r--   0        0        0    12907 2023-07-10 14:47:42.739791 imephu-0.5.0/src/imephu/finder_chart.py
+-rw-r--r--   0        0        0     9710 2023-07-10 14:47:42.740083 imephu-0.5.0/src/imephu/geometry.py
+-rw-r--r--   0        0        0        0 2023-07-10 14:47:42.740215 imephu-0.5.0/src/imephu/py.typed
+-rw-r--r--   0        0        0        0 2023-07-10 14:47:42.740669 imephu-0.5.0/src/imephu/salt/annotation/__init__.py
+-rw-r--r--   0        0        0    12623 2023-07-12 17:32:34.547738 imephu-0.5.0/src/imephu/salt/annotation/nir.py
+-rw-r--r--   0        0        0     4365 2023-07-14 17:06:28.691527 imephu-0.5.0/src/imephu/salt/annotation/rss.py
+-rw-r--r--   0        0        0     1195 2023-07-10 14:47:42.741408 imephu-0.5.0/src/imephu/salt/annotation/salticam.py
+-rw-r--r--   0        0        0     9004 2023-07-10 14:47:42.741632 imephu-0.5.0/src/imephu/salt/annotation/telescope.py
+-rw-r--r--   0        0        0    15615 2023-07-14 17:06:28.692233 imephu-0.5.0/src/imephu/salt/finder_chart.py
+-rw-r--r--   0        0        0     4859 2023-07-10 14:47:42.742110 imephu-0.5.0/src/imephu/salt/utils.py
+-rw-r--r--   0        0        0    10500 2023-07-14 17:06:28.692870 imephu-0.5.0/src/imephu/schema.json
+-rw-r--r--   0        0        0     9716 2023-07-18 15:32:47.000288 imephu-0.5.0/src/imephu/service/horizons.py
+-rw-r--r--   0        0        0    15225 2023-07-10 14:47:42.742998 imephu-0.5.0/src/imephu/service/survey.py
+-rw-r--r--   0        0        0     4149 2023-07-18 15:32:47.001155 imephu-0.5.0/src/imephu/utils.py
+-rw-r--r--   0        0        0     1876 1970-01-01 00:00:00.000000 imephu-0.5.0/PKG-INFO
```

### Comparing `imephu-0.4.0/LICENSE` & `imephu-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `imephu-0.4.0/README.md` & `imephu-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `imephu-0.4.0/pyproject.toml` & `imephu-0.5.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "imephu"
-version = "0.4.0"
+version = "0.5.0"
 description = "Generate finder charts for astronomical observations."
 authors = ["Southern African Large Telescope"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `imephu-0.4.0/src/imephu/annotation/__init__.py` & `imephu-0.5.0/src/imephu/annotation/__init__.py`

 * *Files identical despite different names*

### Comparing `imephu-0.4.0/src/imephu/annotation/general/__init__.py` & `imephu-0.5.0/src/imephu/annotation/general/__init__.py`

 * *Files identical despite different names*

### Comparing `imephu-0.4.0/src/imephu/annotation/general/arrow.py` & `imephu-0.5.0/src/imephu/annotation/general/arrow.py`

 * *Files identical despite different names*

### Comparing `imephu-0.4.0/src/imephu/annotation/general/circle.py` & `imephu-0.5.0/src/imephu/annotation/general/circle.py`

 * *Files identical despite different names*

### Comparing `imephu-0.4.0/src/imephu/annotation/general/crosshairs.py` & `imephu-0.5.0/src/imephu/annotation/general/crosshairs.py`

 * *Files identical despite different names*

### Comparing `imephu-0.4.0/src/imephu/annotation/general/empty.py` & `imephu-0.5.0/src/imephu/annotation/general/empty.py`

 * *Files identical despite different names*

### Comparing `imephu-0.4.0/src/imephu/annotation/general/group.py` & `imephu-0.5.0/src/imephu/annotation/general/group.py`

 * *Files identical despite different names*

### Comparing `imephu-0.4.0/src/imephu/annotation/general/line_path.py` & `imephu-0.5.0/src/imephu/annotation/general/line_path.py`

 * *Files identical despite different names*

### Comparing `imephu-0.4.0/src/imephu/annotation/general/rectangle.py` & `imephu-0.5.0/src/imephu/annotation/general/rectangle.py`

 * *Files identical despite different names*

### Comparing `imephu-0.4.0/src/imephu/annotation/general/text.py` & `imephu-0.5.0/src/imephu/annotation/general/text.py`

 * *Files identical despite different names*

### Comparing `imephu-0.4.0/src/imephu/annotation/motion.py` & `imephu-0.5.0/src/imephu/annotation/motion.py`

 * *Files identical despite different names*

### Comparing `imephu-0.4.0/src/imephu/cli.py` & `imephu-0.5.0/src/imephu/cli.py`

 * *Files identical despite different names*

### Comparing `imephu-0.4.0/src/imephu/finder_chart.py` & `imephu-0.5.0/src/imephu/finder_chart.py`

 * *Files identical despite different names*

### Comparing `imephu-0.4.0/src/imephu/geometry.py` & `imephu-0.5.0/src/imephu/geometry.py`

 * *Files identical despite different names*

### Comparing `imephu-0.4.0/src/imephu/salt/annotation/nir.py` & `imephu-0.5.0/src/imephu/salt/annotation/nir.py`

 * *Files identical despite different names*

### Comparing `imephu-0.4.0/src/imephu/salt/annotation/rss.py` & `imephu-0.5.0/src/imephu/salt/annotation/rss.py`

 * *Files identical despite different names*

### Comparing `imephu-0.4.0/src/imephu/salt/annotation/salticam.py` & `imephu-0.5.0/src/imephu/salt/annotation/salticam.py`

 * *Files identical despite different names*

### Comparing `imephu-0.4.0/src/imephu/salt/annotation/telescope.py` & `imephu-0.5.0/src/imephu/salt/annotation/telescope.py`

 * *Files identical despite different names*

### Comparing `imephu-0.4.0/src/imephu/salt/finder_chart.py` & `imephu-0.5.0/src/imephu/salt/finder_chart.py`

 * *Files identical despite different names*

### Comparing `imephu-0.4.0/src/imephu/salt/utils.py` & `imephu-0.5.0/src/imephu/salt/utils.py`

 * *Files identical despite different names*

### Comparing `imephu-0.4.0/src/imephu/schema.json` & `imephu-0.5.0/src/imephu/schema.json`

 * *Files identical despite different names*

### Comparing `imephu-0.4.0/src/imephu/service/horizons.py` & `imephu-0.5.0/src/imephu/service/horizons.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import List, Optional
 
 from astropy import units as u
 from astropy.coordinates import SkyCoord
 from astropy.units import Quantity
 from astroquery.jplhorizons import Horizons
 from dateutil.parser import parse
-from imephu.utils import Ephemeris, MagnitudeRange
+from imephu.utils import Ephemeris, MagnitudeRange, SkyCoordRate
 
 
 class HorizonsService:
     """A service for querying ephemerides from JPL Horizons.
 
     The service is initialised by calling the constructor with a start and end time,
     and ephemerides can be queried with the `ephemerides` method, which takes a start
@@ -174,24 +174,27 @@
 
         # store the ephemerides in the format we need
         self._ephemerides = []
         for row in range(len(ephemerides)):
             epoch = parse(ephemerides["datetime_str"][row]).replace(tzinfo=timezone.utc)
             ra = float(ephemerides["RA"][row]) * u.deg
             dec = float(ephemerides["DEC"][row]) * u.deg
+            ra_rate = float(ephemerides["RA_rate"][row]) * u.arcsec / u.hour
+            dec_rate = float(ephemerides["DEC_rate"][row]) * u.arcsec / u.hour
             if "V" in ephemerides.keys():
                 magnitude = float(ephemerides["V"][row])
                 magnitude_range = MagnitudeRange(
                     min_magnitude=magnitude, max_magnitude=magnitude, bandpass="V"
                 )
             else:
                 magnitude_range = None
             self._ephemerides.append(
                 Ephemeris(
                     position=SkyCoord(ra=ra, dec=dec),
+                    position_rate=SkyCoordRate(ra=ra_rate, dec=dec_rate),
                     magnitude_range=magnitude_range,
                     epoch=epoch,
                 )
             )
 
     def _cover_time_interval(self, start: datetime, end: datetime) -> List[Ephemeris]:
         """Find the smallest list of ephemerides covering a time interval."""
```

### Comparing `imephu-0.4.0/src/imephu/service/survey.py` & `imephu-0.5.0/src/imephu/service/survey.py`

 * *Files identical despite different names*

### Comparing `imephu-0.4.0/src/imephu/utils.py` & `imephu-0.5.0/src/imephu/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,30 @@
 from dataclasses import dataclass
 from datetime import datetime
 from typing import List, Optional
 
 from astropy.coordinates import SkyCoord
+from astropy.units import Quantity
+
+
+@dataclass
+class SkyCoordRate:
+    """A rate of change in position on the sky.
+
+    Attributes
+    ----------
+    ra: `~astropy.unit.Quantity`
+        The rate of change in right ascension.
+    dec: `~astropy.unit.Quantity`
+        The rate of change in declination.
+    """
+
+    ra: Quantity
+
+    dec: Quantity
 
 
 @dataclass
 class MagnitudeRange:
     """A magnitude range.
 
     Attributes
@@ -31,22 +49,26 @@
     Parameters
     ----------
     epoch: `~datetime.datetime`
         The epoch, i.e. the datetime for which the position is given. The epoch must be
         a timezone-aware datetime.
     position: `~astropy.coordinates.SkyCoord`
         The position, in right ascension and declination.
+    position_rate: SkyCoordRate
+        The rate of change in the position on the sky.
     magnitude_range: `~imephu.utils.MagnitudeRange`
         The magnitude range.
     """
 
     epoch: datetime
 
     position: SkyCoord
 
+    position_rate: SkyCoordRate
+
     magnitude_range: Optional[MagnitudeRange]
 
     def __post_init__(self) -> None:
         """Check that the epoch is timezone-aware."""
         if self.epoch.tzinfo is None or self.epoch.tzinfo.utcoffset(None) is None:
             raise ValueError("The epoch must be a timezone-aware datetime object.")
```

### Comparing `imephu-0.4.0/PKG-INFO` & `imephu-0.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imephu
-Version: 0.4.0
+Version: 0.5.0
 Summary: Generate finder charts for astronomical observations.
 License: MIT
 Author: Southern African Large Telescope
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

