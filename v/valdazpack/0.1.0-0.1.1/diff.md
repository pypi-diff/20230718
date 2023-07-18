# Comparing `tmp/valdazpack-0.1.0.tar.gz` & `tmp/valdazpack-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valdazpack-0.1.0.tar", max compression
+gzip compressed data, was "valdazpack-0.1.1.tar", max compression
```

## Comparing `valdazpack-0.1.0.tar` & `valdazpack-0.1.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0     1085 2022-08-29 23:54:26.816824 valdazpack-0.1.0/LICENSE
--rw-r--r--   0        0        0     1053 2023-07-17 21:24:59.897268 valdazpack-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-08-30 00:47:21.800787 valdazpack-0.1.0/README.rst
--rw-r--r--   0        0        0        0 2022-09-05 23:10:13.045452 valdazpack-0.1.0/src/valdazpack/__init__.py
--rw-r--r--   0        0        0     5154 2023-07-17 21:03:25.459261 valdazpack-0.1.0/src/valdazpack/__main__.py
--rw-r--r--   0        0        0       82 2022-12-19 23:13:39.653828 valdazpack-0.1.0/src/valdazpack/data/daz/audiences.txt
--rw-r--r--   0        0        0      186 2022-12-19 23:21:52.316696 valdazpack-0.1.0/src/valdazpack/data/daz/common_content_directories.txt
--rw-r--r--   0        0        0      539 2022-12-19 23:01:05.733458 valdazpack-0.1.0/src/valdazpack/data/daz/deprecated_categories.txt
--rw-r--r--   0        0        0      207 2022-12-19 23:13:59.167603 valdazpack-0.1.0/src/valdazpack/data/daz/deprecated_content_types.txt
--rw-r--r--   0        0        0     5597 2023-01-06 22:15:58.653750 valdazpack-0.1.0/src/valdazpack/data/daz/dson_external_file_references.txt
--rw-r--r--   0        0        0       28 2022-09-11 03:21:48.687333 valdazpack-0.1.0/src/valdazpack/data/daz/expected_runtime_directories.txt
--rw-r--r--   0        0        0      110 2023-03-21 22:26:33.861899 valdazpack-0.1.0/src/valdazpack/data/daz/import_file_extensions.txt
--rw-r--r--   0        0        0      104 2023-03-22 02:35:00.580416 valdazpack-0.1.0/src/valdazpack/data/daz/native_file_extensions.txt
--rw-r--r--   0        0        0      142 2022-12-19 23:05:07.289081 valdazpack-0.1.0/src/valdazpack/data/daz/reserved_package_prefixes.txt
--rw-r--r--   0        0        0      208 2022-12-26 04:23:20.072506 valdazpack-0.1.0/src/valdazpack/data/daz/special_categories.txt
--rw-r--r--   0        0        0      121 2022-12-19 23:15:44.533969 valdazpack-0.1.0/src/valdazpack/data/daz/user_facing_excluded_directories.txt
--rw-r--r--   0        0        0       73 2022-09-29 01:48:10.269010 valdazpack-0.1.0/src/valdazpack/data/poser/expected_libraries_directories.txt
--rw-r--r--   0        0        0       41 2022-09-29 01:48:12.821575 valdazpack-0.1.0/src/valdazpack/data/poser/expected_runtime_directories.txt
--rw-r--r--   0        0        0      169 2023-03-21 22:25:34.023326 valdazpack-0.1.0/src/valdazpack/data/poser/poser_file_extensions.txt
--rw-r--r--   0        0        0      278 2022-09-30 03:19:43.642827 valdazpack-0.1.0/src/valdazpack/data/schemas/djl.schema.json
--rw-r--r--   0        0        0    48236 2022-12-15 06:06:50.007131 valdazpack-0.1.0/src/valdazpack/data/schemas/dson.schema.json
--rw-r--r--   0        0        0     6022 2022-04-30 05:16:10.431363 valdazpack-0.1.0/src/valdazpack/data/schemas/Manifest.xsd
--rw-r--r--   0        0        0    11094 2022-12-26 00:04:42.553870 valdazpack-0.1.0/src/valdazpack/data/schemas/Metadata.xsd
--rw-r--r--   0        0        0     3563 2022-05-20 21:44:36.549122 valdazpack-0.1.0/src/valdazpack/data/schemas/Supplement.xsd
--rw-r--r--   0        0        0     3487 2023-03-21 00:31:42.637863 valdazpack-0.1.0/src/valdazpack/data/templates/report.css
--rw-r--r--   0        0        0     5507 2023-01-12 23:25:41.181128 valdazpack-0.1.0/src/valdazpack/data/templates/report.html.jinja
--rw-r--r--   0        0        0     1565 2023-03-22 00:33:29.914470 valdazpack-0.1.0/src/valdazpack/data/templates/report.js
--rw-r--r--   0        0        0     2375 2023-01-07 06:01:10.350265 valdazpack-0.1.0/src/valdazpack/data/templates/report.txt.jinja
--rw-r--r--   0        0        0      174 2022-10-25 04:33:59.210378 valdazpack-0.1.0/src/valdazpack/issues/__init__.py
--rw-r--r--   0        0        0     3921 2023-03-22 01:35:54.887195 valdazpack-0.1.0/src/valdazpack/issues/contentdirectory.py
--rw-r--r--   0        0        0     2716 2023-01-12 23:19:13.531945 valdazpack-0.1.0/src/valdazpack/issues/data.py
--rw-r--r--   0        0        0     2075 2023-01-12 22:34:05.574615 valdazpack-0.1.0/src/valdazpack/issues/dsonfiles.py
--rw-r--r--   0        0        0      920 2023-01-05 18:57:34.768791 valdazpack-0.1.0/src/valdazpack/issues/geometries.py
--rw-r--r--   0        0        0      901 2023-01-05 18:57:34.371791 valdazpack-0.1.0/src/valdazpack/issues/libraries.py
--rw-r--r--   0        0        0     1114 2023-01-05 18:57:33.926793 valdazpack-0.1.0/src/valdazpack/issues/manifest.py
--rw-r--r--   0        0        0     8046 2023-01-05 18:57:33.546790 valdazpack-0.1.0/src/valdazpack/issues/metadatafile.py
--rw-r--r--   0        0        0     1082 2022-10-16 22:19:10.273269 valdazpack-0.1.0/src/valdazpack/issues/package.py
--rw-r--r--   0        0        0     3277 2023-01-05 18:57:33.021791 valdazpack-0.1.0/src/valdazpack/issues/runtime.py
--rw-r--r--   0        0        0     1756 2022-10-23 23:11:24.610000 valdazpack-0.1.0/src/valdazpack/issues/supplementfile.py
--rw-r--r--   0        0        0     2115 2022-12-25 07:17:26.284582 valdazpack-0.1.0/src/valdazpack/issues/support.py
--rw-r--r--   0        0        0      229 2022-10-23 23:21:23.629820 valdazpack-0.1.0/src/valdazpack/issues/zipfile.py
--rw-r--r--   0        0        0        0 2022-10-27 04:10:50.868562 valdazpack-0.1.0/src/valdazpack/rules/__init__.py
--rw-r--r--   0        0        0    11556 2023-03-22 02:34:29.799765 valdazpack-0.1.0/src/valdazpack/rules/contentdirectory.py
--rw-r--r--   0        0        0     6122 2023-01-12 23:54:48.326685 valdazpack-0.1.0/src/valdazpack/rules/datadirectory.py
--rw-r--r--   0        0        0     7668 2023-03-18 03:14:56.249828 valdazpack-0.1.0/src/valdazpack/rules/dsonfiles.py
--rw-r--r--   0        0        0    22233 2023-01-12 22:59:54.589007 valdazpack-0.1.0/src/valdazpack/rules/metadatafiles.py
--rw-r--r--   0        0        0     1701 2023-01-07 05:18:06.188047 valdazpack-0.1.0/src/valdazpack/rules/package.py
--rw-r--r--   0        0        0     2738 2023-01-07 05:18:06.188047 valdazpack-0.1.0/src/valdazpack/rules/packagemanifest.py
--rw-r--r--   0        0        0     3588 2023-01-07 04:46:12.383612 valdazpack-0.1.0/src/valdazpack/rules/packagesupplementfile.py
--rw-r--r--   0        0        0     7090 2023-01-12 20:33:01.902261 valdazpack-0.1.0/src/valdazpack/rules/runtimedirectory.py
--rw-r--r--   0        0        0     2642 2023-01-12 20:34:19.472932 valdazpack-0.1.0/src/valdazpack/rules/runtimegeometriesdirectory.py
--rw-r--r--   0        0        0     3121 2023-01-10 00:32:34.555553 valdazpack-0.1.0/src/valdazpack/rules/runtimelibrariesdirectory.py
--rw-r--r--   0        0        0     3939 2023-01-10 00:32:34.555553 valdazpack-0.1.0/src/valdazpack/rules/runtimesupportdirectory.py
--rw-r--r--   0        0        0     1268 2023-01-07 02:41:50.310647 valdazpack-0.1.0/src/valdazpack/rules/zipfile.py
--rw-r--r--   0        0        0      145 2022-10-27 04:15:16.882331 valdazpack-0.1.0/src/valdazpack/validator/__init__.py
--rw-r--r--   0        0        0     1379 2022-12-25 05:26:07.181510 valdazpack-0.1.0/src/valdazpack/validator/issues.py
--rw-r--r--   0        0        0     2148 2023-01-07 04:13:47.687679 valdazpack-0.1.0/src/valdazpack/validator/package.py
--rw-r--r--   0        0        0      609 2022-10-27 02:09:13.847021 valdazpack-0.1.0/src/valdazpack/validator/resources.py
--rw-r--r--   0        0        0     1741 2023-01-07 02:41:50.313647 valdazpack-0.1.0/src/valdazpack/validator/ruleset.py
--rw-r--r--   0        0        0     2129 2023-04-16 21:18:49.873534 valdazpack-0.1.0/src/valdazpack/validator/schema.py
--rw-r--r--   0        0        0     6466 2023-04-16 21:18:38.776652 valdazpack-0.1.0/src/valdazpack/validator/utilities.py
--rw-r--r--   0        0        0     1605 2023-01-12 23:09:52.137826 valdazpack-0.1.0/src/valdazpack/validator/validate.py
--rw-r--r--   0        0        0     4400 2023-04-16 21:18:56.658222 valdazpack-0.1.0/src/valdazpack/validator/validationdata.py
--rw-r--r--   0        0        0      890 1970-01-01 00:00:00.000000 valdazpack-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1085 2022-08-29 23:54:26.816824 valdazpack-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1088 2023-07-18 00:53:06.289991 valdazpack-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1938 2023-07-17 23:19:38.701219 valdazpack-0.1.1/README.rst
+-rw-r--r--   0        0        0        0 2022-09-05 23:10:13.045452 valdazpack-0.1.1/src/valdazpack/__init__.py
+-rw-r--r--   0        0        0     5154 2023-07-17 22:52:02.335528 valdazpack-0.1.1/src/valdazpack/__main__.py
+-rw-r--r--   0        0        0       82 2022-12-19 23:13:39.653828 valdazpack-0.1.1/src/valdazpack/data/daz/audiences.txt
+-rw-r--r--   0        0        0      186 2022-12-19 23:21:52.316696 valdazpack-0.1.1/src/valdazpack/data/daz/common_content_directories.txt
+-rw-r--r--   0        0        0      539 2022-12-19 23:01:05.733458 valdazpack-0.1.1/src/valdazpack/data/daz/deprecated_categories.txt
+-rw-r--r--   0        0        0      207 2022-12-19 23:13:59.167603 valdazpack-0.1.1/src/valdazpack/data/daz/deprecated_content_types.txt
+-rw-r--r--   0        0        0     5597 2023-01-06 22:15:58.653750 valdazpack-0.1.1/src/valdazpack/data/daz/dson_external_file_references.txt
+-rw-r--r--   0        0        0       28 2022-09-11 03:21:48.687333 valdazpack-0.1.1/src/valdazpack/data/daz/expected_runtime_directories.txt
+-rw-r--r--   0        0        0      110 2023-03-21 22:26:33.861899 valdazpack-0.1.1/src/valdazpack/data/daz/import_file_extensions.txt
+-rw-r--r--   0        0        0      104 2023-03-22 02:35:00.580416 valdazpack-0.1.1/src/valdazpack/data/daz/native_file_extensions.txt
+-rw-r--r--   0        0        0      142 2022-12-19 23:05:07.289081 valdazpack-0.1.1/src/valdazpack/data/daz/reserved_package_prefixes.txt
+-rw-r--r--   0        0        0      208 2022-12-26 04:23:20.072506 valdazpack-0.1.1/src/valdazpack/data/daz/special_categories.txt
+-rw-r--r--   0        0        0      121 2022-12-19 23:15:44.533969 valdazpack-0.1.1/src/valdazpack/data/daz/user_facing_excluded_directories.txt
+-rw-r--r--   0        0        0       73 2022-09-29 01:48:10.269010 valdazpack-0.1.1/src/valdazpack/data/poser/expected_libraries_directories.txt
+-rw-r--r--   0        0        0       41 2022-09-29 01:48:12.821575 valdazpack-0.1.1/src/valdazpack/data/poser/expected_runtime_directories.txt
+-rw-r--r--   0        0        0      169 2023-03-21 22:25:34.023326 valdazpack-0.1.1/src/valdazpack/data/poser/poser_file_extensions.txt
+-rw-r--r--   0        0        0      278 2022-09-30 03:19:43.642827 valdazpack-0.1.1/src/valdazpack/data/schemas/djl.schema.json
+-rw-r--r--   0        0        0    48236 2022-12-15 06:06:50.007131 valdazpack-0.1.1/src/valdazpack/data/schemas/dson.schema.json
+-rw-r--r--   0        0        0     6022 2022-04-30 05:16:10.431363 valdazpack-0.1.1/src/valdazpack/data/schemas/Manifest.xsd
+-rw-r--r--   0        0        0    11094 2022-12-26 00:04:42.553870 valdazpack-0.1.1/src/valdazpack/data/schemas/Metadata.xsd
+-rw-r--r--   0        0        0     3563 2022-05-20 21:44:36.549122 valdazpack-0.1.1/src/valdazpack/data/schemas/Supplement.xsd
+-rw-r--r--   0        0        0     3487 2023-03-21 00:31:42.637863 valdazpack-0.1.1/src/valdazpack/data/templates/report.css
+-rw-r--r--   0        0        0     5507 2023-01-12 23:25:41.181128 valdazpack-0.1.1/src/valdazpack/data/templates/report.html.jinja
+-rw-r--r--   0        0        0     1565 2023-03-22 00:33:29.914470 valdazpack-0.1.1/src/valdazpack/data/templates/report.js
+-rw-r--r--   0        0        0     2375 2023-01-07 06:01:10.350265 valdazpack-0.1.1/src/valdazpack/data/templates/report.txt.jinja
+-rw-r--r--   0        0        0      174 2022-10-25 04:33:59.210378 valdazpack-0.1.1/src/valdazpack/issues/__init__.py
+-rw-r--r--   0        0        0     3921 2023-03-22 01:35:54.887195 valdazpack-0.1.1/src/valdazpack/issues/contentdirectory.py
+-rw-r--r--   0        0        0     2716 2023-01-12 23:19:13.531945 valdazpack-0.1.1/src/valdazpack/issues/data.py
+-rw-r--r--   0        0        0     2075 2023-01-12 22:34:05.574615 valdazpack-0.1.1/src/valdazpack/issues/dsonfiles.py
+-rw-r--r--   0        0        0      920 2023-01-05 18:57:34.768791 valdazpack-0.1.1/src/valdazpack/issues/geometries.py
+-rw-r--r--   0        0        0      901 2023-01-05 18:57:34.371791 valdazpack-0.1.1/src/valdazpack/issues/libraries.py
+-rw-r--r--   0        0        0     1114 2023-01-05 18:57:33.926793 valdazpack-0.1.1/src/valdazpack/issues/manifest.py
+-rw-r--r--   0        0        0     8046 2023-01-05 18:57:33.546790 valdazpack-0.1.1/src/valdazpack/issues/metadatafile.py
+-rw-r--r--   0        0        0     1082 2022-10-16 22:19:10.273269 valdazpack-0.1.1/src/valdazpack/issues/package.py
+-rw-r--r--   0        0        0     3277 2023-01-05 18:57:33.021791 valdazpack-0.1.1/src/valdazpack/issues/runtime.py
+-rw-r--r--   0        0        0     1756 2022-10-23 23:11:24.610000 valdazpack-0.1.1/src/valdazpack/issues/supplementfile.py
+-rw-r--r--   0        0        0     2115 2022-12-25 07:17:26.284582 valdazpack-0.1.1/src/valdazpack/issues/support.py
+-rw-r--r--   0        0        0      229 2022-10-23 23:21:23.629820 valdazpack-0.1.1/src/valdazpack/issues/zipfile.py
+-rw-r--r--   0        0        0        0 2022-10-27 04:10:50.868562 valdazpack-0.1.1/src/valdazpack/rules/__init__.py
+-rw-r--r--   0        0        0    11556 2023-03-22 02:34:29.799765 valdazpack-0.1.1/src/valdazpack/rules/contentdirectory.py
+-rw-r--r--   0        0        0     6122 2023-01-12 23:54:48.326685 valdazpack-0.1.1/src/valdazpack/rules/datadirectory.py
+-rw-r--r--   0        0        0     7668 2023-03-18 03:14:56.249828 valdazpack-0.1.1/src/valdazpack/rules/dsonfiles.py
+-rw-r--r--   0        0        0    22233 2023-01-12 22:59:54.589007 valdazpack-0.1.1/src/valdazpack/rules/metadatafiles.py
+-rw-r--r--   0        0        0     1701 2023-01-07 05:18:06.188047 valdazpack-0.1.1/src/valdazpack/rules/package.py
+-rw-r--r--   0        0        0     2738 2023-01-07 05:18:06.188047 valdazpack-0.1.1/src/valdazpack/rules/packagemanifest.py
+-rw-r--r--   0        0        0     3588 2023-01-07 04:46:12.383612 valdazpack-0.1.1/src/valdazpack/rules/packagesupplementfile.py
+-rw-r--r--   0        0        0     7090 2023-01-12 20:33:01.902261 valdazpack-0.1.1/src/valdazpack/rules/runtimedirectory.py
+-rw-r--r--   0        0        0     2642 2023-01-12 20:34:19.472932 valdazpack-0.1.1/src/valdazpack/rules/runtimegeometriesdirectory.py
+-rw-r--r--   0        0        0     3121 2023-01-10 00:32:34.555553 valdazpack-0.1.1/src/valdazpack/rules/runtimelibrariesdirectory.py
+-rw-r--r--   0        0        0     3939 2023-01-10 00:32:34.555553 valdazpack-0.1.1/src/valdazpack/rules/runtimesupportdirectory.py
+-rw-r--r--   0        0        0     1268 2023-01-07 02:41:50.310647 valdazpack-0.1.1/src/valdazpack/rules/zipfile.py
+-rw-r--r--   0        0        0      145 2022-10-27 04:15:16.882331 valdazpack-0.1.1/src/valdazpack/validator/__init__.py
+-rw-r--r--   0        0        0     1379 2022-12-25 05:26:07.181510 valdazpack-0.1.1/src/valdazpack/validator/issues.py
+-rw-r--r--   0        0        0     2148 2023-01-07 04:13:47.687679 valdazpack-0.1.1/src/valdazpack/validator/package.py
+-rw-r--r--   0        0        0      609 2022-10-27 02:09:13.847021 valdazpack-0.1.1/src/valdazpack/validator/resources.py
+-rw-r--r--   0        0        0     1741 2023-01-07 02:41:50.313647 valdazpack-0.1.1/src/valdazpack/validator/ruleset.py
+-rw-r--r--   0        0        0     2129 2023-04-16 21:18:49.873534 valdazpack-0.1.1/src/valdazpack/validator/schema.py
+-rw-r--r--   0        0        0     6466 2023-04-16 21:18:38.776652 valdazpack-0.1.1/src/valdazpack/validator/utilities.py
+-rw-r--r--   0        0        0     1605 2023-01-12 23:09:52.137826 valdazpack-0.1.1/src/valdazpack/validator/validate.py
+-rw-r--r--   0        0        0     4400 2023-04-16 21:18:56.658222 valdazpack-0.1.1/src/valdazpack/validator/validationdata.py
+-rw-r--r--   0        0        0     2859 1970-01-01 00:00:00.000000 valdazpack-0.1.1/PKG-INFO
```

### Comparing `valdazpack-0.1.0/LICENSE` & `valdazpack-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `valdazpack-0.1.0/pyproject.toml` & `valdazpack-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "valdazpack"
-version = "0.1.0"
+version = "0.1.1"
 description = "DAZ Package Validator"
 license = "MIT"
 authors = ["Omni Flux <omniflux@omniflux.com>"]
 readme = "README.rst"
+repository = "https://github.com/Omniflux/valdazpack"
 classifiers = [
-	"Private :: Do Not Upload",
 	"Development Status :: 3 - Alpha",
 	"Operating System :: OS Independent",
 	"Programming Language :: Python :: 3 :: Only",
 	"Programming Language :: Python :: 3.11",
 	"Topic :: Utilities"
 ]
 
@@ -30,12 +30,12 @@
 types-pillow = "^10.0.0.1"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4.0"
 pytest-mock = "^3.11.1"
 
 [tool.poetry.scripts]
-valdazpack = {reference = "valdazpack.main", type = "console"}
+valdazpack = {reference = "valdazpack.__main__:_main", type = "console"}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `valdazpack-0.1.0/src/valdazpack/__main__.py` & `valdazpack-0.1.1/src/valdazpack/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 		raise ArgumentTypeError(repr(e))
 	except Exception as e:
 		raise ArgumentTypeError(e)
 
 def _main() -> None:
 	parser = ArgumentParser(description = 'Validate DAZ Studio Product', epilog = 'For non-DIM ZIP files, a subdirectory may be specified as the content root by appending !<subdirectory> to the filename: "example.zip!My Library"')
 	parser.add_argument('product_path', type = _content_location, nargs = '+', help = 'DIM Packages, ZIP files, or Content Directories to validate')
-	parser.add_argument('-d', '--dependencies', type = _content_location, nargs = '*', help = 'additional DIM Packages, ZIP files, or Content Directories which are not validated but which the validated product depends on')
+	parser.add_argument('-d', '--dependencies', type = _content_location, nargs = '+', help = 'additional DIM Packages, ZIP files, or Content Directories which are not validated but which the validated product depends on')
 
 	parser.add_argument('-D', '--daz', action = 'store_true', help = 'enable validation rules for products distributed by Daz Productions, Inc')
 	parser.add_argument('-O', '--daz-original', action = 'store_true', help = 'enable validation rules for products produced by Daz Productions, Inc')
 
 	parser.add_argument('-p', '--poser', action = 'store_true', help = 'enable validation rules for included Poser content (experimental)')
 	parser.add_argument('-s', '--dson-schema', action = 'store_true', help = 'enable DSON schema checking (experimental)')
 
@@ -104,9 +104,9 @@
 	profiler = cProfile.Profile()
 	profiler.enable()
 	_main()
 	profiler.disable()
 	pstats.Stats(profiler).dump_stats('stats.profiler')
  
 if __name__ == '__main__':
-	# _profile()
-	_main()
+	_profile()
+	# _main()
```

### Comparing `valdazpack-0.1.0/src/valdazpack/data/daz/deprecated_categories.txt` & `valdazpack-0.1.1/src/valdazpack/data/daz/deprecated_categories.txt`

 * *Files identical despite different names*

### Comparing `valdazpack-0.1.0/src/valdazpack/data/daz/dson_external_file_references.txt` & `valdazpack-0.1.1/src/valdazpack/data/daz/dson_external_file_references.txt`

 * *Files identical despite different names*

### Comparing `valdazpack-0.1.0/src/valdazpack/data/schemas/dson.schema.json` & `valdazpack-0.1.1/src/valdazpack/data/schemas/dson.schema.json`

 * *Files identical despite different names*

### Comparing `valdazpack-0.1.0/src/valdazpack/data/schemas/Manifest.xsd` & `valdazpack-0.1.1/src/valdazpack/data/schemas/Manifest.xsd`

 * *Files identical despite different names*

### Comparing `valdazpack-0.1.0/src/valdazpack/data/schemas/Metadata.xsd` & `valdazpack-0.1.1/src/valdazpack/data/schemas/Metadata.xsd`

 * *Files identical despite different names*

### Comparing `valdazpack-0.1.0/src/valdazpack/data/schemas/Supplement.xsd` & `valdazpack-0.1.1/src/valdazpack/data/schemas/Supplement.xsd`

 * *Files identical despite different names*

### Comparing `valdazpack-0.1.0/src/valdazpack/data/templates/report.css` & `valdazpack-0.1.1/src/valdazpack/data/templates/report.css`

 * *Files identical despite different names*

### Comparing `valdazpack-0.1.0/src/valdazpack/data/templates/report.html.jinja` & `valdazpack-0.1.1/src/valdazpack/data/templates/report.html.jinja`

 * *Files identical despite different names*

### Comparing `valdazpack-0.1.0/src/valdazpack/data/templates/report.js` & `valdazpack-0.1.1/src/valdazpack/data/templates/report.js`

 * *Files identical despite different names*

### Comparing `valdazpack-0.1.0/src/valdazpack/data/templates/report.txt.jinja` & `valdazpack-0.1.1/src/valdazpack/data/templates/report.txt.jinja`

 * *Files identical despite different names*

### Comparing `valdazpack-0.1.0/src/valdazpack/issues/contentdirectory.py` & `valdazpack-0.1.1/src/valdazpack/issues/contentdirectory.py`

 * *Files identical despite different names*

### Comparing `valdazpack-0.1.0/src/valdazpack/issues/data.py` & `valdazpack-0.1.1/src/valdazpack/issues/data.py`

 * *Files identical despite different names*

### Comparing `valdazpack-0.1.0/src/valdazpack/issues/dsonfiles.py` & `valdazpack-0.1.1/src/valdazpack/issues/dsonfiles.py`

 * *Files identical despite different names*

### Comparing `valdazpack-0.1.0/src/valdazpack/issues/geometries.py` & `valdazpack-0.1.1/src/valdazpack/issues/geometries.py`

 * *Files identical despite different names*

### Comparing `valdazpack-0.1.0/src/valdazpack/issues/libraries.py` & `valdazpack-0.1.1/src/valdazpack/issues/libraries.py`

 * *Files identical despite different names*

### Comparing `valdazpack-0.1.0/src/valdazpack/issues/manifest.py` & `valdazpack-0.1.1/src/valdazpack/issues/manifest.py`

 * *Files identical despite different names*

### Comparing `valdazpack-0.1.0/src/valdazpack/issues/metadatafile.py` & `valdazpack-0.1.1/src/valdazpack/issues/metadatafile.py`

 * *Files identical despite different names*

### Comparing `valdazpack-0.1.0/src/valdazpack/issues/package.py` & `valdazpack-0.1.1/src/valdazpack/issues/package.py`

 * *Files identical despite different names*

### Comparing `valdazpack-0.1.0/src/valdazpack/issues/runtime.py` & `valdazpack-0.1.1/src/valdazpack/issues/runtime.py`

 * *Files identical despite different names*

### Comparing `valdazpack-0.1.0/src/valdazpack/issues/supplementfile.py` & `valdazpack-0.1.1/src/valdazpack/issues/supplementfile.py`

 * *Files identical despite different names*

### Comparing `valdazpack-0.1.0/src/valdazpack/issues/support.py` & `valdazpack-0.1.1/src/valdazpack/issues/support.py`

 * *Files identical despite different names*

### Comparing `valdazpack-0.1.0/src/valdazpack/rules/contentdirectory.py` & `valdazpack-0.1.1/src/valdazpack/rules/contentdirectory.py`

 * *Files identical despite different names*

### Comparing `valdazpack-0.1.0/src/valdazpack/rules/datadirectory.py` & `valdazpack-0.1.1/src/valdazpack/rules/datadirectory.py`

 * *Files identical despite different names*

### Comparing `valdazpack-0.1.0/src/valdazpack/rules/dsonfiles.py` & `valdazpack-0.1.1/src/valdazpack/rules/dsonfiles.py`

 * *Files identical despite different names*

### Comparing `valdazpack-0.1.0/src/valdazpack/rules/metadatafiles.py` & `valdazpack-0.1.1/src/valdazpack/rules/metadatafiles.py`

 * *Files identical despite different names*

### Comparing `valdazpack-0.1.0/src/valdazpack/rules/package.py` & `valdazpack-0.1.1/src/valdazpack/rules/package.py`

 * *Files identical despite different names*

### Comparing `valdazpack-0.1.0/src/valdazpack/rules/packagemanifest.py` & `valdazpack-0.1.1/src/valdazpack/rules/packagemanifest.py`

 * *Files identical despite different names*

### Comparing `valdazpack-0.1.0/src/valdazpack/rules/packagesupplementfile.py` & `valdazpack-0.1.1/src/valdazpack/rules/packagesupplementfile.py`

 * *Files identical despite different names*

### Comparing `valdazpack-0.1.0/src/valdazpack/rules/runtimedirectory.py` & `valdazpack-0.1.1/src/valdazpack/rules/runtimedirectory.py`

 * *Files identical despite different names*

### Comparing `valdazpack-0.1.0/src/valdazpack/rules/runtimegeometriesdirectory.py` & `valdazpack-0.1.1/src/valdazpack/rules/runtimegeometriesdirectory.py`

 * *Files identical despite different names*

### Comparing `valdazpack-0.1.0/src/valdazpack/rules/runtimelibrariesdirectory.py` & `valdazpack-0.1.1/src/valdazpack/rules/runtimelibrariesdirectory.py`

 * *Files identical despite different names*

### Comparing `valdazpack-0.1.0/src/valdazpack/rules/runtimesupportdirectory.py` & `valdazpack-0.1.1/src/valdazpack/rules/runtimesupportdirectory.py`

 * *Files identical despite different names*

### Comparing `valdazpack-0.1.0/src/valdazpack/rules/zipfile.py` & `valdazpack-0.1.1/src/valdazpack/rules/zipfile.py`

 * *Files identical despite different names*

### Comparing `valdazpack-0.1.0/src/valdazpack/validator/issues.py` & `valdazpack-0.1.1/src/valdazpack/validator/issues.py`

 * *Files identical despite different names*

### Comparing `valdazpack-0.1.0/src/valdazpack/validator/package.py` & `valdazpack-0.1.1/src/valdazpack/validator/package.py`

 * *Files identical despite different names*

### Comparing `valdazpack-0.1.0/src/valdazpack/validator/resources.py` & `valdazpack-0.1.1/src/valdazpack/validator/resources.py`

 * *Files identical despite different names*

### Comparing `valdazpack-0.1.0/src/valdazpack/validator/ruleset.py` & `valdazpack-0.1.1/src/valdazpack/validator/ruleset.py`

 * *Files identical despite different names*

### Comparing `valdazpack-0.1.0/src/valdazpack/validator/schema.py` & `valdazpack-0.1.1/src/valdazpack/validator/schema.py`

 * *Files identical despite different names*

### Comparing `valdazpack-0.1.0/src/valdazpack/validator/utilities.py` & `valdazpack-0.1.1/src/valdazpack/validator/utilities.py`

 * *Files identical despite different names*

### Comparing `valdazpack-0.1.0/src/valdazpack/validator/validate.py` & `valdazpack-0.1.1/src/valdazpack/validator/validate.py`

 * *Files identical despite different names*

### Comparing `valdazpack-0.1.0/src/valdazpack/validator/validationdata.py` & `valdazpack-0.1.1/src/valdazpack/validator/validationdata.py`

 * *Files identical despite different names*

