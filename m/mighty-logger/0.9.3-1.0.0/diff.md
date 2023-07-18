# Comparing `tmp/mighty_logger-0.9.3.tar.gz` & `tmp/mighty_logger-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mighty_logger-0.9.3.tar", last modified: Wed Jul 12 09:58:22 2023, max compression
+gzip compressed data, was "mighty_logger-1.0.0.tar", last modified: Tue Jul 18 15:22:49 2023, max compression
```

## Comparing `mighty_logger-0.9.3.tar` & `mighty_logger-1.0.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 09:58:22.763353 mighty_logger-0.9.3/
--rw-rw-rw-   0        0        0    11357 2023-04-10 16:24:05.000000 mighty_logger-0.9.3/LICENSE
--rw-rw-rw-   0        0        0     9902 2023-07-12 09:58:22.764353 mighty_logger-0.9.3/PKG-INFO
--rw-rw-rw-   0        0        0     8973 2023-07-12 09:39:43.000000 mighty_logger-0.9.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 09:58:22.678766 mighty_logger-0.9.3/mighty_logger/
--rw-rw-rw-   0        0        0      861 2023-07-04 16:28:33.000000 mighty_logger-0.9.3/mighty_logger/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 09:58:22.735628 mighty_logger-0.9.3/mighty_logger/basic/
--rw-rw-rw-   0        0        0      836 2023-07-04 16:29:00.000000 mighty_logger-0.9.3/mighty_logger/basic/__init__.py
--rw-rw-rw-   0        0        0     7576 2023-07-04 17:04:11.000000 mighty_logger-0.9.3/mighty_logger/basic/basic_logger.py
--rw-rw-rw-   0        0        0     1370 2023-07-02 15:20:50.000000 mighty_logger-0.9.3/mighty_logger/basic/exceptions.py
--rw-rw-rw-   0        0        0     2607 2023-07-04 14:49:44.000000 mighty_logger-0.9.3/mighty_logger/basic/exporter.py
-drwxrwxrwx   0        0        0        0 2023-07-12 09:58:22.754351 mighty_logger-0.9.3/mighty_logger/basic/lib_types/
--rw-rw-rw-   0        0        0      934 2023-07-02 15:05:20.000000 mighty_logger-0.9.3/mighty_logger/basic/lib_types/__init__.py
--rw-rw-rw-   0        0        0      912 2023-07-02 15:18:08.000000 mighty_logger-0.9.3/mighty_logger/basic/lib_types/animation_type.py
--rw-rw-rw-   0        0        0     1798 2023-07-02 15:18:23.000000 mighty_logger-0.9.3/mighty_logger/basic/lib_types/entry_type.py
--rw-rw-rw-   0        0        0     1290 2023-07-02 15:20:29.000000 mighty_logger-0.9.3/mighty_logger/basic/lib_types/environment_type.py
--rw-rw-rw-   0        0        0      797 2023-07-02 15:20:29.000000 mighty_logger-0.9.3/mighty_logger/basic/lib_types/sorting_key_type.py
--rw-rw-rw-   0        0        0     2623 2023-07-04 17:40:06.000000 mighty_logger-0.9.3/mighty_logger/basic/lib_types/text_buffer_type.py
--rw-rw-rw-   0        0        0     7018 2023-07-04 14:49:44.000000 mighty_logger-0.9.3/mighty_logger/basic/modifier.py
--rw-rw-rw-   0        0        0      757 2023-07-02 15:22:45.000000 mighty_logger-0.9.3/mighty_logger/basic/singleton.py
--rw-rw-rw-   0        0        0     9274 2023-07-04 16:52:30.000000 mighty_logger-0.9.3/mighty_logger/basic/text_buffer.py
--rw-rw-rw-   0        0        0    19889 2023-07-11 17:36:31.000000 mighty_logger-0.9.3/mighty_logger/mighty_logger.py
--rw-rw-rw-   0        0        0     5994 2023-07-09 10:51:28.000000 mighty_logger-0.9.3/mighty_logger/simple_logger.py
-drwxrwxrwx   0        0        0        0 2023-07-12 09:58:22.762354 mighty_logger-0.9.3/mighty_logger/src/
--rw-rw-rw-   0        0        0     1081 2023-07-04 14:45:31.000000 mighty_logger-0.9.3/mighty_logger/src/__init__.py
--rw-rw-rw-   0        0        0     9825 2023-07-02 15:30:09.000000 mighty_logger-0.9.3/mighty_logger/src/animations.py
--rw-rw-rw-   0        0        0     3541 2023-07-02 15:30:09.000000 mighty_logger-0.9.3/mighty_logger/src/ansi_format.py
--rw-rw-rw-   0        0        0     6656 2023-07-02 15:30:09.000000 mighty_logger-0.9.3/mighty_logger/src/color_picker.py
--rw-rw-rw-   0        0        0    36171 2023-07-02 15:24:11.000000 mighty_logger-0.9.3/mighty_logger/src/entry_types.py
--rw-rw-rw-   0        0        0      968 2023-07-02 15:24:25.000000 mighty_logger-0.9.3/mighty_logger/src/environments.py
--rw-rw-rw-   0        0        0      901 2023-07-02 15:24:25.000000 mighty_logger-0.9.3/mighty_logger/src/sorting_keys.py
-drwxrwxrwx   0        0        0        0 2023-07-12 09:58:22.689378 mighty_logger-0.9.3/mighty_logger.egg-info/
--rw-rw-rw-   0        0        0     9902 2023-07-12 09:58:22.000000 mighty_logger-0.9.3/mighty_logger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1026 2023-07-12 09:58:22.000000 mighty_logger-0.9.3/mighty_logger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 09:58:22.000000 mighty_logger-0.9.3/mighty_logger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-12 09:58:22.000000 mighty_logger-0.9.3/mighty_logger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1823 2023-07-04 14:50:52.000000 mighty_logger-0.9.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-12 09:58:22.765354 mighty_logger-0.9.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-18 15:22:49.247042 mighty_logger-1.0.0/
+-rw-rw-rw-   0        0        0    11357 2023-04-10 16:24:05.000000 mighty_logger-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     9915 2023-07-18 15:22:49.247042 mighty_logger-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8973 2023-07-18 14:54:46.000000 mighty_logger-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 15:22:49.115263 mighty_logger-1.0.0/mighty_logger/
+-rw-rw-rw-   0        0        0      861 2023-07-18 14:42:23.000000 mighty_logger-1.0.0/mighty_logger/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 15:22:49.186278 mighty_logger-1.0.0/mighty_logger/basic/
+-rw-rw-rw-   0        0        0      836 2023-07-04 16:29:00.000000 mighty_logger-1.0.0/mighty_logger/basic/__init__.py
+-rw-rw-rw-   0        0        0     7576 2023-07-04 17:04:11.000000 mighty_logger-1.0.0/mighty_logger/basic/basic_logger.py
+-rw-rw-rw-   0        0        0     1370 2023-07-02 15:20:50.000000 mighty_logger-1.0.0/mighty_logger/basic/exceptions.py
+-rw-rw-rw-   0        0        0     2649 2023-07-17 17:55:08.000000 mighty_logger-1.0.0/mighty_logger/basic/exporter.py
+drwxrwxrwx   0        0        0        0 2023-07-18 15:22:49.213875 mighty_logger-1.0.0/mighty_logger/basic/lib_types/
+-rw-rw-rw-   0        0        0      934 2023-07-02 15:05:20.000000 mighty_logger-1.0.0/mighty_logger/basic/lib_types/__init__.py
+-rw-rw-rw-   0        0        0      912 2023-07-02 15:18:08.000000 mighty_logger-1.0.0/mighty_logger/basic/lib_types/animation_type.py
+-rw-rw-rw-   0        0        0     1798 2023-07-02 15:18:23.000000 mighty_logger-1.0.0/mighty_logger/basic/lib_types/entry_type.py
+-rw-rw-rw-   0        0        0     1290 2023-07-02 15:20:29.000000 mighty_logger-1.0.0/mighty_logger/basic/lib_types/environment_type.py
+-rw-rw-rw-   0        0        0      797 2023-07-02 15:20:29.000000 mighty_logger-1.0.0/mighty_logger/basic/lib_types/sorting_key_type.py
+-rw-rw-rw-   0        0        0     2747 2023-07-17 14:23:23.000000 mighty_logger-1.0.0/mighty_logger/basic/lib_types/text_buffer_type.py
+-rw-rw-rw-   0        0        0     6242 2023-07-18 13:14:12.000000 mighty_logger-1.0.0/mighty_logger/basic/modifier.py
+-rw-rw-rw-   0        0        0      757 2023-07-02 15:22:45.000000 mighty_logger-1.0.0/mighty_logger/basic/singleton.py
+-rw-rw-rw-   0        0        0     9524 2023-07-17 15:24:51.000000 mighty_logger-1.0.0/mighty_logger/basic/text_buffer.py
+-rw-rw-rw-   0        0        0    19892 2023-07-17 18:08:37.000000 mighty_logger-1.0.0/mighty_logger/mighty_logger.py
+-rw-rw-rw-   0        0        0     5992 2023-07-17 18:28:30.000000 mighty_logger-1.0.0/mighty_logger/simple_logger.py
+drwxrwxrwx   0        0        0        0 2023-07-18 15:22:49.244986 mighty_logger-1.0.0/mighty_logger/src/
+-rw-rw-rw-   0        0        0     1103 2023-07-18 13:17:33.000000 mighty_logger-1.0.0/mighty_logger/src/__init__.py
+-rw-rw-rw-   0        0        0     9692 2023-07-17 17:26:43.000000 mighty_logger-1.0.0/mighty_logger/src/animations.py
+-rw-rw-rw-   0        0        0     3541 2023-07-02 15:30:09.000000 mighty_logger-1.0.0/mighty_logger/src/ansi_format.py
+-rw-rw-rw-   0        0        0     6656 2023-07-02 15:30:09.000000 mighty_logger-1.0.0/mighty_logger/src/color_picker.py
+-rw-rw-rw-   0        0        0    44708 2023-07-18 13:14:12.000000 mighty_logger-1.0.0/mighty_logger/src/entry_types.py
+-rw-rw-rw-   0        0        0      968 2023-07-02 15:24:25.000000 mighty_logger-1.0.0/mighty_logger/src/environments.py
+-rw-rw-rw-   0        0        0      901 2023-07-02 15:24:25.000000 mighty_logger-1.0.0/mighty_logger/src/sorting_keys.py
+drwxrwxrwx   0        0        0        0 2023-07-18 15:22:49.128265 mighty_logger-1.0.0/mighty_logger.egg-info/
+-rw-rw-rw-   0        0        0     9915 2023-07-18 15:22:49.000000 mighty_logger-1.0.0/mighty_logger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1026 2023-07-18 15:22:49.000000 mighty_logger-1.0.0/mighty_logger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 15:22:49.000000 mighty_logger-1.0.0/mighty_logger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-18 15:22:49.000000 mighty_logger-1.0.0/mighty_logger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1836 2023-07-18 14:55:17.000000 mighty_logger-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-18 15:22:49.248042 mighty_logger-1.0.0/setup.cfg
```

### Comparing `mighty_logger-0.9.3/LICENSE` & `mighty_logger-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.9.3/PKG-INFO` & `mighty_logger-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: mighty_logger
-Version: 0.9.3
+Version: 1.0.0
 Summary: Mighty functional logger
 Author-email: Kalynovsky 'Nakamura Akira' Valentin <nakama3942@gmail.com>
 License: Apache License Version 2.0
 Project-URL: Repository, https://github.com/Nakama3942/mighty_logger
 Project-URL: Releases, https://github.com/Nakama3942/mighty_logger/releases
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Logging
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
@@ -122,15 +122,15 @@
 - [x] v0.7.1 - Modding update (buffer modification added - sorting, searching and selecting)
 - [x] v0.7.2 - Categories update (separated the entry category from the type)
 - [x] v0.8.0 - Export update (added conversion to csv)
 - [x] v0.9.0 - Extension update (made wheel format and instruction of toml)
 - [x] v0.9.1 - Documenting update (documented library)
 - [x] v0.9.2 - Feature update (made optimizations)
 - [x] v0.9.3 - Web docs update (added generation of web docs)
-- [ ] v1.0.0 - Completion of logger development (logger development completed)
+- [x] v1.0.0 - Completion of logger development (logger development completed)
 - [ ] v1.1.0 - Font update (added a class that formats text outside the logger)
 
 </details>
 
 - [Content](#content)
 
 ## Features
```

### Comparing `mighty_logger-0.9.3/README.md` & `mighty_logger-1.0.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 - [x] v0.7.1 - Modding update (buffer modification added - sorting, searching and selecting)
 - [x] v0.7.2 - Categories update (separated the entry category from the type)
 - [x] v0.8.0 - Export update (added conversion to csv)
 - [x] v0.9.0 - Extension update (made wheel format and instruction of toml)
 - [x] v0.9.1 - Documenting update (documented library)
 - [x] v0.9.2 - Feature update (made optimizations)
 - [x] v0.9.3 - Web docs update (added generation of web docs)
-- [ ] v1.0.0 - Completion of logger development (logger development completed)
+- [x] v1.0.0 - Completion of logger development (logger development completed)
 - [ ] v1.1.0 - Font update (added a class that formats text outside the logger)
 
 </details>
 
 - [Content](#content)
 
 ## Features
```

### Comparing `mighty_logger-0.9.3/mighty_logger/__init__.py` & `mighty_logger-1.0.0/mighty_logger/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,9 +16,9 @@
 limitations under the License.
 """
 
 from .mighty_logger import MightyLogger
 from .simple_logger import Logger
 
 __authot__ = "Kalynovsky 'Nakamura Akira' Valentin"
-__version__ = "0.9.3"
+__version__ = "1.0.0"
 __email__ = "nakama3942@gmail.com"
```

### Comparing `mighty_logger-0.9.3/mighty_logger/basic/__init__.py` & `mighty_logger-1.0.0/mighty_logger/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.9.3/mighty_logger/basic/basic_logger.py` & `mighty_logger-1.0.0/mighty_logger/basic/basic_logger.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.9.3/mighty_logger/basic/exceptions.py` & `mighty_logger-1.0.0/mighty_logger/basic/exceptions.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.9.3/mighty_logger/basic/exporter.py` & `mighty_logger-1.0.0/mighty_logger/basic/exporter.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,30 +29,32 @@
 		self.__env: EnvironmentType = environment
 		self.__csv: list[dict] = []
 
 	@property
 	def entries(self) -> list[str]:
 		return self.__entries
 
+	def _clearing_entry(self, dirty_entry: str) -> str:
+		match self.__env.environment_name:
+			case LogEnvironments.CONSOLE.environment_name:
+				return sub(r"\033\[.*?m", "", dirty_entry)
+			case LogEnvironments.PLAIN_CONSOLE.environment_name:
+				return dirty_entry
+			case LogEnvironments.HTML.environment_name:
+				return sub(r"<.*?>", "", dirty_entry)
+			case LogEnvironments.MARKDOWN.environment_name:
+				return sub(r"<.*?>", "", dirty_entry)
+			case LogEnvironments.PLAIN.environment_name:
+				return dirty_entry
+
 	def export_to_csv(self) -> None:
-		cleared_entry = ""
 		csv_entry = {}
 
 		for entry in self.__entries[1:]:
-			match self.__env.environment_name:
-				case LogEnvironments.CONSOLE.environment_name:
-					cleared_entry = sub(r"\033\[.*?m", "", entry)
-				case LogEnvironments.PLAIN_CONSOLE.environment_name:
-					cleared_entry = entry
-				case LogEnvironments.HTML.environment_name:
-					cleared_entry = sub(r"<.*?>", "", entry)
-				case LogEnvironments.MARKDOWN.environment_name:
-					cleared_entry = sub(r"<.*?>", "", entry)
-				case LogEnvironments.PLAIN.environment_name:
-					cleared_entry = entry
+			cleared_entry = self._clearing_entry(entry)
 			if cleared_entry.startswith("-?"):
 				parts = cleared_entry.split("*")
 				entry_data = parts[1].split()
 
 				csv_entry["Icon"] = entry_data[2]
 				try:
 					csv_entry["Duration"] = parts[0].split()[1]
@@ -61,15 +63,14 @@
 				csv_entry["Time"] = " ".join(entry_data[0:2])
 				csv_entry["Category"] = entry_data[4][0]
 				csv_entry["Type"] = entry_data[4][1:]
 				csv_entry["Message"] = " ".join(entry_data[6:])
 
 				self.__csv.append(csv_entry.copy())
 				csv_entry.clear()
-				continue
 
 	def save_to_csv(self, file_name: str) -> None:
 		with open(f"{file_name}.csv", "w", encoding="utf-8") as csv:
 			# Write headers (first line) to file
 			headers = self.__csv[0].keys()
 			csv.write(",".join(headers) + "\n")
```

### Comparing `mighty_logger-0.9.3/mighty_logger/basic/lib_types/__init__.py` & `mighty_logger-1.0.0/mighty_logger/basic/lib_types/__init__.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.9.3/mighty_logger/basic/lib_types/animation_type.py` & `mighty_logger-1.0.0/mighty_logger/basic/lib_types/animation_type.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.9.3/mighty_logger/basic/lib_types/entry_type.py` & `mighty_logger-1.0.0/mighty_logger/basic/lib_types/entry_type.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.9.3/mighty_logger/basic/lib_types/environment_type.py` & `mighty_logger-1.0.0/mighty_logger/basic/lib_types/environment_type.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.9.3/mighty_logger/basic/lib_types/sorting_key_type.py` & `mighty_logger-1.0.0/mighty_logger/basic/lib_types/sorting_key_type.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.9.3/mighty_logger/basic/lib_types/text_buffer_type.py` & `mighty_logger-1.0.0/mighty_logger/basic/lib_types/text_buffer_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,7 +65,10 @@
 		raise NotImplementedError("Method input() is not implemented in the base class")
 
 	def update_console(self) -> None:
 		raise NotImplementedError("Method update_console() is not implemented in the base class")
 
 	def update_entry(self) -> None:
 		raise NotImplementedError("Method update_entry() is not implemented in the base class")
+
+	def output_entry(self) -> None:
+		raise NotImplementedError("Method output_entry() is not implemented in the base class")
```

### Comparing `mighty_logger-0.9.3/mighty_logger/basic/singleton.py` & `mighty_logger-1.0.0/mighty_logger/basic/singleton.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.9.3/mighty_logger/basic/text_buffer.py` & `mighty_logger-1.0.0/mighty_logger/basic/text_buffer.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,14 +112,17 @@
 
 	def update_console(self) -> None:
 		super().update_console()
 
 	def update_entry(self) -> None:
 		super().update_console()
 
+	def output_entry(self) -> None:
+		super().output_entry()
+
 class TextBuffer(Singleton, TextBufferType):
 	def __init__(self, env: EnvironmentType, console_width: int = 60) -> None:
 		if not hasattr(self, "_text_buffer"):
 			if env.environment_name in [
 				LogEnvironments.HTML.environment_name,
 				LogEnvironments.MARKDOWN.environment_name,
 				LogEnvironments.PLAIN.environment_name
@@ -227,7 +230,14 @@
 		stdout.flush()
 		self._cursor_string = self._buffer_size - 1
 
 	def update_entry(self) -> None:
 		stdout.write(f'\r')
 		stdout.write(self._text_buffer[-1])
 		stdout.flush()
+
+	def output_entry(self) -> None:
+		if len(self._text_buffer) > 1:
+			stdout.write(f'\n')
+		stdout.write(self._text_buffer[-1])
+		stdout.flush()
+		self._cursor_string = self._buffer_size - 1
```

### Comparing `mighty_logger-0.9.3/mighty_logger/mighty_logger.py` & `mighty_logger-1.0.0/mighty_logger/mighty_logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,33 +148,33 @@
 	#                                    Inputter of Logger                                    #
 	#                                                                                          #
 	# ######################################################################################## #
 
 	def empty(self, entry: str) -> None:
 		self._buffer.append(entry)
 		if self._environment.updatable:
-			self._buffer.update_console()
+			self._buffer.output_entry()
 
 	def addy(self, number_string: int, message: str) -> None:
 		self._buffer.insert(number_string, message)
 		if self._environment.updatable:
 			self._buffer.update_console()
 
 	def modify(self, number_string: int, message: str) -> None:
 		self._buffer.replace(number_string, message)
 		if self._environment.updatable:
 			self._buffer.update_console()
 
-	def catchy(self, number_string: int) -> str:
+	def catchy(self, number_string: int = -1) -> str:
 		data = self._buffer.pop(number_string)
 		if self._environment.updatable:
 			self._buffer.update_console()
 		return data
 
-	def extractly(self, number_string: int) -> None:
+	def extractly(self, number_string: int = -1) -> None:
 		self._buffer.remove(number_string)
 		if self._environment.updatable:
 			self._buffer.update_console()
 
 	def clearly(self) -> None:
 		self._buffer.clear()
 		if self._environment.updatable:
@@ -405,20 +405,20 @@
 		if self._environment.updatable:
 			self._buffer.update_console()
 		while not self._progress_interrupt:
 			if old_progress_rise == self._progress_rise:
 				continue
 			else:
 				old_progress_rise = self._progress_rise
-				animation_item = f"{self._animation.animation[(self._progress_rise // 15) + (2 if self._progress_rise == 100 else 1)]} - {self._progress_rise} %"
+				animation_item = f"{self._animation.animation[(self._progress_rise // 15) + (2 if self._progress_rise == 100 else 1)]}"
 				self._buffer.text_buffer[-1] = self._assemble_entry(
 					ServiceProcessEntryTypes.process,
 					self._icon_set,
 					animation_item,
-					message_text,
+					f"{message_text} - {self._progress_rise} %",
 					local_settings
 				)
 				if self._environment.updatable:
 					self._buffer.update_entry()
 			sleep(0.1)
 		if self._environment.updatable:
 			self._buffer.update_console()
@@ -429,15 +429,15 @@
 	def note_process(
 		self,
 		entry_type: EntryType,
 		message_text: str,
 		local_settings: dict = None
 	) -> None:
 		sleep(0.001)
-		last = self._buffer.pop()
+		last = self.catchy()
 
 		progress_stop = datetime.now()
 		self._progress_time = "&" + str(progress_stop - self._progress_start).split(".")[0]
 		args = {'message_text': message_text}
 		if local_settings is not None:
 			args['local_settings'] = local_settings
 		self.entry(entry_type, **args)
@@ -447,15 +447,15 @@
 	def stop_process(
 		self,
 		message_text: str,
 		local_settings: dict = None
 	) -> None:
 		self._progress_interrupt = True
 		sleep(0.11)
-		self._buffer.remove()
+		self.extractly()
 
 		progress_stop = datetime.now()
 		self._progress_time = "&" + str(progress_stop - self._progress_start).split(".")[0]
 		args = {'message_text': message_text}
 		if local_settings is not None:
 			args['local_settings'] = local_settings
 		self.entry(
```

### Comparing `mighty_logger-0.9.3/mighty_logger/simple_logger.py` & `mighty_logger-1.0.0/mighty_logger/simple_logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 		console_width: int = 60,
 		icon_set: int = 1,
 		global_bold_font: bool = False,
 		global_italic_font: bool = False,
 		global_invert_font: bool = False,
 		global_background: bool = False
 	) -> None:
-
 		if not hasattr(self, "_Logger__logger"):
 			if MightyLogger._instance is not None:
 				self.__logger = MightyLogger._instance
 				self.notice("An existing logger was taken into use")
 			else:
 				self.__logger = MightyLogger(
 					program_name=program_name,
```

### Comparing `mighty_logger-0.9.3/mighty_logger/src/__init__.py` & `mighty_logger-1.0.0/mighty_logger/src/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,10 +23,10 @@
 	AnsiColor,\
 	Dec2Hex,\
 	Dec2Ansi,\
 	Hex2Dec,\
 	Hex2Ansi,\
 	Ansi2Dec,\
 	Ansi2Hex
-from .entry_types import LoggerEntryTypes, ProcessEntryTypes, SelectionTypes, SelectionCategories
+from .entry_types import LoggerEntryTypes, ProcessEntryTypes, AdditionalEntryTypes, SelectionTypes, SelectionCategories
 from .environments import LogEnvironments
 from .sorting_keys import SortingKeys
```

### Comparing `mighty_logger-0.9.3/mighty_logger/src/animations.py` & `mighty_logger-1.0.0/mighty_logger/src/animations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 """
-The source of IndefiniteAnimation:
-https://github.com/kopensource/colored_logs/blob/develop/colored_logs/models/animation_type.py
-\n
 Copyright © 2023 Kalynovsky Valentin. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `mighty_logger-0.9.3/mighty_logger/src/ansi_format.py` & `mighty_logger-1.0.0/mighty_logger/src/ansi_format.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.9.3/mighty_logger/src/color_picker.py` & `mighty_logger-1.0.0/mighty_logger/src/color_picker.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.9.3/mighty_logger/src/entry_types.py` & `mighty_logger-1.0.0/mighty_logger/src/entry_types.py`

 * *Files 8% similar despite different names*

```diff
@@ -998,14 +998,256 @@
 			("", HexColor('SKYBLUE')),
 			("", HexColor('SKYBLUE')),
 			("", "")
 		),
 		icon=('⏲️', '🕙', '🟪', '⌛')
 	)
 
+class AdditionalEntryTypes:
+	hint = EntryType(
+		type_category="/",
+		type_name="HINT",
+		time_color=(
+			(AnsiColor('ORCHID', "foreground"), AnsiColor('LAVENDERBLUSH', "foreground")),
+			("", ""),
+			(HexColor('ORCHID'), HexColor('LAVENDERBLUSH')),
+			(HexColor('ORCHID'), HexColor('LAVENDERBLUSH')),
+			("", "")
+		),
+		status_color=(
+			(AnsiColor('ORANGE', "foreground"), AnsiColor('CHARTREUSE', "foreground")),
+			("", ""),
+			(HexColor('ORANGE'), HexColor('CHARTREUSE')),
+			(HexColor('ORANGE'), HexColor('CHARTREUSE')),
+			("", "")
+		),
+		type_color=(
+			(AnsiColor('GREEN', "foreground"), AnsiColor('PALEGREEN', "foreground")),
+			("", ""),
+			(HexColor('GREEN'), HexColor('PALEGREEN')),
+			(HexColor('GREEN'), HexColor('PALEGREEN')),
+			("", "")
+		),
+		message_color=(
+			(AnsiColor('DARKGREEN', "foreground"), AnsiColor('LIGHTGREEN', "foreground")),
+			("", ""),
+			(HexColor('DARKGREEN'), HexColor('LIGHTGREEN')),
+			(HexColor('DARKGREEN'), HexColor('LIGHTGREEN')),
+			("", "")
+		),
+		background_color=(
+			("", AnsiColor('DARKGREEN', "background")),
+			("", ""),
+			("", HexColor('DARKGREEN')),
+			("", HexColor('DARKGREEN')),
+			("", "")
+		),
+		icon=('🔍', '🔎', '🕵️', '🔬')
+	)
+	tip = EntryType(
+		type_category="/",
+		type_name="TIP",
+		time_color=(
+			(AnsiColor('ORCHID', "foreground"), AnsiColor('LAVENDERBLUSH', "foreground")),
+			("", ""),
+			(HexColor('ORCHID'), HexColor('LAVENDERBLUSH')),
+			(HexColor('ORCHID'), HexColor('LAVENDERBLUSH')),
+			("", "")
+		),
+		status_color=(
+			(AnsiColor('ORANGE', "foreground"), AnsiColor('CHARTREUSE', "foreground")),
+			("", ""),
+			(HexColor('ORANGE'), HexColor('CHARTREUSE')),
+			(HexColor('ORANGE'), HexColor('CHARTREUSE')),
+			("", "")
+		),
+		type_color=(
+			(AnsiColor('GREEN', "foreground"), AnsiColor('PALEGREEN', "foreground")),
+			("", ""),
+			(HexColor('GREEN'), HexColor('PALEGREEN')),
+			(HexColor('GREEN'), HexColor('PALEGREEN')),
+			("", "")
+		),
+		message_color=(
+			(AnsiColor('DARKGREEN', "foreground"), AnsiColor('LIGHTGREEN', "foreground")),
+			("", ""),
+			(HexColor('DARKGREEN'), HexColor('LIGHTGREEN')),
+			(HexColor('DARKGREEN'), HexColor('LIGHTGREEN')),
+			("", "")
+		),
+		background_color=(
+			("", AnsiColor('DARKGREEN', "background")),
+			("", ""),
+			("", HexColor('DARKGREEN')),
+			("", HexColor('DARKGREEN')),
+			("", "")
+		),
+		icon=('💡', '🌟', '🎯', '🔔')
+	)
+	important = EntryType(
+		type_category="/",
+		type_name="IMPORTANT",
+		time_color=(
+			(AnsiColor('ORCHID', "foreground"), AnsiColor('PURPLE', "foreground")),
+			("", ""),
+			(HexColor('ORCHID'), HexColor('PURPLE')),
+			(HexColor('ORCHID'), HexColor('PURPLE')),
+			("", "")
+		),
+		status_color=(
+			(AnsiColor('ORANGE', "foreground"), AnsiColor('DARKRED', "foreground")),
+			("", ""),
+			(HexColor('ORANGE'), HexColor('DARKRED')),
+			(HexColor('ORANGE'), HexColor('DARKRED')),
+			("", "")
+		),
+		type_color=(
+			(AnsiColor('LIGHTSKYBLUE', "foreground"), AnsiColor('NAVY', "foreground")),
+			("", ""),
+			(HexColor('LIGHTSKYBLUE'), HexColor('NAVY')),
+			(HexColor('LIGHTSKYBLUE'), HexColor('NAVY')),
+			("", "")
+		),
+		message_color=(
+			(AnsiColor('SKYBLUE', "foreground"), AnsiColor('MIDNIGHTBLUE', "foreground")),
+			("", ""),
+			(HexColor('SKYBLUE'), HexColor('MIDNIGHTBLUE')),
+			(HexColor('SKYBLUE'), HexColor('MIDNIGHTBLUE')),
+			("", "")
+		),
+		background_color=(
+			("", AnsiColor('SKYBLUE', "background")),
+			("", ""),
+			("", HexColor('SKYBLUE')),
+			("", HexColor('SKYBLUE')),
+			("", "")
+		),
+		icon=('❗️', '‼️', '⚠️', '🚨')
+	)
+	attention = EntryType(
+		type_category="/",
+		type_name="ATTENTION",
+		time_color=(
+			(AnsiColor('ORCHID', "foreground"), AnsiColor('DARKMAGENTA', "foreground")),
+			("", ""),
+			(HexColor('ORCHID'), HexColor('DARKMAGENTA')),
+			(HexColor('ORCHID'), HexColor('DARKMAGENTA')),
+			("", "")
+		),
+		status_color=(
+			(AnsiColor('ORANGE', "foreground"), AnsiColor('DARKRED', "foreground")),
+			("", ""),
+			(HexColor('ORANGE'), HexColor('DARKRED')),
+			(HexColor('ORANGE'), HexColor('DARKRED')),
+			("", "")
+		),
+		type_color=(
+			(AnsiColor('YELLOW', "foreground"), AnsiColor('NAVY', "foreground")),
+			("", ""),
+			(HexColor('YELLOW'), HexColor('NAVY')),
+			(HexColor('YELLOW'), HexColor('NAVY')),
+			("", "")
+		),
+		message_color=(
+			(AnsiColor('DARKYELLOW', "foreground"), AnsiColor('MIDNIGHTBLUE', "foreground")),
+			("", ""),
+			(HexColor('DARKYELLOW'), HexColor('MIDNIGHTBLUE')),
+			(HexColor('DARKYELLOW'), HexColor('MIDNIGHTBLUE')),
+			("", "")
+		),
+		background_color=(
+			("", AnsiColor('DARKYELLOW', "background")),
+			("", ""),
+			("", HexColor('DARKYELLOW')),
+			("", HexColor('DARKYELLOW')),
+			("", "")
+		),
+		icon=('⚡️', '⛔️', '⏰', '🛑')
+	)
+	caution = EntryType(
+		type_category="/",
+		type_name="CAUTION",
+		time_color=(
+			(AnsiColor('ORCHID', "foreground"), AnsiColor('DARKMAGENTA', "foreground")),
+			("", ""),
+			(HexColor('ORCHID'), HexColor('DARKMAGENTA')),
+			(HexColor('ORCHID'), HexColor('DARKMAGENTA')),
+			("", "")
+		),
+		status_color=(
+			(AnsiColor('ORANGE', "foreground"), AnsiColor('DARKRED', "foreground")),
+			("", ""),
+			(HexColor('ORANGE'), HexColor('DARKRED')),
+			(HexColor('ORANGE'), HexColor('DARKRED')),
+			("", "")
+		),
+		type_color=(
+			(AnsiColor('YELLOW', "foreground"), AnsiColor('NAVY', "foreground")),
+			("", ""),
+			(HexColor('YELLOW'), HexColor('NAVY')),
+			(HexColor('YELLOW'), HexColor('NAVY')),
+			("", "")
+		),
+		message_color=(
+			(AnsiColor('DARKYELLOW', "foreground"), AnsiColor('MIDNIGHTBLUE', "foreground")),
+			("", ""),
+			(HexColor('DARKYELLOW'), HexColor('MIDNIGHTBLUE')),
+			(HexColor('DARKYELLOW'), HexColor('MIDNIGHTBLUE')),
+			("", "")
+		),
+		background_color=(
+			("", AnsiColor('DARKYELLOW', "background")),
+			("", ""),
+			("", HexColor('DARKYELLOW')),
+			("", HexColor('DARKYELLOW')),
+			("", "")
+		),
+		icon=('⚠️', '⚡️', '⚙️', '🚧')
+	)
+	danger = EntryType(
+		type_category="/",
+		type_name="DANGER",
+		time_color=(
+			(AnsiColor('ORCHID', "foreground"), AnsiColor('LAVENDERBLUSH', "foreground")),
+			("", ""),
+			(HexColor('ORCHID'), HexColor('LAVENDERBLUSH')),
+			(HexColor('ORCHID'), HexColor('LAVENDERBLUSH')),
+			("", "")
+		),
+		status_color=(
+			(AnsiColor('ORANGE', "foreground"), AnsiColor('ORANGE', "foreground")),
+			("", ""),
+			(HexColor('ORANGE'), HexColor('ORANGE')),
+			(HexColor('ORANGE'), HexColor('ORANGE')),
+			("", "")
+		),
+		type_color=(
+			(AnsiColor('FIREBRICK', "foreground"), AnsiColor('YELLOW', "foreground")),
+			("", ""),
+			(HexColor('FIREBRICK'), HexColor('YELLOW')),
+			(HexColor('FIREBRICK'), HexColor('YELLOW')),
+			("", "")
+		),
+		message_color=(
+			(AnsiColor('DARKRED', "foreground"), AnsiColor('DARKYELLOW', "foreground")),
+			("", ""),
+			(HexColor('DARKRED'), HexColor('DARKYELLOW')),
+			(HexColor('DARKRED'), HexColor('DARKYELLOW')),
+			("", "")
+		),
+		background_color=(
+			("", AnsiColor('DARKRED', "background")),
+			("", ""),
+			("", HexColor('DARKRED')),
+			("", HexColor('DARKRED')),
+			("", "")
+		),
+		icon=('🔥', '💣', '☠️', '⚡️')
+	)
+
 class SelectionTypes:
 	debug = EntryType(
 		type_category="",
 		type_name="DEBUG",
 		time_color = (),
 		status_color = (),
 		type_color = (),
@@ -1239,14 +1481,74 @@
 		time_color = (),
 		status_color = (),
 		type_color = (),
 		message_color = (),
 		background_color = (),
 		icon = ()
 	)
+	hint = EntryType(
+		type_category="",
+		type_name="HINT",
+		time_color=(),
+		status_color=(),
+		type_color=(),
+		message_color=(),
+		background_color=(),
+		icon=()
+	)
+	tip = EntryType(
+		type_category="",
+		type_name="TIP",
+		time_color=(),
+		status_color=(),
+		type_color=(),
+		message_color=(),
+		background_color=(),
+		icon=()
+	)
+	important = EntryType(
+		type_category="",
+		type_name="IMPORTANT",
+		time_color=(),
+		status_color=(),
+		type_color=(),
+		message_color=(),
+		background_color=(),
+		icon=()
+	)
+	attention = EntryType(
+		type_category="",
+		type_name="ATTENTION",
+		time_color=(),
+		status_color=(),
+		type_color=(),
+		message_color=(),
+		background_color=(),
+		icon=()
+	)
+	caution = EntryType(
+		type_category="",
+		type_name="CAUTION",
+		time_color=(),
+		status_color=(),
+		type_color=(),
+		message_color=(),
+		background_color=(),
+		icon=()
+	)
+	danger = EntryType(
+		type_category="",
+		type_name="DANGER",
+		time_color=(),
+		status_color=(),
+		type_color=(),
+		message_color=(),
+		background_color=(),
+		icon=()
+	)
 
 class SelectionCategories:
 	debug = EntryType(
 		type_category="%",
 		type_name="",
 		time_color = (),
 		status_color = (),
@@ -1301,7 +1603,17 @@
 		time_color = (),
 		status_color = (),
 		type_color = (),
 		message_color = (),
 		background_color = (),
 		icon = ()
 	)
+	additional = EntryType(
+		type_category="/",
+		type_name="",
+		time_color=(),
+		status_color=(),
+		type_color=(),
+		message_color=(),
+		background_color=(),
+		icon=()
+	)
```

### Comparing `mighty_logger-0.9.3/mighty_logger/src/environments.py` & `mighty_logger-1.0.0/mighty_logger/src/environments.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.9.3/mighty_logger/src/sorting_keys.py` & `mighty_logger-1.0.0/mighty_logger/src/sorting_keys.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.9.3/mighty_logger.egg-info/PKG-INFO` & `mighty_logger-1.0.0/mighty_logger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: mighty-logger
-Version: 0.9.3
+Version: 1.0.0
 Summary: Mighty functional logger
 Author-email: Kalynovsky 'Nakamura Akira' Valentin <nakama3942@gmail.com>
 License: Apache License Version 2.0
 Project-URL: Repository, https://github.com/Nakama3942/mighty_logger
 Project-URL: Releases, https://github.com/Nakama3942/mighty_logger/releases
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Logging
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
@@ -122,15 +122,15 @@
 - [x] v0.7.1 - Modding update (buffer modification added - sorting, searching and selecting)
 - [x] v0.7.2 - Categories update (separated the entry category from the type)
 - [x] v0.8.0 - Export update (added conversion to csv)
 - [x] v0.9.0 - Extension update (made wheel format and instruction of toml)
 - [x] v0.9.1 - Documenting update (documented library)
 - [x] v0.9.2 - Feature update (made optimizations)
 - [x] v0.9.3 - Web docs update (added generation of web docs)
-- [ ] v1.0.0 - Completion of logger development (logger development completed)
+- [x] v1.0.0 - Completion of logger development (logger development completed)
 - [ ] v1.1.0 - Font update (added a class that formats text outside the logger)
 
 </details>
 
 - [Content](#content)
 
 ## Features
```

### Comparing `mighty_logger-0.9.3/mighty_logger.egg-info/SOURCES.txt` & `mighty_logger-1.0.0/mighty_logger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.9.3/pyproject.toml` & `mighty_logger-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -15,23 +15,23 @@
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mighty_logger"
-version = "0.9.3"
+version = "1.0.0"
 authors = [
 	{name = "Kalynovsky 'Nakamura Akira' Valentin", email = "nakama3942@gmail.com"},
 ]
 description = "Mighty functional logger"
 readme = "README.md"
 license = {text = "Apache License Version 2.0"}
 classifiers = [
-	"Development Status :: 4 - Beta",
+	"Development Status :: 5 - Production/Stable",
 	"Intended Audience :: Developers",
 	"License :: OSI Approved :: Apache Software License",
 	"Operating System :: OS Independent",
 	"Programming Language :: Python :: 3.11",
 	"Topic :: System :: Logging",
 ]
 requires-python = ">=3.11"
```

