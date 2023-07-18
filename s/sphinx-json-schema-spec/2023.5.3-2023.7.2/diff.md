# Comparing `tmp/sphinx_json_schema_spec-2023.5.3.tar.gz` & `tmp/sphinx_json_schema_spec-2023.7.2.tar.gz`

## Comparing `sphinx_json_schema_spec-2023.5.3.tar` & `sphinx_json_schema_spec-2023.7.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.3/.flake8
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.3/.readthedocs.yml
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.3/noxfile.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.3/.github/FUNDING.yml
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.3/.github/SECURITY.md
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.3/.github/dependabot.yml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.3/.github/release.yml
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.3/.github/workflows/ci.yml
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.3/docs/Makefile
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.3/docs/conf.py
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.3/docs/index.rst
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.3/docs/requirements.in
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.3/docs/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.3/docs/spelling-wordlist.txt
--rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.3/sphinx_json_schema_spec/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.3/sphinx_json_schema_spec/tests/__init__.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.3/sphinx_json_schema_spec/tests/test_sphinx.py
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.3/.gitignore
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.3/COPYING
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.3/README.rst
--rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.3/pyproject.toml
--rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.3/PKG-INFO
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.2/.flake8
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.2/.readthedocs.yml
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.2/noxfile.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.2/.github/FUNDING.yml
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.2/.github/SECURITY.md
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.2/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.2/.github/release.yml
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.2/docs/Makefile
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.2/docs/conf.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.2/docs/index.rst
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.2/docs/requirements.in
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.2/docs/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.2/docs/spelling-wordlist.txt
+-rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.2/sphinx_json_schema_spec/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.2/sphinx_json_schema_spec/tests/__init__.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.2/sphinx_json_schema_spec/tests/test_sphinx.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.2/.gitignore
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.2/COPYING
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.2/README.rst
+-rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.2/pyproject.toml
+-rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.2/PKG-INFO
```

### Comparing `sphinx_json_schema_spec-2023.5.3/.pre-commit-config.yaml` & `sphinx_json_schema_spec-2023.7.2/.pre-commit-config.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -14,10 +14,10 @@
         args: [--fix, lf]
       - id: trailing-whitespace
   - repo: https://github.com/PyCQA/isort
     rev: 5.12.0
     hooks:
       - id: isort
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: "v3.0.0-alpha.9-for-vscode"
+    rev: "v3.0.0"
     hooks:
       - id: prettier
```

### Comparing `sphinx_json_schema_spec-2023.5.3/noxfile.py` & `sphinx_json_schema_spec-2023.7.2/noxfile.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from pathlib import Path
+from tempfile import TemporaryDirectory
 
 import nox
 
 ROOT = Path(__file__).parent
 PYPROJECT = ROOT / "pyproject.toml"
 DOCS = ROOT / "docs"
 PACKAGE = ROOT / "sphinx_json_schema_spec"
@@ -30,25 +31,18 @@
 def audit(session):
     session.install("pip-audit", ROOT)
     session.run("python", "-m", "pip_audit")
 
 
 @session(tags=["build"])
 def build(session):
-    session.install("build")
-    tmpdir = session.create_tmp()
-    session.run("python", "-m", "build", ROOT, "--outdir", tmpdir)
-
-
-@session(tags=["style"])
-def readme(session):
     session.install("build", "twine")
-    tmpdir = session.create_tmp()
-    session.run("python", "-m", "build", ROOT, "--outdir", tmpdir)
-    session.run("python", "-m", "twine", "check", tmpdir + "/*")
+    with TemporaryDirectory() as tmpdir:
+        session.run("python", "-m", "build", ROOT, "--outdir", tmpdir)
+        session.run("twine", "check", "--strict", tmpdir + "/*")
 
 
 @session(tags=["style"])
 def style(session):
     session.install("ruff")
     session.run("ruff", "check", ROOT)
 
@@ -71,28 +65,29 @@
             "man",
             "spelling",
         ]
     ],
 )
 def docs(session, builder):
     session.install("-r", DOCS / "requirements.txt")
-    tmpdir = Path(session.create_tmp())
-    argv = ["-n", "-T", "-W"]
-    if builder != "spelling":
-        argv += ["-q"]
-    session.run(
-        "python",
-        "-m",
-        "sphinx",
-        "-b",
-        builder,
-        DOCS,
-        tmpdir / builder,
-        *argv,
-    )
+    with TemporaryDirectory() as tmpdir_str:
+        tmpdir = Path(tmpdir_str)
+        argv = ["-n", "-T", "-W"]
+        if builder != "spelling":
+            argv += ["-q"]
+        session.run(
+            "python",
+            "-m",
+            "sphinx",
+            "-b",
+            builder,
+            DOCS,
+            tmpdir / builder,
+            *argv,
+        )
 
 
 @session(tags=["docs", "style"], name="docs(style)")
 def docs_style(session):
     session.install(
         "doc8",
         "pygments",
```

### Comparing `sphinx_json_schema_spec-2023.5.3/.github/SECURITY.md` & `sphinx_json_schema_spec-2023.7.2/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.5.3/.github/workflows/ci.yml` & `sphinx_json_schema_spec-2023.7.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.5.3/docs/Makefile` & `sphinx_json_schema_spec-2023.7.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.5.3/docs/conf.py` & `sphinx_json_schema_spec-2023.7.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.5.3/docs/index.rst` & `sphinx_json_schema_spec-2023.7.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.5.3/docs/requirements.txt` & `sphinx_json_schema_spec-2023.7.2/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.5.3/sphinx_json_schema_spec/__init__.py` & `sphinx_json_schema_spec-2023.7.2/sphinx_json_schema_spec/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.5.3/.gitignore` & `sphinx_json_schema_spec-2023.7.2/.gitignore`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.5.3/COPYING` & `sphinx_json_schema_spec-2023.7.2/COPYING`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.5.3/README.rst` & `sphinx_json_schema_spec-2023.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.5.3/pyproject.toml` & `sphinx_json_schema_spec-2023.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.5.3/PKG-INFO` & `sphinx_json_schema_spec-2023.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx_json_schema_spec
-Version: 2023.5.3
+Version: 2023.7.2
 Summary: Sphinx support for the JSON Schema specifications
 Project-URL: Documentation, https://sphinx-json-schema-spec.readthedocs.io/
 Project-URL: Homepage, https://github.com/python-jsonschema/sphinx-json-schema-spec
 Project-URL: Issues, https://github.com/python-jsonschema/sphinx-json-schema-spec/issues/
 Project-URL: Funding, https://github.com/sponsors/Julian
 Project-URL: Source, https://github.com/python-jsonschema/sphinx-json-schema-spec
 Author: Julian Berman
```

