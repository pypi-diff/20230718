# Comparing `tmp/docx_charts-0.1.6.tar.gz` & `tmp/docx_charts-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docx_charts-0.1.6.tar", max compression
+gzip compressed data, was "docx_charts-0.1.7.tar", max compression
```

## Comparing `docx_charts-0.1.6.tar` & `docx_charts-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1075 2023-07-15 15:55:15.811412 docx_charts-0.1.6/LICENSE
--rw-r--r--   0        0        0      247 2023-07-16 14:30:02.509753 docx_charts-0.1.6/README.md
--rw-r--r--   0        0        0       78 2023-07-16 13:44:16.854606 docx_charts-0.1.6/docx_charts/__init__.py
--rw-r--r--   0        0        0     2880 2023-07-16 16:29:12.559205 docx_charts-0.1.6/docx_charts/chart.py
--rw-r--r--   0        0        0     2864 2023-07-16 16:05:17.775128 docx_charts-0.1.6/docx_charts/document.py
--rw-r--r--   0        0        0      485 2023-07-16 16:29:25.738206 docx_charts-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      657 1970-01-01 00:00:00.000000 docx_charts-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-07-15 15:55:15.811412 docx_charts-0.1.7/LICENSE
+-rw-r--r--   0        0        0      490 2023-07-18 19:42:35.683348 docx_charts-0.1.7/README.md
+-rw-r--r--   0        0        0       78 2023-07-16 13:44:16.854606 docx_charts-0.1.7/docx_charts/__init__.py
+-rw-r--r--   0        0        0     3383 2023-07-18 19:44:04.036353 docx_charts-0.1.7/docx_charts/chart.py
+-rw-r--r--   0        0        0     2854 2023-07-18 18:28:29.375111 docx_charts-0.1.7/docx_charts/document.py
+-rw-r--r--   0        0        0      485 2023-07-18 19:44:29.247354 docx_charts-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      900 1970-01-01 00:00:00.000000 docx_charts-0.1.7/PKG-INFO
```

### Comparing `docx_charts-0.1.6/LICENSE` & `docx_charts-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `docx_charts-0.1.6/docx_charts/chart.py` & `docx_charts-0.1.7/docx_charts/chart.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 import io
 from xml.dom import minidom
 
 
-Series = dict[str, float]
+Series = dict[str, float]  # category: value
+ChartData = dict[str, Series]  # series_name: Series
+
+
+def series_name(series: minidom.Element) -> str | None:
+	if not series.getElementsByTagName('c:tx'):
+		return None
+	return series.getElementsByTagName('c:tx')[0].getElementsByTagName('c:v')[0].firstChild.nodeValue.lower().replace(' ', '_')  # type: ignore
 
 
 class Chart:
 	'''
 	Represents a chart in a Word document.
 
 	Attributes:
@@ -44,49 +51,52 @@
 			A string representation of the Chart object.
 		'''
 		return f'{self.name} ({self.file.name})'
 
 	__repr__ = __str__
 
 
-	def data(self) -> list[Series]:
+	def data(self) -> ChartData:
 		'''
 		Gets the internal table data the chart is based on.
 
 		Returns:
 			A list of Series dictionaries representing the data for the chart.
 		'''
 		dom = minidom.parse(self.file)
-		series = [
+		series = {
+			series_name(series) or f'series{i+1}':
 			dict(zip(
 				[cat.firstChild.nodeValue for cat in series.getElementsByTagName('c:cat')[0].getElementsByTagName('c:v')
 					if cat.firstChild and isinstance(cat.firstChild, minidom.Text) and isinstance(cat.firstChild.nodeValue, str)],
 				[float(val.firstChild.nodeValue) for val in series.getElementsByTagName('c:val')[0].getElementsByTagName('c:v')
 					if val.firstChild and isinstance(val.firstChild, minidom.Text)]
 			))
-			for series in dom.getElementsByTagName('c:ser')
-		]
+			for i, series in enumerate(dom.getElementsByTagName('c:ser'))
+		}
 		self.file.seek(0)
 		return series
 
 
-	def write_data(self, data: list[Series]) -> None:
+	def write(self, data: ChartData) -> None:
 		'''
 		Overwrites the data of the chart.
 
 		Args:
 			data (list[Series]): The data to write to the chart.
 
 		Note:
 			The data must be in the same number of series as the original data.
 			However, unchanged categories may be left out.
 		'''
 		assert len(data) == len(self.data()), 'The new data must have the same number of series as the original data.'
 		dom = minidom.parse(self.file)
-		for series, new_series in zip(dom.getElementsByTagName('c:ser'), data):
+
+		for (new_series_name, new_series) in data.items():
+			series = [series for i, series in enumerate(dom.getElementsByTagName('c:ser')) if (series_name(series) or f'series{i+1}') == new_series_name][0]
 			cats = [cat.firstChild for cat in series.getElementsByTagName('c:cat')[0].getElementsByTagName('c:v')
 				if cat.firstChild and isinstance(cat.firstChild, minidom.Text)]
 			vals = [val.firstChild for val in series.getElementsByTagName('c:val')[0].getElementsByTagName('c:v')
 				if val.firstChild and isinstance(val.firstChild, minidom.Text)]
 
 			for new_cat, new_val in new_series.items():
 				assert new_cat in [cat.nodeValue for cat in cats], 'The new data must have the same categories as the original data.'
```

### Comparing `docx_charts-0.1.6/docx_charts/document.py` & `docx_charts-0.1.7/docx_charts/document.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 		Returns:
 			A list of files in the root of the extracted archive
 		'''
 		return os.listdir(self.extracted.name)
 
 
-	def list_charts(self) -> list[Chart]:
+	def charts(self) -> list[Chart]:
 		'''
 		Lists the charts in the Word document.
 
 		Returns:
 			A list of objects representing the charts in the Word document.
 		'''
 		charts: list[Chart] = []
@@ -90,8 +90,8 @@
 
 		Returns:
 			A list of objects representing the charts in the Word document with the specified name.
 
 		Note:
 			Generally this will only return one chart, but it is possible for there to be multiple charts with the same name.
 		'''
-		return [chart for chart in self.list_charts() if chart.name == name]
+		return [chart for chart in self.charts() if chart.name == name]
```

### Comparing `docx_charts-0.1.6/PKG-INFO` & `docx_charts-0.1.7/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,31 @@
 Metadata-Version: 2.1
 Name: docx-charts
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python library for manipulating chart data in word documents
 Author: Julia van der Kris
 Author-email: julia@juuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuulia.dev
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # docx-charts
 
 Python library for manipulating chart data in word documents
 
 Disclaimer: this is a project made for a very specific usecase, because nothing better existed yet. No stability guarantees are made, and the API is subject to change :)
 
+&nbsp;
+
+# Example
+```py
+from docx_charts import Document
+
+doc = Document('example.docx')
+chart = doc.find_charts_by_name('Chart 1')[0]
+data = chart.data()
+data['student_total']['CTB1002 Linear Algebra'] = 0.6
+chart.write(data)
+doc.save()
+```
+
```

