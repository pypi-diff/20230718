# Comparing `tmp/docx_charts-0.1.7.tar.gz` & `tmp/docx_charts-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docx_charts-0.1.7.tar", max compression
+gzip compressed data, was "docx_charts-0.1.8.tar", max compression
```

## Comparing `docx_charts-0.1.7.tar` & `docx_charts-0.1.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1075 2023-07-15 15:55:15.811412 docx_charts-0.1.7/LICENSE
--rw-r--r--   0        0        0      490 2023-07-18 19:42:35.683348 docx_charts-0.1.7/README.md
--rw-r--r--   0        0        0       78 2023-07-16 13:44:16.854606 docx_charts-0.1.7/docx_charts/__init__.py
--rw-r--r--   0        0        0     3383 2023-07-18 19:44:04.036353 docx_charts-0.1.7/docx_charts/chart.py
--rw-r--r--   0        0        0     2854 2023-07-18 18:28:29.375111 docx_charts-0.1.7/docx_charts/document.py
--rw-r--r--   0        0        0      485 2023-07-18 19:44:29.247354 docx_charts-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      900 1970-01-01 00:00:00.000000 docx_charts-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-07-15 15:55:15.811412 docx_charts-0.1.8/LICENSE
+-rw-r--r--   0        0        0      490 2023-07-18 19:42:35.683348 docx_charts-0.1.8/README.md
+-rw-r--r--   0        0        0       78 2023-07-16 13:44:16.854606 docx_charts-0.1.8/docx_charts/__init__.py
+-rw-r--r--   0        0        0     3536 2023-07-18 20:06:11.157424 docx_charts-0.1.8/docx_charts/chart.py
+-rw-r--r--   0        0        0     2860 2023-07-18 20:03:48.566416 docx_charts-0.1.8/docx_charts/document.py
+-rw-r--r--   0        0        0      485 2023-07-18 20:07:58.752430 docx_charts-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      900 1970-01-01 00:00:00.000000 docx_charts-0.1.8/PKG-INFO
```

### Comparing `docx_charts-0.1.7/LICENSE` & `docx_charts-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `docx_charts-0.1.7/docx_charts/chart.py` & `docx_charts-0.1.8/docx_charts/chart.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 
 	def data(self) -> ChartData:
 		'''
 		Gets the internal table data the chart is based on.
 
 		Returns:
-			A list of Series dictionaries representing the data for the chart.
+			A dictionary of Series dicts representing data for the chart.
 		'''
 		dom = minidom.parse(self.file)
 		series = {
 			series_name(series) or f'series{i+1}':
 			dict(zip(
 				[cat.firstChild.nodeValue for cat in series.getElementsByTagName('c:cat')[0].getElementsByTagName('c:v')
 					if cat.firstChild and isinstance(cat.firstChild, minidom.Text) and isinstance(cat.firstChild.nodeValue, str)],
@@ -78,32 +78,35 @@
 
 
 	def write(self, data: ChartData) -> None:
 		'''
 		Overwrites the data of the chart.
 
 		Args:
-			data (list[Series]): The data to write to the chart.
+			data (dict[str, dict[str, float]]): The data to write to the chart. The first key is the name of the series, the second key is the name of the category.
 
 		Note:
-			The data must be in the same number of series as the original data.
-			However, unchanged categories may be left out.
+			The names of the series and categories must be the same as in the original data.
+			However, unchanged series and categories may be left out.
 		'''
-		assert len(data) == len(self.data()), 'The new data must have the same number of series as the original data.'
 		dom = minidom.parse(self.file)
 
 		for (new_series_name, new_series) in data.items():
-			series = [series for i, series in enumerate(dom.getElementsByTagName('c:ser')) if (series_name(series) or f'series{i+1}') == new_series_name][0]
+			try:
+				series = [series for i, series in enumerate(dom.getElementsByTagName('c:ser')) if (series_name(series) or f'series{i+1}') == new_series_name][0]
+			except IndexError:
+				raise ValueError(f'Chart {self.name} does not contain a series named {new_series_name}.')
 			cats = [cat.firstChild for cat in series.getElementsByTagName('c:cat')[0].getElementsByTagName('c:v')
 				if cat.firstChild and isinstance(cat.firstChild, minidom.Text)]
 			vals = [val.firstChild for val in series.getElementsByTagName('c:val')[0].getElementsByTagName('c:v')
 				if val.firstChild and isinstance(val.firstChild, minidom.Text)]
 
 			for new_cat, new_val in new_series.items():
-				assert new_cat in [cat.nodeValue for cat in cats], 'The new data must have the same categories as the original data.'
+				if new_cat not in [cat.nodeValue for cat in cats]:
+					raise ValueError(f'Chart {self.name} does not contain a category named {new_cat}.')
 				for cat, val in zip(cats, vals):
 					if cat.nodeValue == new_cat:
 						val.replaceWholeText(str(new_val))
 						break
 
 		self.file.seek(0)
 		self.file.truncate()
```

### Comparing `docx_charts-0.1.7/docx_charts/document.py` & `docx_charts-0.1.8/docx_charts/document.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,21 +77,21 @@
 					relationship = [rel for rel in rels_dom.getElementsByTagName('Relationship') if rel.getAttribute('Id') == relationship_id][0]
 					path = os.path.join(self.extracted.name, 'word', relationship.getAttribute('Target'))
 					name = node.parentNode.parentNode.parentNode.getElementsByTagName('wp:docPr')[0].getAttribute('name')
 					charts.append(Chart(path, name))
 		return charts
 
 
-	def find_charts_by_name(self, name: str) -> list[Chart]:
+	def charts_by_name(self, name: str) -> list[Chart]:
 		'''
 		Finds the charts in the Word document with the specified name.
 
 		Args:
 			name (str): The name of the charts to find.
 
 		Returns:
 			A list of objects representing the charts in the Word document with the specified name.
 
 		Note:
-			Generally this will only return one chart, but it is possible for there to be multiple charts with the same name.
+			Generally this will only return one chart, but technically it's possible for there to be multiple charts with the same name.
 		'''
 		return [chart for chart in self.charts() if chart.name == name]
```

### Comparing `docx_charts-0.1.7/PKG-INFO` & `docx_charts-0.1.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docx-charts
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python library for manipulating chart data in word documents
 Author: Julia van der Kris
 Author-email: julia@juuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuulia.dev
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

