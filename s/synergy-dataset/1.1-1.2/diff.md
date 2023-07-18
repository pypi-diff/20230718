# Comparing `tmp/synergy-dataset-1.1.tar.gz` & `tmp/synergy-dataset-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synergy-dataset-1.1.tar", last modified: Fri Jul 14 10:38:43 2023, max compression
+gzip compressed data, was "synergy-dataset-1.2.tar", last modified: Tue Jul 18 08:48:43 2023, max compression
```

## Comparing `synergy-dataset-1.1.tar` & `synergy-dataset-1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:38:43.114902 synergy-dataset-1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:38:43.110902 synergy-dataset-1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:38:43.110902 synergy-dataset-1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-14 10:38:29.000000 synergy-dataset-1.1/.github/workflows/python-lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-14 10:38:29.000000 synergy-dataset-1.1/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-14 10:38:29.000000 synergy-dataset-1.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-14 10:38:29.000000 synergy-dataset-1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-14 10:38:29.000000 synergy-dataset-1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-14 10:38:29.000000 synergy-dataset-1.1/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-14 10:38:29.000000 synergy-dataset-1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-14 10:38:43.114902 synergy-dataset-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-14 10:38:29.000000 synergy-dataset-1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-14 10:38:29.000000 synergy-dataset-1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 10:38:43.114902 synergy-dataset-1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:38:43.110902 synergy-dataset-1.1/synergy_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-14 10:38:29.000000 synergy-dataset-1.1/synergy_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9900 2023-07-14 10:38:29.000000 synergy-dataset-1.1/synergy_dataset/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-14 10:38:42.000000 synergy-dataset-1.1/synergy_dataset/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-07-14 10:38:29.000000 synergy-dataset-1.1/synergy_dataset/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:38:43.114902 synergy-dataset-1.1/synergy_dataset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-14 10:38:43.000000 synergy-dataset-1.1/synergy_dataset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-14 10:38:43.000000 synergy-dataset-1.1/synergy_dataset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 10:38:43.000000 synergy-dataset-1.1/synergy_dataset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-14 10:38:43.000000 synergy-dataset-1.1/synergy_dataset.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-14 10:38:43.000000 synergy-dataset-1.1/synergy_dataset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-14 10:38:43.000000 synergy-dataset-1.1/synergy_dataset.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:38:43.114902 synergy-dataset-1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-14 10:38:29.000000 synergy-dataset-1.1/tests/test_synergy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:48:43.457788 synergy-dataset-1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:48:43.453788 synergy-dataset-1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:48:43.453788 synergy-dataset-1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-18 08:48:30.000000 synergy-dataset-1.2/.github/workflows/python-lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-18 08:48:30.000000 synergy-dataset-1.2/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-18 08:48:30.000000 synergy-dataset-1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-18 08:48:30.000000 synergy-dataset-1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-18 08:48:30.000000 synergy-dataset-1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-18 08:48:30.000000 synergy-dataset-1.2/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-18 08:48:30.000000 synergy-dataset-1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-18 08:48:43.457788 synergy-dataset-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-18 08:48:30.000000 synergy-dataset-1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-18 08:48:30.000000 synergy-dataset-1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 08:48:43.457788 synergy-dataset-1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:48:43.453788 synergy-dataset-1.2/synergy_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-18 08:48:30.000000 synergy-dataset-1.2/synergy_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9900 2023-07-18 08:48:30.000000 synergy-dataset-1.2/synergy_dataset/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-18 08:48:43.000000 synergy-dataset-1.2/synergy_dataset/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9696 2023-07-18 08:48:30.000000 synergy-dataset-1.2/synergy_dataset/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:48:43.457788 synergy-dataset-1.2/synergy_dataset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-18 08:48:43.000000 synergy-dataset-1.2/synergy_dataset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-18 08:48:43.000000 synergy-dataset-1.2/synergy_dataset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 08:48:43.000000 synergy-dataset-1.2/synergy_dataset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-18 08:48:43.000000 synergy-dataset-1.2/synergy_dataset.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-18 08:48:43.000000 synergy-dataset-1.2/synergy_dataset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 08:48:43.000000 synergy-dataset-1.2/synergy_dataset.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:48:43.457788 synergy-dataset-1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-18 08:48:30.000000 synergy-dataset-1.2/tests/test_synergy.py
```

### Comparing `synergy-dataset-1.1/.github/workflows/python-package.yml` & `synergy-dataset-1.2/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `synergy-dataset-1.1/.github/workflows/python-publish.yml` & `synergy-dataset-1.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `synergy-dataset-1.1/.gitignore` & `synergy-dataset-1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `synergy-dataset-1.1/LICENSE` & `synergy-dataset-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `synergy-dataset-1.1/PKG-INFO` & `synergy-dataset-1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synergy-dataset
-Version: 1.1
+Version: 1.2
 Summary: Python package for the SYNERGY dataset
 Author-email: Jonathan de Bruin <asreview@uu.nl>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `synergy-dataset-1.1/README.md` & `synergy-dataset-1.2/README.md`

 * *Files identical despite different names*

### Comparing `synergy-dataset-1.1/pyproject.toml` & `synergy-dataset-1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `synergy-dataset-1.1/synergy_dataset/__main__.py` & `synergy-dataset-1.2/synergy_dataset/__main__.py`

 * *Files identical despite different names*

### Comparing `synergy-dataset-1.1/synergy_dataset/base.py` & `synergy-dataset-1.2/synergy_dataset/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -135,83 +135,85 @@
         version = SYNERGY_VERSION if version is None else version
         path = Path(path, f"synergy-dataset-{version}")
 
     for dataset in sorted(
         glob.glob(str(Path(path, "*", "metadata.json"))),
         key=lambda x: x.lower(),
     ):
-        yield Dataset(Path(dataset).parts[-2])
+        yield Dataset(Path(dataset).parts[-2], path=Path(dataset).parent)
 
 
 class Dataset:
     """Dataset object belonging to a systematic review."""
 
-    def __init__(self, name):
+    def __init__(self, name, path=None):
         super().__init__()
         self.name = name
+        self.path = path
+
+        # create a path if not present
+        self._path = path if path else Path(_get_path_raw_dataset(), self.name)
 
     @property
     def cite(self):
         """Citation for the publication."""
         if not hasattr(self, "_cite"):
             with open(
-                Path(_get_path_raw_dataset(), self.name, "CITATION.txt"),
+                Path(self._path, "CITATION.txt"),
                 encoding="utf-8",
             ) as f:
                 self._cite = f.read()
 
         return self._cite
 
     @property
     def cite_collection(self):
         """Citation for the collection."""
         if not hasattr(self, "_cite_collection"):
             with open(
-                Path(_get_path_raw_dataset(), self.name, "CITATION_collection.txt"),
+                Path(self._path, "CITATION_collection.txt"),
                 encoding="utf-8",
             ) as f:
                 self._cite_collection = f.read()
 
         return self._cite_collection
 
     @property
     def metadata(self):
         """Metadata for the dataset."""
         if not hasattr(self, "_metadata"):
             with open(
-                Path(_get_path_raw_dataset(), self.name, "metadata.json"),
+                Path(self._path, "metadata.json"),
                 encoding="utf-8",
             ) as f:
                 self._metadata = json.load(f)
             with open(
-                Path(_get_path_raw_dataset(), self.name, "metadata_publication.json"),
+                Path(self._path, "metadata_publication.json"),
                 encoding="utf-8",
             ) as f:
                 self._metadata["publication"] = json.load(f)
 
             try:
                 with open(
-                    Path(
-                        _get_path_raw_dataset(), self.name, "metadata_collection.json"
-                    ),
+                    Path(self._path, "metadata_collection.json"),
                     encoding="utf-8",
                 ) as f:
                     self._metadata["collection"] = json.load(f)
             except FileNotFoundError:
                 pass
 
         return self._metadata
 
     @property
     def labels(self):
         """Metadata on the corresponding publication as work."""
         if not hasattr(self, "_labels"):
             self._labels = {}
             with open(
-                Path(_get_path_raw_dataset(), self.name, "labels.csv"),
+                Path(self._path, "labels.csv"),
                 newline="",
                 encoding="utf-8",
             ) as idfile:
                 reader = csv.DictReader(idfile)
                 for row in reader:
                     self._labels[row["openalex_id"]] = int(row["label_included"])
 
@@ -221,15 +223,15 @@
 
     def iter(self):
         """Iterate over the works in the dataset.
 
         Yields:
             Work: pyalex.Work object, label
         """
-        p_zipped_works = str(Path(_get_path_raw_dataset(), self.name, "works_*.zip"))
+        p_zipped_works = str(Path(self._path, "works_*.zip"))
 
         for f_work in glob.glob(p_zipped_works):
             with zipfile.ZipFile(f_work, "r") as z:
                 for work_set in z.namelist():
                     with z.open(work_set) as f:
                         d = json.loads(f.read())
```

### Comparing `synergy-dataset-1.1/synergy_dataset.egg-info/PKG-INFO` & `synergy-dataset-1.2/synergy_dataset.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synergy-dataset
-Version: 1.1
+Version: 1.2
 Summary: Python package for the SYNERGY dataset
 Author-email: Jonathan de Bruin <asreview@uu.nl>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `synergy-dataset-1.1/synergy_dataset.egg-info/SOURCES.txt` & `synergy-dataset-1.2/synergy_dataset.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `synergy-dataset-1.1/tests/test_synergy.py` & `synergy-dataset-1.2/tests/test_synergy.py`

 * *Files identical despite different names*

