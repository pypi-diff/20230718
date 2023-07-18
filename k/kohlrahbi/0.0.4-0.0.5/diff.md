# Comparing `tmp/kohlrahbi-0.0.4.tar.gz` & `tmp/kohlrahbi-0.0.5.tar.gz`

## Comparing `kohlrahbi-0.0.4.tar` & `kohlrahbi-0.0.5.tar`

### file list

```diff
@@ -1,43 +1,44 @@
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0     6576 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/README.md
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/requirements.in
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/requirements.txt
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/tox.ini
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/.github/dependabot.yml
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/.github/workflows/black.yml
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/.github/workflows/packaging_test.yml
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/.github/workflows/pythonlint.yml
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/.github/workflows/unittests.yml
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/_kohlrahbi_version.py
--rw-r--r--   0        0        0     7383 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/__init__.py
--rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/ahbfilefinder.py
--rw-r--r--   0        0        0     4299 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/all_known_pruefis.toml
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/collect_pruefis.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/logger.ini
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/logger.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/py.typed
--rw-r--r--   0        0        0     6134 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/read_functions.py
--rw-r--r--   0        0        0     5203 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/row_type_checker.py
--rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/seed.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/ahb/__init__.py
--rw-r--r--   0        0        0     5028 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/ahb/ahbsubtable.py
--rw-r--r--   0        0        0     7849 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/ahb/ahbtable.py
--rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/ahb/ahbtablerow.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/docxtablecells/__init__.py
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/docxtablecells/bedinungscell.py
--rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/docxtablecells/bodycell.py
--rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/docxtablecells/edifactstrukturcell.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/enums/__init__.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/enums/flat_ahb_row_type.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/enums/row_type.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/enums/row_type_color.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/unfoldedahb/__init__.py
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/unfoldedahb/unfoldedahbline.py
--rw-r--r--   0        0        0    15706 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/unfoldedahb/unfoldedahbtable.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/unfoldedahb/unfoldedahbtablemetadata.py
--rw-r--r--   0        0        0   861363 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/temp/test-fobar.docx
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/.gitignore
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     7690 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     6576 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/README.md
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/requirements.in
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/requirements.txt
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/tox.ini
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/.github/dependabot.yml
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/.github/workflows/black.yml
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/.github/workflows/packaging_test.yml
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/.github/workflows/pythonlint.yml
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/.github/workflows/unittests.yml
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/_kohlrahbi_version.py
+-rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/__init__.py
+-rw-r--r--   0        0        0     4325 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/ahbfilefinder.py
+-rw-r--r--   0        0        0     4299 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/all_known_pruefis.toml
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/collect_pruefis.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/logger.ini
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/logger.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/py.typed
+-rw-r--r--   0        0        0     6188 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/read_functions.py
+-rw-r--r--   0        0        0     5203 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/row_type_checker.py
+-rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/seed.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/ahb/__init__.py
+-rw-r--r--   0        0        0     5028 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/ahb/ahbsubtable.py
+-rw-r--r--   0        0        0     7849 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/ahb/ahbtable.py
+-rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/ahb/ahbtablerow.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/docxtablecells/__init__.py
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/docxtablecells/bedinungscell.py
+-rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/docxtablecells/bodycell.py
+-rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/docxtablecells/edifactstrukturcell.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/enums/__init__.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/enums/flat_ahb_row_type.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/enums/row_type.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/enums/row_type_color.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/unfoldedahb/__init__.py
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/unfoldedahb/unfoldedahbline.py
+-rw-r--r--   0        0        0    15722 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/unfoldedahb/unfoldedahbtable.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/src/kohlrahbi/unfoldedahb/unfoldedahbtablemetadata.py
+-rw-r--r--   0        0        0   861363 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/temp/test-fobar.docx
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     7738 2020-02-02 00:00:00.000000 kohlrahbi-0.0.5/PKG-INFO
```

### Comparing `kohlrahbi-0.0.4/.pre-commit-config.yaml` & `kohlrahbi-0.0.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.4/README.md` & `kohlrahbi-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.4/requirements.txt` & `kohlrahbi-0.0.5/requirements.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    pip-compile requirements.in
 #
-attrs==22.2.0
+attrs==23.1.0
     # via
     #   -r requirements.in
     #   maus
-click==8.1.3
+click==8.1.5
     # via
     #   -r requirements.in
     #   maus
 colorlog==6.7.0
     # via -r requirements.in
 et-xmlfile==1.1.0
     # via openpyxl
 lxml==4.9.2
     # via python-docx
 marshmallow==3.19.0
     # via maus
-maus==0.3.11
+maus==0.3.39
     # via -r requirements.in
 more-itertools==9.0.0
     # via maus
 numpy==1.24.1
     # via pandas
 openpyxl==3.1.2
     # via -r requirements.in
 packaging==22.0
     # via marshmallow
-pandas==2.0.0
+pandas==2.0.3
     # via -r requirements.in
 python-dateutil==2.8.2
     # via pandas
 python-docx==0.8.11
     # via -r requirements.in
 pytz==2023.3
     # via pandas
 six==1.16.0
     # via python-dateutil
-tomlkit==0.11.7
+tomlkit==0.11.8
     # via -r requirements.in
 tzdata==2023.3
     # via pandas
-xlsxwriter==3.0.9
+xlsxwriter==3.1.2
     # via -r requirements.in
```

### Comparing `kohlrahbi-0.0.4/tox.ini` & `kohlrahbi-0.0.5/tox.ini`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.4/.github/dependabot.yml` & `kohlrahbi-0.0.5/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.4/.github/workflows/black.yml` & `kohlrahbi-0.0.5/.github/workflows/black.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.4/.github/workflows/coverage.yml` & `kohlrahbi-0.0.5/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.4/.github/workflows/packaging_test.yml` & `kohlrahbi-0.0.5/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.4/.github/workflows/python-publish.yml` & `kohlrahbi-0.0.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.4/.github/workflows/pythonlint.yml` & `kohlrahbi-0.0.5/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.4/.github/workflows/unittests.yml` & `kohlrahbi-0.0.5/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.4/src/kohlrahbi/__init__.py` & `kohlrahbi-0.0.5/src/kohlrahbi/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 kohlrahbi is a package to scrape AHBs (in docx format)
 """
-
-
+import gc
 import re
 import sys
 from pathlib import Path
 from typing import Any
 
 import click
 import docx  # type:ignore[import]
@@ -120,15 +119,15 @@
 )
 @click.option(
     "--assume-yes",
     "-y",
     is_flag=True,
     help="Confirm all prompts automatically.",
 )
-# pylint: disable=too-many-branches
+# pylint: disable=too-many-branches, too-many-statements, too-many-locals
 def main(pruefis: list[str], input_path: Path, output_path: Path, file_type: list[str], assume_yes: bool):
     """
     A program to get a machine readable version of the AHBs docx files published by edi@energy.
     """
     check_python_version()
 
     if not assume_yes:
@@ -136,75 +135,90 @@
     else:
         if output_path.exists():
             click.secho(f"The output directory '{output_path}' exists already.", fg="yellow")
         else:
             output_path.mkdir(parents=True)
             click.secho(f"I created a new directory at {output_path}", fg="yellow")
 
-    if len(pruefis) == 0:
+    if not any(pruefis):
         click.secho("☝️ No pruefis were given. I will parse all known pruefis.", fg="yellow")
         pruefis = load_all_known_pruefis_from_file()
-    if len(file_type) == 0:
-        click.secho(
-            "ℹ You did not provide any value for the parameter --file-type. No files will be created.", fg="yellow"
-        )
+    if not any(file_type):
+        message = "ℹ You did not provide any value for the parameter --file-type. No files will be created."
+        click.secho(message, fg="yellow")
+        logger.warning(message)
+
     valid_pruefis: list[str] = get_valid_pruefis(list_of_pruefis=pruefis)
-    if valid_pruefis == []:
+    if not any(valid_pruefis):
         click.secho("⚠️ There are no valid pruefidentifkatoren.", fg="red")
         raise click.Abort()
 
     if len(valid_pruefis) != len(pruefis):
         click.secho("☝️ Not all given pruefidentifikatoren are valid.", fg="yellow")
         click.secho(f"I will continue with the following valid pruefis: {valid_pruefis}.", fg="yellow")
+    ahb_file_finder = AhbFileFinder.from_input_path(input_path=input_path)
+    path_to_document_mapping: dict[Path, docx.Document] = {}
 
     for pruefi in valid_pruefis:
-        logger.info("start looking for pruefi '%s'", pruefi)
-
-        ahb_file_finder = AhbFileFinder.from_input_path(input_path=input_path)
-
-        ahb_file_paths: list[Path] = ahb_file_finder.get_docx_files_which_may_contain_searched_pruefi(
-            searched_pruefi=pruefi
-        )
-
-        if len(ahb_file_paths) == 0:
-            logger.warning("No docx file was found for pruefi '%s'", pruefi)
-            continue
+        try:
+            logger.info("start looking for pruefi '%s'", pruefi)
 
-        for ahb_file_path in ahb_file_paths:
-            try:
-                doc = docx.Document(ahb_file_path)  # Creating word reader object.
-
-            except IOError as ioe:
-                logger.exception("There was an error opening the file '%s'", ahb_file_path, exc_info=True)
-                raise click.Abort() from ioe
-
-            logger.info("start reading docx file(s) '%s'", str(ahb_file_path))
-
-            ahb_table: AhbTable | None = get_ahb_table(
-                document=doc,
-                pruefi=pruefi,
+            ahb_file_paths: list[Path] = ahb_file_finder.get_docx_files_which_may_contain_searched_pruefi(
+                searched_pruefi=pruefi
             )
 
-            if ahb_table is None:
+            if not any(ahb_file_paths):
+                logger.warning("No docx file was found for pruefi '%s'", pruefi)
                 continue
 
-            if isinstance(ahb_table, AhbTable):
-                unfolded_ahb = UnfoldedAhb.from_ahb_table(ahb_table=ahb_table, pruefi=pruefi)
+            for ahb_file_path in ahb_file_paths:
+                if not (doc := path_to_document_mapping.get(ahb_file_path, None)):
+                    try:
+                        doc = docx.Document(ahb_file_path)  # Creating word reader object.
+                        path_to_document_mapping[ahb_file_path] = doc
+                        logger.debug("Saved %s document in cache", ahb_file_path)  # to not re-read it every time
+                    except IOError as ioe:
+                        logger.exception("There was an error opening the file '%s'", ahb_file_path, exc_info=True)
+                        raise click.Abort() from ioe
+
+                logger.info("start reading docx file '%s'", str(ahb_file_path))
+
+                ahb_table: AhbTable | None = get_ahb_table(
+                    document=doc,
+                    pruefi=pruefi,
+                )
+
+                if ahb_table is None:
+                    continue
 
-                if "xlsx" in file_type:
-                    logger.info("💾 Saving xlsx file %s", pruefi)
-                    unfolded_ahb.dump_xlsx(path_to_output_directory=output_path)
-
-                if "flatahb" in file_type:
-                    logger.info("💾 Saving flatahb file %s", pruefi)
-                    unfolded_ahb.dump_flatahb_json(output_directory_path=output_path)
-
-                if "csv" in file_type:
-                    logger.info("💾 Saving csv file %s", pruefi)
-                    unfolded_ahb.dump_csv(path_to_output_directory=output_path)
+                if isinstance(ahb_table, AhbTable):
+                    unfolded_ahb = UnfoldedAhb.from_ahb_table(ahb_table=ahb_table, pruefi=pruefi)
 
-                break
+                    if "xlsx" in file_type:
+                        logger.info("💾 Saving xlsx file %s", pruefi)
+                        unfolded_ahb.dump_xlsx(path_to_output_directory=output_path)
+
+                    if "flatahb" in file_type:
+                        logger.info("💾 Saving flatahb file %s", pruefi)
+                        unfolded_ahb.dump_flatahb_json(output_directory_path=output_path)
+
+                    if "csv" in file_type:
+                        logger.info("💾 Saving csv file %s", pruefi)
+                        unfolded_ahb.dump_csv(path_to_output_directory=output_path)
+                    break
+        except Exception as general_error:  # pylint:disable=broad-except
+            logger.exception(
+                "There was an uncaught error while processing the pruefi '%s': %s",
+                pruefi,
+                str(general_error),
+                exc_info=True,
+            )
+            continue
+        del ahb_table
+        if "unfolded_ahb" in locals():
+            del unfolded_ahb
+        gc.collect()
 
 
 if __name__ == "__main__":
     # the parameter arguments gets provided over the CLI
     main()  # pylint:disable=no-value-for-parameter
```

### Comparing `kohlrahbi-0.0.4/src/kohlrahbi/ahbfilefinder.py` & `kohlrahbi-0.0.5/src/kohlrahbi/ahbfilefinder.py`

 * *Files 10% similar despite different names*

```diff
@@ -85,9 +85,20 @@
         edifact_format = get_format_of_pruefidentifikator(searched_pruefi)
         if edifact_format is None:
             logger.exception("❌ There is no known format for the prüfi '%s'.", searched_pruefi)
             raise ValueError(f"There is no known format for the prüfi '{searched_pruefi}'.")
 
         self.filter_for_latest_ahb_docx_files()
         self.filter_docx_files_for_edifact_format(edifact_format=edifact_format)
-
+        if (
+            edifact_format == EdifactFormat.UTILMD
+            and searched_pruefi.startswith("11")
+            and all("202310" in path.name for path in self.paths_to_docx_files)
+        ):
+            logger.info(
+                # pylint:disable=line-too-long
+                "You searched for a UTILMD prüfi %s starting with the soon deprecated prefix '11' but all relevant files %s are valid from 2023-10 onwards. They won't contain any match.",
+                searched_pruefi,
+                ", ".join([path.name for path in self.paths_to_docx_files]),
+            )
+            return []
         return self.paths_to_docx_files
```

### Comparing `kohlrahbi-0.0.4/src/kohlrahbi/all_known_pruefis.toml` & `kohlrahbi-0.0.5/src/kohlrahbi/all_known_pruefis.toml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.4/src/kohlrahbi/collect_pruefis.py` & `kohlrahbi-0.0.5/src/kohlrahbi/collect_pruefis.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.4/src/kohlrahbi/read_functions.py` & `kohlrahbi-0.0.5/src/kohlrahbi/read_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,14 +91,15 @@
     searched_pruefi_is_found: bool = False
 
     # Iterate through the whole word document
     logger.info("Start iterating through paragraphs and tables")
     for item in get_all_paragraphs_and_tables(parent=document):
         # Check if we reached the end of the current AHB document and stop if it's true.
         if isinstance(item, Paragraph) and "Heading" in item.style.name and "Änderungshistorie" in item.text:
+            del seed
             return None
 
         # Check if there is just a text paragraph,
         if isinstance(item, Paragraph) and not "Heading" in item.style.name:
             continue
 
         if isinstance(item, Table) and does_the_table_contain_pruefidentifikatoren(table=item):
@@ -107,14 +108,15 @@
             logger.info("Found a table with the following pruefis: %s", seed.pruefidentifikatoren)
 
         we_reached_the_end_of_the_ahb_table_of_the_searched_pruefi: bool = (
             seed is not None and pruefi not in seed.pruefidentifikatoren and searched_pruefi_is_found
         )
 
         if we_reached_the_end_of_the_ahb_table_of_the_searched_pruefi:
+            del seed
             seed = None
             logger.info("🏁 We reached the end of the AHB table of the Prüfidentifikator '%s'", pruefi)
             break
 
         if isinstance(item, Table) and does_the_table_contain_pruefidentifikatoren(table=item):
             # check which pruefis
             seed = Seed.from_table(docx_table=item)
@@ -137,9 +139,9 @@
             ahb_table.append_ahb_sub_table(ahb_sub_table=ahb_sub_table)
 
     if ahb_table is None:
         logger.warning("⛔️ Your searched pruefi '%s' was not found in the provided files.\n", pruefi)
         return None
 
     ahb_table.sanitize()
-
+    del seed
     return ahb_table
```

### Comparing `kohlrahbi-0.0.4/src/kohlrahbi/row_type_checker.py` & `kohlrahbi-0.0.5/src/kohlrahbi/row_type_checker.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.4/src/kohlrahbi/seed.py` & `kohlrahbi-0.0.5/src/kohlrahbi/seed.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,50 +1,48 @@
 """
 This module provides a class to collect information which of need for all parsing functions
 """
 
-from typing import List
-
 from attrs import define
 from docx.table import Table  # type:ignore[import]
 from docx.text.paragraph import Paragraph  # type:ignore[import]
 
 from kohlrahbi.enums import RowType
 
 
-def get_tabstop_positions(paragraph: Paragraph) -> List[int]:
+def get_tabstop_positions(paragraph: Paragraph) -> list[int]:
     """Find all tabstop positions in a given paragraph.
 
     Mainly the tabstop positions of cells from the middle column are determined
 
     Args:
         paragraph (Paragraph):
 
     Returns:
         List[int]: All tabstop positions in the given paragraph
     """
-    tabstop_positions: List[int] = []
+    tabstop_positions: list[int] = []
     for tabstop in paragraph.paragraph_format.tab_stops:
         tabstop_positions.append(tabstop.position)
     return tabstop_positions
 
 
 # pylint: disable=too-few-public-methods
 @define
 class Seed:
     """
     helper class to store all values to extract the AHB and the final AHB as dataframe
     """
 
-    pruefidentifikatoren: List[str] = []
-    column_headers: List[str] = []
+    pruefidentifikatoren: list[str] = []
+    column_headers: list[str] = []
     edifact_struktur_left_indent_position: int = 0
     middle_cell_left_indent_position: int = 0
-    tabstop_positions: List[int] = []
-    last_two_row_types: List[RowType] = []
+    tabstop_positions: list[int] = []
+    last_two_row_types: list[RowType] = []
 
     # why this classmethod?
     # to decouple the data structure of Elixir from the input data
     # more information can be found on https://www.attrs.org/en/stable/init.html#initialization
     @classmethod
     def from_table(cls, docx_table: Table) -> "Seed":
         """Prepare DataFrame for a new table with new Prüfidentifikatoren
@@ -63,25 +61,25 @@
         edifact_struktur_left_indent_position = edifact_struktur_indicator_paragraph.paragraph_format.left_indent
 
         # middle cell
         middle_cell_indicator_paragraph = docx_table.cell(row_idx=4, col_idx=1).paragraphs[0]
         middle_cell_left_indent_position = middle_cell_indicator_paragraph.paragraph_format.left_indent
         tabstop_positions = get_tabstop_positions(middle_cell_indicator_paragraph)
 
-        base_column_names: List = [
+        base_column_names: list = [
             "Segment Gruppe",
             "Segment",
             "Datenelement",
             "Codes und Qualifier",
             "Beschreibung",
         ]
         columns = base_column_names + pruefidentifikatoren + ["Bedingung"]
 
         # Initialize help variables
-        last_two_row_types: List = [RowType.EMPTY, RowType.EMPTY]
+        last_two_row_types: list[RowType] = [RowType.EMPTY, RowType.EMPTY]
 
         return cls(
             pruefidentifikatoren=pruefidentifikatoren,
             column_headers=columns,
             edifact_struktur_left_indent_position=edifact_struktur_left_indent_position,
             middle_cell_left_indent_position=middle_cell_left_indent_position,
             tabstop_positions=tabstop_positions,
```

### Comparing `kohlrahbi-0.0.4/src/kohlrahbi/ahb/ahbsubtable.py` & `kohlrahbi-0.0.5/src/kohlrahbi/ahb/ahbsubtable.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.4/src/kohlrahbi/ahb/ahbtable.py` & `kohlrahbi-0.0.5/src/kohlrahbi/ahb/ahbtable.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.4/src/kohlrahbi/ahb/ahbtablerow.py` & `kohlrahbi-0.0.5/src/kohlrahbi/ahb/ahbtablerow.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.4/src/kohlrahbi/docxtablecells/bedinungscell.py` & `kohlrahbi-0.0.5/src/kohlrahbi/docxtablecells/bedinungscell.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.4/src/kohlrahbi/docxtablecells/bodycell.py` & `kohlrahbi-0.0.5/src/kohlrahbi/docxtablecells/bodycell.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 """
 This module contains the class BodyCell
 """
-from typing import List
-
 import attrs
 import pandas as pd
 from docx.table import _Cell  # type:ignore[import]
 from maus.reader.flat_ahb_reader import FlatAhbCsvReader
 
 from kohlrahbi.seed import get_tabstop_positions
 
@@ -19,15 +17,15 @@
     BodyCell contains all information and a method
     to extract dataelement/qualifier, the name of the dataelement
     as well as the conditions for each Prüfidentifikator.
     """
 
     table_cell: _Cell
     left_indent_position: int
-    indicator_tabstop_positions: List[int]
+    indicator_tabstop_positions: list[int]
 
     # I see why pylint is not happy about this many branches, but at the moment I have no clue how to avoid them.
     # pylint: disable=too-many-branches
     def parse(self, ahb_row_dataframe: pd.DataFrame) -> pd.DataFrame:
         """Parses a paragraph in the middle column and puts the information into the appropriate columns
 
         Args:
```

### Comparing `kohlrahbi-0.0.4/src/kohlrahbi/docxtablecells/edifactstrukturcell.py` & `kohlrahbi-0.0.5/src/kohlrahbi/docxtablecells/edifactstrukturcell.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.4/src/kohlrahbi/enums/row_type.py` & `kohlrahbi-0.0.5/src/kohlrahbi/enums/row_type.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.4/src/kohlrahbi/unfoldedahb/unfoldedahbline.py` & `kohlrahbi-0.0.5/src/kohlrahbi/unfoldedahb/unfoldedahbline.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.4/src/kohlrahbi/unfoldedahb/unfoldedahbtable.py` & `kohlrahbi-0.0.5/src/kohlrahbi/unfoldedahb/unfoldedahbtable.py`

 * *Files 1% similar despite different names*

```diff
@@ -309,15 +309,15 @@
                 "Segmentgruppe": unfolded_ahb_line.segment_gruppe,
                 "Segment": unfolded_ahb_line.segment,
                 "Datenelement": unfolded_ahb_line.datenelement,
                 "Code": unfolded_ahb_line.code,
                 "Qualifier": unfolded_ahb_line.qualifier,
                 "Beschreibung": unfolded_ahb_line.beschreibung,
                 "Bedingungsausdruck": unfolded_ahb_line.bedinung_ausdruck,
-                "Bedinung": unfolded_ahb_line.bedingung,
+                "Bedingung": unfolded_ahb_line.bedingung,
             }
             for unfolded_ahb_line in self.unfolded_ahb_lines
         ]
 
         df = pd.DataFrame(unfolded_ahb_lines)
         df.fillna(value="", inplace=True)
         return df
@@ -340,14 +340,15 @@
 
         df.to_csv(csv_output_directory_path / f"{self.meta_data.pruefidentifikator}.csv")
         logger.info(
             "The csv file for %s is saved at %s",
             self.meta_data.pruefidentifikator,
             csv_output_directory_path / f"{self.meta_data.pruefidentifikator}.csv",
         )
+        del df
 
     def dump_xlsx(self, path_to_output_directory: Path) -> None:
         """
         Dump a AHB table of a given pruefi into an excel file.
         The file will be stored in the directory:
             'path_to_output_directory/<edifact_format>/xlsx/<pruefidentifikator>.xlsx'
         """
```

### Comparing `kohlrahbi-0.0.4/temp/test-fobar.docx` & `kohlrahbi-0.0.5/temp/test-fobar.docx`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.4/.gitignore` & `kohlrahbi-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.4/pyproject.toml` & `kohlrahbi-0.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 [build-system]
 requires = ["hatchling>=1.8.0", "hatch-vcs", "hatch-fancy-pypi-readme"]
 build-backend = "hatchling.build"
 
 [project]
 name = "kohlrahbi"
 description = "Tool to generate machine readable files from AHB documents"
-license = { text = "MIT" }
+license = { text = "GPL" }
 requires-python = ">=3.11"
 authors = [{ name = "Kevin Krechan", email = "kevin.krechan@hochfrequenz.de" }]
 keywords = ["automation", "ahb", "bdew", "edi@energy"]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Environment :: Console",
   "Intended Audience :: Developers",
-  "License :: OSI Approved :: MIT License",
+  "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
   "attrs>=22.2.0",
```

### Comparing `kohlrahbi-0.0.4/PKG-INFO` & `kohlrahbi-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: kohlrahbi
-Version: 0.0.4
+Version: 0.0.5
 Summary: Tool to generate machine readable files from AHB documents
 Project-URL: Changelog, https://github.com/Hochfrequenz/kohlrahbi/releases
 Project-URL: Homepage, https://github.com/Hochfrequenz/kohlrahbi
 Author-email: Kevin Krechan <kevin.krechan@hochfrequenz.de>
-License: MIT
+License: GPL
+License-File: LICENSE
 Keywords: ahb,automation,bdew,edi@energy
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Requires-Dist: attrs>=22.2.0
 Requires-Dist: click>=8.0.0
```

