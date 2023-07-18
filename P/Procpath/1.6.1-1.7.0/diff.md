# Comparing `tmp/Procpath-1.6.1.tar.gz` & `tmp/Procpath-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Procpath-1.6.1.tar", last modified: Sun Sep 18 15:14:06 2022, max compression
+gzip compressed data, was "Procpath-1.7.0.tar", last modified: Tue Jul 18 21:51:18 2023, max compression
```

## Comparing `Procpath-1.6.1.tar` & `Procpath-1.7.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2022-09-18 15:14:06.164324 Procpath-1.6.1/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5274 2022-09-18 15:14:06.164324 Procpath-1.6.1/PKG-INFO
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2022-09-18 15:14:06.152322 Procpath-1.6.1/Procpath.egg-info/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5274 2022-09-18 15:14:05.000000 Procpath-1.6.1/Procpath.egg-info/PKG-INFO
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      590 2022-09-18 15:14:06.000000 Procpath-1.6.1/Procpath.egg-info/SOURCES.txt
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        1 2022-09-18 15:14:05.000000 Procpath-1.6.1/Procpath.egg-info/dependency_links.txt
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       47 2022-09-18 15:14:05.000000 Procpath-1.6.1/Procpath.egg-info/entry_points.txt
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       81 2022-09-18 15:14:05.000000 Procpath-1.6.1/Procpath.egg-info/requires.txt
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        9 2022-09-18 15:14:06.000000 Procpath-1.6.1/Procpath.egg-info/top_level.txt
--rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     4013 2022-09-18 14:35:24.000000 Procpath-1.6.1/README.rst
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2022-09-18 15:14:06.160323 Procpath-1.6.1/procpath/
--rw-rw-rw-   0 nobody   (65534) nogroup  (65534)       22 2022-09-18 14:35:24.000000 Procpath-1.6.1/procpath/__init__.py
--rw-rw-rw-   0 nobody   (65534) nogroup  (65534)       62 2022-09-18 14:35:24.000000 Procpath-1.6.1/procpath/__main__.py
--rw-rw-rw-   0 nobody   (65534) nogroup  (65534)    16414 2022-09-18 14:35:24.000000 Procpath-1.6.1/procpath/cli.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2022-09-18 15:14:06.164324 Procpath-1.6.1/procpath/cmd/
--rw-rw-rw-   0 nobody   (65534) nogroup  (65534)      408 2022-09-18 14:35:24.000000 Procpath-1.6.1/procpath/cmd/__init__.py
--rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     3535 2022-09-18 14:35:24.000000 Procpath-1.6.1/procpath/cmd/explore.py
--rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     1482 2022-09-18 14:35:24.000000 Procpath-1.6.1/procpath/cmd/play.py
--rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     3225 2022-09-18 14:35:24.000000 Procpath-1.6.1/procpath/cmd/plot.py
--rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     1588 2022-09-18 14:35:24.000000 Procpath-1.6.1/procpath/cmd/query.py
--rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     1887 2022-09-18 14:35:24.000000 Procpath-1.6.1/procpath/cmd/record.py
--rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     5303 2022-09-18 14:35:24.000000 Procpath-1.6.1/procpath/cmd/watch.py
--rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     8070 2022-09-18 14:35:24.000000 Procpath-1.6.1/procpath/playbook.py
--rw-rw-rw-   0 nobody   (65534) nogroup  (65534)    17111 2022-09-18 14:35:24.000000 Procpath-1.6.1/procpath/plotting.py
--rw-rw-rw-   0 nobody   (65534) nogroup  (65534)    27763 2022-09-18 14:35:24.000000 Procpath-1.6.1/procpath/procfile.py
--rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     2868 2022-09-18 14:35:24.000000 Procpath-1.6.1/procpath/procrec.py
--rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     5559 2022-09-18 14:35:24.000000 Procpath-1.6.1/procpath/procret.py
--rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     8532 2022-09-18 14:35:24.000000 Procpath-1.6.1/procpath/proctree.py
--rw-rw-rw-   0 nobody   (65534) nogroup  (65534)   178572 2022-09-18 14:35:24.000000 Procpath-1.6.1/procpath/test.py
--rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     1320 2022-09-18 14:35:24.000000 Procpath-1.6.1/procpath/utility.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       38 2022-09-18 15:14:06.164324 Procpath-1.6.1/setup.cfg
--rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     1896 2022-09-18 14:35:24.000000 Procpath-1.6.1/setup.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-18 21:51:18.981577 Procpath-1.7.0/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5305 2023-07-18 21:51:18.981577 Procpath-1.7.0/PKG-INFO
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-18 21:51:18.969577 Procpath-1.7.0/Procpath.egg-info/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5305 2023-07-18 21:51:18.000000 Procpath-1.7.0/Procpath.egg-info/PKG-INFO
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      590 2023-07-18 21:51:18.000000 Procpath-1.7.0/Procpath.egg-info/SOURCES.txt
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        1 2023-07-18 21:51:18.000000 Procpath-1.7.0/Procpath.egg-info/dependency_links.txt
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       47 2023-07-18 21:51:18.000000 Procpath-1.7.0/Procpath.egg-info/entry_points.txt
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      103 2023-07-18 21:51:18.000000 Procpath-1.7.0/Procpath.egg-info/requires.txt
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        9 2023-07-18 21:51:18.000000 Procpath-1.7.0/Procpath.egg-info/top_level.txt
+-rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     4013 2023-07-18 21:40:12.000000 Procpath-1.7.0/README.rst
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-18 21:51:18.977577 Procpath-1.7.0/procpath/
+-rw-rw-rw-   0 nobody   (65534) nogroup  (65534)       22 2023-07-18 21:40:12.000000 Procpath-1.7.0/procpath/__init__.py
+-rw-rw-rw-   0 nobody   (65534) nogroup  (65534)       62 2023-07-18 21:40:12.000000 Procpath-1.7.0/procpath/__main__.py
+-rw-rw-rw-   0 nobody   (65534) nogroup  (65534)    16582 2023-07-18 21:40:12.000000 Procpath-1.7.0/procpath/cli.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-18 21:51:18.981577 Procpath-1.7.0/procpath/cmd/
+-rw-rw-rw-   0 nobody   (65534) nogroup  (65534)      408 2023-07-18 21:40:12.000000 Procpath-1.7.0/procpath/cmd/__init__.py
+-rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     3535 2023-07-18 21:40:12.000000 Procpath-1.7.0/procpath/cmd/explore.py
+-rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     1482 2023-07-18 21:40:12.000000 Procpath-1.7.0/procpath/cmd/play.py
+-rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     3283 2023-07-18 21:40:12.000000 Procpath-1.7.0/procpath/cmd/plot.py
+-rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     1588 2023-07-18 21:40:12.000000 Procpath-1.7.0/procpath/cmd/query.py
+-rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     1887 2023-07-18 21:40:12.000000 Procpath-1.7.0/procpath/cmd/record.py
+-rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     5303 2023-07-18 21:40:12.000000 Procpath-1.7.0/procpath/cmd/watch.py
+-rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     8070 2023-07-18 21:40:12.000000 Procpath-1.7.0/procpath/playbook.py
+-rw-rw-rw-   0 nobody   (65534) nogroup  (65534)    18994 2023-07-18 21:40:12.000000 Procpath-1.7.0/procpath/plotting.py
+-rw-rw-rw-   0 nobody   (65534) nogroup  (65534)    27763 2023-07-18 21:40:12.000000 Procpath-1.7.0/procpath/procfile.py
+-rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     2868 2023-07-18 21:40:12.000000 Procpath-1.7.0/procpath/procrec.py
+-rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     5559 2023-07-18 21:40:12.000000 Procpath-1.7.0/procpath/procret.py
+-rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     8532 2023-07-18 21:40:12.000000 Procpath-1.7.0/procpath/proctree.py
+-rw-rw-rw-   0 nobody   (65534) nogroup  (65534)   182860 2023-07-18 21:40:12.000000 Procpath-1.7.0/procpath/test.py
+-rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     1388 2023-07-18 21:40:12.000000 Procpath-1.7.0/procpath/utility.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       38 2023-07-18 21:51:18.981577 Procpath-1.7.0/setup.cfg
+-rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     1985 2023-07-18 21:40:12.000000 Procpath-1.7.0/setup.py
```

### Comparing `Procpath-1.6.1/PKG-INFO` & `Procpath-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: Procpath
-Version: 1.6.1
+Version: 1.7.0
 Summary: Procpath is a process tree analysis workbench
 Home-page: https://heptapod.host/saajns/procpath
 Author: saaj
 Author-email: mail@saaj.me
 License: LGPL-3.0-only
 Project-URL: Source Code, https://heptapod.host/saajns/procpath
 Project-URL: Documentation, https://procpath.readthedocs.io/
 Project-URL: Release Notes, https://procpath.readthedocs.io/en/latest/history.html
 Keywords: procfs jsonpath sqlite plotting
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Requires-Python: >= 3.7
 Provides-Extra: manual
 
@@ -141,9 +141,7 @@
    procpath plot -d out.sqlite -o out.svg -q cpu -q rss
 
 .. image:: https://heptapod.host/saajns/procpath/-/raw/8884bb/manual/_static/default_rss_vs_cpu.svg
    :alt: Procpath RSS vs CPU SVG
 
 
 .. _pipx: https://pypi.org/project/pipx/
-
-
```

### Comparing `Procpath-1.6.1/Procpath.egg-info/PKG-INFO` & `Procpath-1.7.0/Procpath.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: Procpath
-Version: 1.6.1
+Version: 1.7.0
 Summary: Procpath is a process tree analysis workbench
 Home-page: https://heptapod.host/saajns/procpath
 Author: saaj
 Author-email: mail@saaj.me
 License: LGPL-3.0-only
 Project-URL: Source Code, https://heptapod.host/saajns/procpath
 Project-URL: Documentation, https://procpath.readthedocs.io/
 Project-URL: Release Notes, https://procpath.readthedocs.io/en/latest/history.html
 Keywords: procfs jsonpath sqlite plotting
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Requires-Python: >= 3.7
 Provides-Extra: manual
 
@@ -141,9 +141,7 @@
    procpath plot -d out.sqlite -o out.svg -q cpu -q rss
 
 .. image:: https://heptapod.host/saajns/procpath/-/raw/8884bb/manual/_static/default_rss_vs_cpu.svg
    :alt: Procpath RSS vs CPU SVG
 
 
 .. _pipx: https://pypi.org/project/pipx/
-
-
```

### Comparing `Procpath-1.6.1/Procpath.egg-info/SOURCES.txt` & `Procpath-1.7.0/Procpath.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Procpath-1.6.1/README.rst` & `Procpath-1.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `Procpath-1.6.1/procpath/cli.py` & `Procpath-1.7.0/procpath/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,14 +238,19 @@
         help='Override plot title.',
     )
     plot_control.add_argument(
         '--no-dots',
         action='store_true',
         help='Do not add hover dots to the lines.',
     )
+    plot_control.add_argument(
+        '--relative-time',
+        action='store_true',
+        help='Display X axis as time deltas since the first measurement.',
+    )
     postprocessing_control = parser.add_argument_group('post-processing control arguments')
     postprocessing_control.add_argument(
         '-e', '--epsilon',
         type=float,
         help='Reduce points using Ramer-Douglas-Peucker algorithm and given ε.',
     )
     postprocessing_control.add_argument(
```

### Comparing `Procpath-1.6.1/procpath/cmd/explore.py` & `Procpath-1.7.0/procpath/cmd/explore.py`

 * *Files identical despite different names*

### Comparing `Procpath-1.6.1/procpath/cmd/play.py` & `Procpath-1.7.0/procpath/cmd/play.py`

 * *Files identical despite different names*

### Comparing `Procpath-1.6.1/procpath/cmd/plot.py` & `Procpath-1.7.0/procpath/cmd/plot.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import itertools
 from datetime import datetime
-from typing import Iterable, List, Mapping, Optional, Tuple
+from typing import Iterable, List, Mapping, Optional
 
 from .. import plotting, procret
 from . import CommandError
 
 
 __all__ = 'run',
 
@@ -30,15 +30,15 @@
             yield procret.Query(f.read(), 'Custom query')
 
 
 def _get_pid_series_points(
     timeseries: List[Mapping],
     epsilon: Optional[float] = None,
     moving_average_window: Optional[int] = None,
-) -> Mapping[int, List[Tuple[float, float]]]:
+) -> Mapping[int, List[plotting.Point]]:
     pid_series = {}
     for pid, series in itertools.groupby(timeseries, lambda r: r['pid']):
         series = [(r['ts'], r['value']) for r in series]
         if moving_average_window:
             series = list(plotting.moving_average(series, moving_average_window))
         if epsilon:
             series = plotting.decimate(series, epsilon)
@@ -59,14 +59,15 @@
     moving_average_window: Optional[int] = None,
     share_y_axis: bool = False,
     logarithmic: bool = False,
     style: Optional[str] = None,
     formatter: Optional[str] = None,
     title: Optional[str] = None,
     no_dots: bool = False,
+    relative_time: bool = False,
     custom_query_file_list: Optional[list] = None,
     custom_value_expr_list: Optional[list] = None,
 ):
     queries = list(_get_queries(
         query_name_list or [],
         custom_query_file_list or [],
         custom_value_expr_list or [],
@@ -97,8 +98,9 @@
         plot_file,
         title=title,
         share_y_axis=share_y_axis,
         logarithmic=logarithmic,
         style=style,
         formatter=formatter,
         no_dots=no_dots,
+        relative_time=relative_time,
     )
```

### Comparing `Procpath-1.6.1/procpath/cmd/query.py` & `Procpath-1.7.0/procpath/cmd/query.py`

 * *Files identical despite different names*

### Comparing `Procpath-1.6.1/procpath/cmd/record.py` & `Procpath-1.7.0/procpath/cmd/record.py`

 * *Files identical despite different names*

### Comparing `Procpath-1.6.1/procpath/cmd/watch.py` & `Procpath-1.7.0/procpath/cmd/watch.py`

 * *Files identical despite different names*

### Comparing `Procpath-1.6.1/procpath/playbook.py` & `Procpath-1.7.0/procpath/playbook.py`

 * *Files identical despite different names*

### Comparing `Procpath-1.6.1/procpath/plotting.py` & `Procpath-1.7.0/procpath/plotting.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import bisect
 import collections
 import itertools
 import math
 import tempfile
+from datetime import datetime
 from functools import partial
-from typing import Iterable, List, Mapping, Optional, Tuple
+from typing import Callable, Iterable, List, Mapping, Optional, Tuple
 
+import pygal.config
 import pygal.formatters
 import pygal.serie
 import pygal.style
 import pygal.util
 
 
-__all__ = 'decimate', 'moving_average', 'plot'
+__all__ = 'Point', 'decimate', 'moving_average', 'plot'
 
 Point = Tuple[float, float]
 
 
 def get_line_distance(p0: Point, p1: Point, p2: Point) -> float:
     """
     Return the distance from p0 to the line formed by p1 and p2.
@@ -92,14 +94,17 @@
 class CompactXLabelDateTimeLine(pygal.DateTimeLine):  # type: ignore[module-attr]
 
     def _compute_x_labels(self):
         """Override to make compact X labels -- no repetition of dates."""
 
         super()._compute_x_labels()
 
+        if self.relative_time:
+            return
+
         last_date_str = None
         for i, (ts_str, ts) in enumerate(self._x_labels):
             if last_date_str == ts_str[:10]:
                 self._x_labels[i] = ts_str[11:], ts
 
             last_date_str = ts_str[:10]
 
@@ -184,25 +189,73 @@
 
         super().line(serie, rescale)
 
         view_points = self._get_x_label_view_points(serie, rescale)
         self._draw_x_label_dots(serie, view_points)
 
 
+class PlottingConfig(pygal.config.Config):
+    """The Pygal way to add custom attribute on a Graph instance."""
+
+    relative_time = pygal.config.Key(False, bool, 'Value', 'Display X axis as timedeltas')
+
+
+def format_x_value_absolute(v: Optional[datetime]) -> str:
+    s = v.isoformat() if v is not None else ''
+    s = s.rstrip('0') if '.' in s else s
+    return s
+
+
+def format_x_value_relative(start: datetime, v: Optional[datetime]) -> str:
+    delta = str(v - start) if v is not None else ''
+    delta = delta.rstrip('0') if '.' in delta else delta
+    return delta
+
+
+def get_x_value_formatter(
+    pid_series_list: List[Mapping[int, List[Point]]], config: pygal.config.Config
+) -> Callable[[Optional[datetime]], str]:
+    if not config.relative_time:
+        return format_x_value_absolute
+
+    # Points are expected to be ordered in each serie so it sufficient
+    # to take the first and the last
+    x_min = min(
+        min(points[0][0] for points in pid_series.values())
+        for pid_series in pid_series_list
+    )
+    x_max = max(
+        max(points[-1][0] for points in pid_series.values())
+        for pid_series in pid_series_list
+    )
+    # Use PyGal's X scale for the first timedelta tick to be exactly 0
+    x_scale: List[float] = pygal.util.compute_scale(
+        x_min,
+        x_max,
+        config.logarithmic,
+        config.order_min,
+        config.min_scale,
+        config.max_scale,
+    )
+    start = datetime.utcfromtimestamp(x_scale[0])
+    return partial(format_x_value_relative, start)
+
+
 def plot(
     pid_series_list: List[Mapping[int, List[Point]]],
     queries: list,
     plot_file: str,
     *,
     title: Optional[str] = None,
     style: Optional[str] = None,
     formatter: Optional[str] = None,
     share_y_axis: bool = False,
     logarithmic: bool = False,
     no_dots: bool = False,
+    relative_time: bool = False,
 ):
     assert pid_series_list and len(pid_series_list) == len(queries), 'Series must match queries'
     assert share_y_axis or len(pid_series_list) <= 2, 'Only one Y axis allowed with share_y_axis'
 
     if not title:
         if share_y_axis:
             title = '; '.join(f'{i}. {q.title}' for i, q in enumerate(queries, start=1))
@@ -223,14 +276,19 @@
             logarithmic=logarithmic,
             x_label_rotation=35,
             title=title,
             value_formatter=getattr(pygal.formatters, formatter or 'human_readable'),
             style=getattr(pygal.style, style or 'DefaultStyle'),
             no_prefix=True,
             js=[f'file://{f.name}'],  # embed "svg/ui.py" converted to JavaScript
+            config=PlottingConfig,
+            relative_time=relative_time,
+        )
+        datetimeline.config.x_value_formatter = get_x_value_formatter(
+            pid_series_list, datetimeline.config
         )
         datetimeline.config.css.append(f'inline:{_ui_css}')
         datetimeline.config.style.tooltip_font_size = 11
 
         for i, (query, pid_series) in enumerate(zip(queries, pid_series_list)):
             for pid, points in pid_series.items():
                 datetimeline.add(
```

### Comparing `Procpath-1.6.1/procpath/procfile.py` & `Procpath-1.7.0/procpath/procfile.py`

 * *Files identical despite different names*

### Comparing `Procpath-1.6.1/procpath/procrec.py` & `Procpath-1.7.0/procpath/procrec.py`

 * *Files identical despite different names*

### Comparing `Procpath-1.6.1/procpath/procret.py` & `Procpath-1.7.0/procpath/procret.py`

 * *Files identical despite different names*

### Comparing `Procpath-1.6.1/procpath/proctree.py` & `Procpath-1.7.0/procpath/proctree.py`

 * *Files identical despite different names*

### Comparing `Procpath-1.6.1/procpath/test.py` & `Procpath-1.7.0/procpath/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import asyncio
 import configparser
 import contextlib
-import datetime
 import functools
 import io
 import json
 import math
 import multiprocessing
 import os
 import re
@@ -15,14 +14,15 @@
 import sys
 import tempfile
 import textwrap
 import time
 import unittest
 import urllib.request
 import zipfile
+from datetime import date, datetime, timezone
 from unittest import mock
 
 import jsonpyth
 
 from . import cli, playbook, plotting, procfile, procrec, procret, proctree, utility
 from .cmd import CommandError, explore, play, plot, query, record, watch
 
@@ -36,30 +36,34 @@
 class TestUtility(unittest.TestCase):
 
     def test_evaluate(self):
         actual = utility.evaluate([
             ('A', 'date -I'),
             ('B', 'echo 42')
         ])
-        self.assertEqual({'A': datetime.date.today().isoformat(), 'B': '42'}, actual)
+        self.assertEqual({'A': date.today().isoformat(), 'B': '42'}, actual)
 
     def test_get_meta(self):
         self.assertEqual(
             {
                 'platform_node',
                 'platform_platform',
                 'page_size',
                 'clock_ticks',
                 'cpu_count',
                 'physical_pages',
                 'procfile_list',
+                'procpath_version',
             },
             utility.get_meta(['stat']).keys(),
         )
 
+
+class TestPlotting(unittest.TestCase):
+
     def test_get_line_distance(self):
         self.assertEqual(10, plotting.get_line_distance((0, 0), (10, 0), (10, 0)))
         self.assertEqual(10, plotting.get_line_distance((0, 0), (10, 0), (10, 10)))
 
         actual = plotting.get_line_distance((90, 51), (34, 15), (-11, -51))
         self.assertAlmostEqual(25.9886, actual, delta=0.00001)
 
@@ -191,34 +195,125 @@
         self.assertIn(b'2610', svg_bytes)
         self.assertEqual(14, svg_bytes.count(b'<g class="dots">'))
         self.assertGreater(len(svg_bytes), 18000)
 
     def test_plot_compact_x_labels(self):
         pid_series = {
             309: [
-                (datetime.datetime.fromisoformat('2022-07-30T10:41:40.336560'), 0),
-                (datetime.datetime.fromisoformat('2022-07-30T10:43:20.423570'), 1),
-                (datetime.datetime.fromisoformat('2022-07-30T10:45:00.520632'), 2),
-                (datetime.datetime.fromisoformat('2022-07-30T10:50:00.793236'), 3),
-                (datetime.datetime.fromisoformat('2022-07-31T10:41:40.311577'), 4),
-                (datetime.datetime.fromisoformat('2022-07-31T10:41:41.464654'), 5),
+                ('2022-07-30T10:41:40.336560', 0),
+                ('2022-07-30T10:43:20.423570', 1),
+                ('2022-07-30T10:45:00.520632', 2),
+                ('2022-07-30T10:50:00.793236', 3),
+                ('2022-07-31T10:41:40.311577', 4),
+                ('2022-07-31T10:41:41.464654', 5),
             ],
         }
+        pid_series[309] = [
+            (datetime.fromisoformat(dt).replace(tzinfo=timezone.utc).timestamp(), v)
+            for dt, v in pid_series[309]
+        ]
+
         query = procret.Query('SELECT 1', 'Dummy')
         with tempfile.NamedTemporaryFile() as f:
             plotting.plot([pid_series], [query], f.name, title='Visions', no_dots=True)
             svg_bytes = f.read()
 
         self.assertIn(b'<svg', svg_bytes)
         self.assertIn(b'Visions', svg_bytes)
         self.assertIn(b'309', svg_bytes)
         self.assertEqual(1, svg_bytes.count(b'">2022-07-30'))
         self.assertEqual(1, svg_bytes.count(b'">2022-07-31'))
         self.assertGreater(len(svg_bytes), 18000)
 
+    def test_plot_absolute_x_label_formatting(self):
+        pid_series = {
+            309: [
+                ('2022-07-30T10:41:40.322', 0),
+                ('2022-07-30T10:41:40.411', 1),
+                ('2022-07-30T10:41:40.522', 2),
+                ('2022-07-30T10:41:40.611', 3),
+                ('2022-07-30T10:41:40.722', 4),
+            ],
+        }
+        pid_series[309] = [
+            (datetime.fromisoformat(dt).replace(tzinfo=timezone.utc).timestamp(), v)
+            for dt, v in pid_series[309]
+        ]
+
+        query = procret.Query('SELECT 1', 'Dummy')
+        with tempfile.NamedTemporaryFile() as f:
+            plotting.plot([pid_series], [query], f.name, title='Visions', no_dots=True)
+            svg_bytes = f.read()
+
+        self.assertIn(b'<svg', svg_bytes)
+        self.assertIn(b'Visions', svg_bytes)
+        self.assertIn(b'309', svg_bytes)
+        self.assertEqual(0, svg_bytes.count(b'2022-07-30T10:41:40.440000'))
+        self.assertEqual(1, svg_bytes.count(b'2022-07-30T10:41:40.44'))
+        self.assertEqual(0, svg_bytes.count(b'2022-07-30T10:41:40.600000'))
+        self.assertEqual(3, svg_bytes.count(b'2022-07-30T10:41:40.6'))
+
+    def test_plot_relative_x_label_formatting(self):
+        pid_series = {
+            309: [
+                ('2022-07-30T10:41:40.322', 0),
+                ('2022-07-30T10:41:40.411', 1),
+                ('2022-07-30T10:41:40.522', 2),
+                ('2022-07-30T10:41:40.611', 3),
+                ('2022-07-30T10:41:40.722', 4),
+            ],
+        }
+        pid_series[309] = [
+            (datetime.fromisoformat(dt).replace(tzinfo=timezone.utc).timestamp(), v)
+            for dt, v in pid_series[309]
+        ]
+
+        query = procret.Query('SELECT 1', 'Dummy')
+        with tempfile.NamedTemporaryFile() as f:
+            plotting.plot(
+                [pid_series], [query], f.name, title='Visions', no_dots=True, relative_time=True
+            )
+            svg_bytes = f.read()
+
+        self.assertIn(b'<svg', svg_bytes)
+        self.assertIn(b'Visions', svg_bytes)
+        self.assertIn(b'309', svg_bytes)
+        self.assertEqual(0, svg_bytes.count(b'2022-07-30'))
+        self.assertEqual(2, svg_bytes.count(b'>0:00:00<'))
+        self.assertEqual(2, svg_bytes.count(b'0:00:00.04'))
+        self.assertEqual(2, svg_bytes.count(b'0:00:00.08'))
+        self.assertEqual(2, svg_bytes.count(b'0:00:00.12'))
+        self.assertEqual(2, svg_bytes.count(b'0:00:00.16'))
+        self.assertEqual(2, svg_bytes.count(b'0:00:00.2<'))
+        self.assertEqual(2, svg_bytes.count(b'0:00:00.36'))
+
+    def test_format_x_value_absolute(self):
+        actual = plotting.format_x_value_absolute(datetime(2022, 9, 3, 19, 38, 4))
+        self.assertEqual('2022-09-03T19:38:04', actual)
+        actual = plotting.format_x_value_absolute(datetime(2022, 9, 3, 19, 38, 0, 500000))
+        self.assertEqual('2022-09-03T19:38:00.5', actual)
+        actual = plotting.format_x_value_absolute(datetime(2022, 9, 3, 19, 38, 0, 1000))
+        self.assertEqual('2022-09-03T19:38:00.001', actual)
+        actual = plotting.format_x_value_absolute(datetime(2022, 9, 3, 19, 38, 0))
+        self.assertEqual('2022-09-03T19:38:00', actual)
+
+    def test_format_x_value_relative(self):
+        start = datetime(2022, 7, 30, 10, 41, 40, 322000)
+
+        actual = plotting.format_x_value_relative(start, start)
+        self.assertEqual('0:00:00', actual)
+        actual = plotting.format_x_value_relative(start, datetime(2022, 7, 30, 10, 41, 40, 411000))
+        self.assertEqual('0:00:00.089', actual)
+        actual = plotting.format_x_value_relative(start, datetime(2022, 7, 30, 10, 41, 40, 522000))
+        self.assertEqual('0:00:00.2', actual)
+        actual = plotting.format_x_value_relative(start, datetime(2022, 7, 30, 14, 56, 42))
+        self.assertEqual('4:15:01.678', actual)
+        actual = plotting.format_x_value_relative(start, datetime(2022, 7, 31, 12, 41, 40))
+        self.assertEqual('1 day, 1:59:59.678', actual)
+
 
 class ChromiumTree(proctree.Forest):
 
     proc_map: dict
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -723,25 +818,25 @@
         self.assertEqual(1920, len(rows))
         self.assertEqual({'ts': 1567504800.0, 'pid': 18467, 'value': 208.2265625}, rows[0])
 
     def test_rss_filter_ts(self):
         rows = procret.query(
             self.database_file.name,
             procret.registry['rss'],
-            after=datetime.datetime(2019, 9, 3, 10, 30, tzinfo=datetime.timezone.utc),
-            before=datetime.datetime(2019, 9, 3, 11, 30, tzinfo=datetime.timezone.utc),
+            after=datetime(2019, 9, 3, 10, 30, tzinfo=timezone.utc),
+            before=datetime(2019, 9, 3, 11, 30, tzinfo=timezone.utc),
         )
         self.assertEqual(976, len(rows))
         self.assertEqual({'ts': 1567506600.0, 'pid': 18467, 'value': 208.2265625}, rows[0])
 
         rows = procret.query(
             self.database_file.name,
             procret.registry['rss'],
-            after=datetime.datetime(2019, 9, 3, 12, 30, tzinfo=datetime.timezone.utc),
-            before=datetime.datetime(2019, 9, 3, 13, 30, tzinfo=datetime.timezone.utc),
+            after=datetime(2019, 9, 3, 12, 30, tzinfo=timezone.utc),
+            before=datetime(2019, 9, 3, 13, 30, tzinfo=timezone.utc),
         )
         self.assertEqual([], rows)
 
     def test_rss_filter_pid(self):
         rows = procret.query(
             self.database_file.name,
             procret.registry['rss'],
@@ -806,25 +901,25 @@
         )
 
     @unittest.skipUnless(apsw or sqlite3.sqlite_version_info >= (3, 25), 'sqlite3 is too old')
     def test_cpu_filter_ts(self):
         rows = procret.query(
             self.database_file.name,
             procret.registry['cpu'],
-            after=datetime.datetime(2019, 9, 3, 10, 30, tzinfo=datetime.timezone.utc),
-            before=datetime.datetime(2019, 9, 3, 11, 30, tzinfo=datetime.timezone.utc),
+            after=datetime(2019, 9, 3, 10, 30, tzinfo=timezone.utc),
+            before=datetime(2019, 9, 3, 11, 30, tzinfo=timezone.utc),
         )
         self.assertEqual(976, len(rows))
         self.assertEqual({'pid': 18467, 'ts': 1567506600.0, 'value': 0.125}, rows[0])
 
         rows = procret.query(
             self.database_file.name,
             procret.registry['cpu'],
-            after=datetime.datetime(2019, 9, 3, 12, 30, tzinfo=datetime.timezone.utc),
-            before=datetime.datetime(2019, 9, 3, 13, 30, tzinfo=datetime.timezone.utc),
+            after=datetime(2019, 9, 3, 12, 30, tzinfo=timezone.utc),
+            before=datetime(2019, 9, 3, 13, 30, tzinfo=timezone.utc),
         )
         self.assertEqual([], rows)
 
     @unittest.skipUnless(apsw or sqlite3.sqlite_version_info >= (3, 25), 'sqlite3 is too old')
     def test_cpu_filter_pid(self):
         rows = procret.query(
             self.database_file.name,
@@ -841,16 +936,16 @@
         self.assertEqual([], rows)
 
     def test_create_query(self):
         query = procret.create_query('260 / 10', title='Custom query')
         rows = procret.query(
             self.database_file.name,
             query,
-            after=datetime.datetime(2019, 9, 3, 10, 30, tzinfo=datetime.timezone.utc),
-            before=datetime.datetime(2019, 9, 3, 11, 30, tzinfo=datetime.timezone.utc),
+            after=datetime(2019, 9, 3, 10, 30, tzinfo=timezone.utc),
+            before=datetime(2019, 9, 3, 11, 30, tzinfo=timezone.utc),
             pid_list=[18508, 18555, 18757],
         )
         self.assertEqual(183, len(rows))
         self.assertEqual({'ts': 1567506600.0, 'pid': 18508, 'value': 26}, rows[0])
         self.assertEqual({'ts': 1567510200.0, 'pid': 18757, 'value': 26}, rows[-1])
 
     def test_query_get_short_query(self):
@@ -1081,14 +1176,15 @@
             'moving_average_window': None,
             'share_y_axis': False,
             'logarithmic': False,
             'style': None,
             'formatter': None,
             'title': None,
             'no_dots': False,
+            'relative_time': False,
             'custom_query_file_list': None,
             'custom_value_expr_list': None,
             'logging_level': 'INFO',
         }
         self.assertEqual(expected, actual)
 
         parser = cli.build_parser()
@@ -1105,14 +1201,15 @@
             'moving_average_window': None,
             'share_y_axis': False,
             'logarithmic': False,
             'style': None,
             'formatter': None,
             'title': None,
             'no_dots': False,
+            'relative_time': False,
             'custom_query_file_list': None,
             'custom_value_expr_list': None,
             'logging_level': 'INFO',
         }
         self.assertEqual(expected, actual)
 
         parser = cli.build_parser()
@@ -1128,14 +1225,15 @@
             '--epsilon', '26.1089',
             '-w', '10',
             '--style', 'LightGreenStyle',
             '--formatter', 'integer',
             '--title', 'Visions',
             '--no-dots',
             '--share-y-axis',
+            '--relative-time',
         ]))
         expected = {
             'command': 'plot',
             'database_file': 'db.sqite',
             'plot_file': 'rss.svg',
             'query_name_list': ['rss', 'cpu'],
             'after': None,
@@ -1145,14 +1243,15 @@
             'moving_average_window': 10,
             'share_y_axis': True,
             'logarithmic': True,
             'style': 'LightGreenStyle',
             'formatter': 'integer',
             'title': 'Visions',
             'no_dots': True,
+            'relative_time': True,
             'custom_query_file_list': None,
             'custom_value_expr_list': None,
             'logging_level': 'WARNING',
         }
         self.assertEqual(expected, actual)
 
         parser = cli.build_parser()
@@ -1166,25 +1265,26 @@
             '--custom-query-file', 'query2.sql',
         ]))
         expected = {
             'command': 'plot',
             'database_file': 'db.sqite',
             'plot_file': 'plot.svg',
             'query_name_list': None,
-            'after': datetime.datetime(2000, 1, 1, 0, 0, tzinfo=datetime.timezone.utc),
-            'before': datetime.datetime(2020, 1, 1, 0, 0, tzinfo=datetime.timezone.utc),
+            'after': datetime(2000, 1, 1, 0, 0, tzinfo=timezone.utc),
+            'before': datetime(2020, 1, 1, 0, 0, tzinfo=timezone.utc),
             'pid_list': None,
             'epsilon': None,
             'moving_average_window': None,
             'share_y_axis': False,
             'logarithmic': False,
             'style': None,
             'formatter': None,
             'title': 'Custom',
             'no_dots': False,
+            'relative_time': False,
             'custom_query_file_list': ['query1.sql', 'query2.sql'],
             'custom_value_expr_list': None,
             'logging_level': 'INFO',
         }
         self.assertEqual(expected, actual)
 
         parser = cli.build_parser()
@@ -1198,25 +1298,26 @@
             '--custom-value-expr', 'stat_minflt / 1000.0',
         ]))
         expected = {
             'command': 'plot',
             'database_file': 'db.sqite',
             'plot_file': 'plot.svg',
             'query_name_list': None,
-            'after': datetime.datetime(2000, 1, 1, 0, 0, tzinfo=datetime.timezone.utc),
-            'before': datetime.datetime(2020, 1, 1, 0, 0, tzinfo=datetime.timezone.utc),
+            'after': datetime(2000, 1, 1, 0, 0, tzinfo=timezone.utc),
+            'before': datetime(2020, 1, 1, 0, 0, tzinfo=timezone.utc),
             'pid_list': None,
             'epsilon': None,
             'moving_average_window': None,
             'share_y_axis': False,
             'logarithmic': False,
             'style': None,
             'formatter': None,
             'title': 'Custom',
             'no_dots': False,
+            'relative_time': False,
             'custom_query_file_list': None,
             'custom_value_expr_list': ['stat_majflt / 1000.0', 'stat_minflt / 1000.0'],
             'logging_level': 'INFO',
         }
         self.assertEqual(expected, actual)
 
     def test_build_parser_watch(self):
@@ -2972,14 +3073,15 @@
             '/fake',
             title='The Strain',
             style=None,
             formatter=None,
             logarithmic=False,
             share_y_axis=False,
             no_dots=False,
+            relative_time=False,
         )
 
     @mock.patch('procpath.plotting.plot')
     def test_plot_custom_query_file(self, plot_mock):
         with tempfile.NamedTemporaryFile() as f:
             sql = '''
                 SELECT 1 ts, 2 pid, 3 value
@@ -3014,14 +3116,15 @@
                 '/fake',
                 style=None,
                 formatter=None,
                 title='RSS vs Custom query',
                 share_y_axis=False,
                 logarithmic=False,
                 no_dots=False,
+                relative_time=False,
             )
 
     @mock.patch('procpath.plotting.plot')
     def test_plot_custom_value_expr(self, plot_mock):
         q1 = procret.create_query('10', 'Custom expression')
         q2 = procret.create_query('stat_minflt / 1000.0', 'Custom expression')
 
@@ -3065,14 +3168,15 @@
             '/fake',
             style=None,
             formatter=None,
             share_y_axis=False,
             logarithmic=False,
             title=None,
             no_dots=False,
+            relative_time=False,
         )
 
     @mock.patch('procpath.plotting.plot')
     def test_plot_rdp_epsilon(self, plot_mock):
         plot.run(
             self.database_file.name,
             '/fake',
@@ -3089,14 +3193,15 @@
             '/fake',
             title=None,
             style=None,
             formatter=None,
             share_y_axis=False,
             logarithmic=False,
             no_dots=False,
+            relative_time=False,
         )
 
     @mock.patch('procpath.plotting.plot')
     def test_plot_moving_average_window(self, plot_mock):
         plot.run(
             self.database_file.name,
             '/fake',
@@ -3114,14 +3219,15 @@
             '/fake',
             title=None,
             style=None,
             formatter=None,
             share_y_axis=False,
             logarithmic=False,
             no_dots=False,
+            relative_time=False,
         )
 
 
 class TestWatchCommand(unittest.TestCase):
 
     forest = None
 
@@ -3385,15 +3491,15 @@
         self.assertEqual('INFO', ctx.records[0].levelname)
         self.assertEqual('№1: Carousel', ctx.records[0].message)
         self.assertEqual('WARNING', ctx.records[1].levelname)
         self.assertEqual('№2: A Glutton for Punishment', ctx.records[1].message)
 
     def test_watch_std_stream_write_after_stop(self):
         with tempfile.NamedTemporaryFile() as f:
-            now = datetime.datetime.now().isoformat()
+            now = datetime.now().isoformat()
             f.write(now.encode())
             f.flush()
 
             with self.assertLogs('procpath', 'INFO') as ctx:
                 watch.run(
                     interval=0.1,
                     repeat=1,
@@ -3573,14 +3679,15 @@
                 moving_average_window=10,
                 pid_list=None,
                 plot_file='rss.svg',
                 query_name_list=['rss'],
                 style=None,
                 title=None,
                 no_dots=False,
+                relative_time=False,
             )
             watch_mock.assert_called_once_with(
                 command_list=[
                     'smemstat -q -o redis-memdiff-$TS.json -p $L1 30 20',
                     (
                         'timeout --foreground --signal SIGINT 600 py-spy record '
                         '--subprocesses --output app-flamegraph-$TS.svg --pid $C1'
@@ -3723,14 +3830,15 @@
             '  "moving_average_window": 10,',
             '  "no_dots": false,',
             '  "pid_list": null,',
             '  "plot_file": "rss.svg",',
             '  "query_name_list": [',
             '    "rss"',
             '  ],',
+            '  "relative_time": false,',
             '  "share_y_axis": false,',
             '  "style": null,',
             '  "title": null',
             '}'
         ], output_file.getvalue().splitlines())
 
     def test_play_negative_flag(self):
@@ -3765,14 +3873,15 @@
                 moving_average_window=None,
                 pid_list=None,
                 plot_file='rss.svg',
                 query_name_list=['cpu'],
                 style=None,
                 title=None,
                 no_dots=False,
+                relative_time=False,
             )
 
         output_file = io.StringIO()
         with tempfile.NamedTemporaryFile('w') as f, mock.patch('procpath.cmd.record.run') as rm:
             with tempfile.NamedTemporaryFile('w') as db_f:
                 f.write(f'''
                     [record]
```

### Comparing `Procpath-1.6.1/procpath/utility.py` & `Procpath-1.7.0/procpath/utility.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import json
 import logging
 import os
 import platform
 import resource
 import subprocess
 
+from . import __version__
+
 
 __all__ = 'evaluate', 'get_meta'
 
 logger = logging.getLogger(__package__)
 
 
 def evaluate(var_cmd_list) -> dict:
@@ -44,8 +46,9 @@
         'platform_node': platform.node(),
         'platform_platform': platform.platform(),
         'page_size': resource.getpagesize(),
         'clock_ticks': os.sysconf('SC_CLK_TCK'),
         'physical_pages': os.sysconf('SC_PHYS_PAGES'),
         'cpu_count': os.cpu_count(),
         'procfile_list': json.dumps(procfile_list),
+        'procpath_version': __version__,
     }
```

### Comparing `Procpath-1.6.1/setup.py` & `Procpath-1.7.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,24 +27,26 @@
         'Topic :: Software Development :: Libraries',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Intended Audience :: Developers',
         'Intended Audience :: System Administrators',
     ],
     entry_points     = {'console_scripts': ['procpath = procpath.cli:main']},
     install_requires = [
         'jsonpyth < 0.2',
         'pygal >= 3, < 4',
     ],
     extras_require = {
         'manual' : [
             'sphinx >= 4, < 5',
             'sphinxcontrib-programoutput < 0.18',
+            'sphinx-copybutton < 0.6',
         ],
     },
 )
```

