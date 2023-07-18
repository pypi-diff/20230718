# Comparing `tmp/regret-2023.7.2.tar.gz` & `tmp/regret-2023.7.5.tar.gz`

## Comparing `regret-2023.7.2.tar` & `regret-2023.7.5.tar`

### file list

```diff
@@ -1,40 +1,39 @@
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 regret-2023.7.2/.flake8
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 regret-2023.7.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 regret-2023.7.2/.readthedocs.yml
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 regret-2023.7.2/.testr.conf
--rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 regret-2023.7.2/CONTRIBUTING.rst
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 regret-2023.7.2/MANIFEST.in
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 regret-2023.7.2/noxfile.py
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 regret-2023.7.2/test-requirements.in
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 regret-2023.7.2/test-requirements.txt
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 regret-2023.7.2/.github/SECURITY.md
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 regret-2023.7.2/.github/dependabot.yml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 regret-2023.7.2/.github/release.yml
--rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 regret-2023.7.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 regret-2023.7.2/docs/Makefile
--rw-r--r--   0        0        0    11979 2020-02-02 00:00:00.000000 regret-2023.7.2/docs/before-you-deprecate.rst
--rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 regret-2023.7.2/docs/compatibility.rst
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 regret-2023.7.2/docs/conf.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 regret-2023.7.2/docs/index.rst
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 regret-2023.7.2/docs/requirements.in
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 regret-2023.7.2/docs/requirements.txt
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 regret-2023.7.2/docs/spelling_wordlist.txt
--rw-r--r--   0        0        0     7387 2020-02-02 00:00:00.000000 regret-2023.7.2/docs/what-you-can-deprecate.rst
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 regret-2023.7.2/docs/api/modules.rst
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 regret-2023.7.2/docs/api/regret.rst
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 regret-2023.7.2/regret/__init__.py
--rw-r--r--   0        0        0     9407 2020-02-02 00:00:00.000000 regret-2023.7.2/regret/_api.py
--rw-r--r--   0        0        0     5651 2020-02-02 00:00:00.000000 regret-2023.7.2/regret/_inspect.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 regret-2023.7.2/regret/_sphinx.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 regret-2023.7.2/regret/_warnings.py
--rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 regret-2023.7.2/regret/emitted.py
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 regret-2023.7.2/regret/testing.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 regret-2023.7.2/regret/typing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 regret-2023.7.2/regret/tests/__init__.py
--rw-r--r--   0        0        0    62906 2020-02-02 00:00:00.000000 regret-2023.7.2/regret/tests/test_api.py
--rw-r--r--   0        0        0     9570 2020-02-02 00:00:00.000000 regret-2023.7.2/regret/tests/test_integration.py
--rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 regret-2023.7.2/regret/tests/test_testing.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 regret-2023.7.2/COPYING
--rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 regret-2023.7.2/README.rst
--rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 regret-2023.7.2/pyproject.toml
--rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 regret-2023.7.2/PKG-INFO
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 regret-2023.7.5/.flake8
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 regret-2023.7.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 regret-2023.7.5/.readthedocs.yml
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 regret-2023.7.5/.testr.conf
+-rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 regret-2023.7.5/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 regret-2023.7.5/noxfile.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 regret-2023.7.5/test-requirements.in
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 regret-2023.7.5/test-requirements.txt
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 regret-2023.7.5/.github/SECURITY.md
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 regret-2023.7.5/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 regret-2023.7.5/.github/release.yml
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 regret-2023.7.5/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 regret-2023.7.5/docs/Makefile
+-rw-r--r--   0        0        0    11979 2020-02-02 00:00:00.000000 regret-2023.7.5/docs/before-you-deprecate.rst
+-rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 regret-2023.7.5/docs/compatibility.rst
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 regret-2023.7.5/docs/conf.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 regret-2023.7.5/docs/index.rst
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 regret-2023.7.5/docs/requirements.in
+-rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 regret-2023.7.5/docs/requirements.txt
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 regret-2023.7.5/docs/spelling_wordlist.txt
+-rw-r--r--   0        0        0     7387 2020-02-02 00:00:00.000000 regret-2023.7.5/docs/what-you-can-deprecate.rst
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 regret-2023.7.5/docs/api/modules.rst
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 regret-2023.7.5/docs/api/regret.rst
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 regret-2023.7.5/regret/__init__.py
+-rw-r--r--   0        0        0     9407 2020-02-02 00:00:00.000000 regret-2023.7.5/regret/_api.py
+-rw-r--r--   0        0        0     5651 2020-02-02 00:00:00.000000 regret-2023.7.5/regret/_inspect.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 regret-2023.7.5/regret/_sphinx.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 regret-2023.7.5/regret/_warnings.py
+-rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 regret-2023.7.5/regret/emitted.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 regret-2023.7.5/regret/testing.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 regret-2023.7.5/regret/typing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 regret-2023.7.5/regret/tests/__init__.py
+-rw-r--r--   0        0        0    62906 2020-02-02 00:00:00.000000 regret-2023.7.5/regret/tests/test_api.py
+-rw-r--r--   0        0        0     9570 2020-02-02 00:00:00.000000 regret-2023.7.5/regret/tests/test_integration.py
+-rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 regret-2023.7.5/regret/tests/test_testing.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 regret-2023.7.5/COPYING
+-rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 regret-2023.7.5/README.rst
+-rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 regret-2023.7.5/pyproject.toml
+-rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 regret-2023.7.5/PKG-INFO
```

### Comparing `regret-2023.7.2/.pre-commit-config.yaml` & `regret-2023.7.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `regret-2023.7.2/CONTRIBUTING.rst` & `regret-2023.7.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `regret-2023.7.2/noxfile.py` & `regret-2023.7.5/noxfile.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,68 +1,86 @@
 from pathlib import Path
+from tempfile import TemporaryDirectory
+import os
 
 import nox
 
 ROOT = Path(__file__).parent
 PYPROJECT = ROOT / "pyproject.toml"
 DOCS = ROOT / "docs"
 PACKAGE = ROOT / "regret"
+CONTRIBUTING = ROOT / "CONTRIBUTING.rst"
 
 
 nox.options.sessions = []
 
 
 def session(default=True, **kwargs):
     def _session(fn):
         if default:
             nox.options.sessions.append(kwargs.get("name", fn.__name__))
         return nox.session(**kwargs)(fn)
 
     return _session
 
 
-@session(python=["3.8", "3.9", "3.10", "3.11", "pypy3"])
+@session(python=["3.8", "3.9", "3.10", "3.11", "3.12", "pypy3"])
 def tests(session):
     session.install(ROOT, "virtue", "-r", ROOT / "test-requirements.txt")
-    if session.posargs == ["coverage"]:
+
+    if session.posargs and session.posargs[0] == "coverage":
+        if len(session.posargs) > 1 and session.posargs[1] == "github":
+            github = os.environ["GITHUB_STEP_SUMMARY"]
+        else:
+            github = None
+
         session.install("coverage[toml]")
         session.run("coverage", "run", "-m", "virtue", PACKAGE)
-        session.run("coverage", "report")
+        if github is None:
+            session.run("coverage", "report")
+        else:
+            with open(github, "a") as summary:
+                summary.write("### Coverage\n\n")
+                summary.flush()  # without a flush, output seems out of order.
+                session.run(
+                    "coverage",
+                    "report",
+                    "--format=markdown",
+                    stdout=summary,
+                )
     else:
         session.run("python", "-m", "virtue", *session.posargs, "regret")
 
 
 @session()
 def pytest_tests(session):
     session.install(ROOT, "pytest", "-r", ROOT / "test-requirements.txt")
     session.run("pytest", *session.posargs, PACKAGE)
 
 
 @session()
 def audit(session):
-    session.install("pip_audit", ROOT)
+    session.install("pip-audit", ROOT)
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
     session.install("build", "docutils", "twine")
-    tmpdir = session.create_tmp()
-    session.run("python", "-m", "build", ROOT, "--outdir", tmpdir)
-    session.run("python", "-m", "twine", "check", tmpdir + "/*")
-
-    CONTRIBUTING = ROOT / "CONTRIBUTING.rst"
-    session.run("rst2html5.py", "--halt=warning", CONTRIBUTING, "/dev/null")
+    with TemporaryDirectory() as tmpdir:
+        session.run("python", "-m", "build", ROOT, "--outdir", tmpdir)
+        session.run("twine", "check", "--strict", tmpdir + "/*")
+        session.run(
+            "python",
+            "-m",
+            "docutils",
+            "--strict",
+            CONTRIBUTING,
+            os.devnull,
+        )
 
 
 @session(tags=["style"])
 def style(session):
     session.install("ruff")
     session.run("ruff", "check", ROOT)
 
@@ -85,28 +103,29 @@
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

### Comparing `regret-2023.7.2/test-requirements.txt` & `regret-2023.7.5/test-requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --resolver=backtracking test-requirements.in
+#    pip-compile test-requirements.in
 #
 attrs==23.1.0
     # via
     #   automat
     #   twisted
 automat==22.10.0
     # via twisted
```

### Comparing `regret-2023.7.2/.github/SECURITY.md` & `regret-2023.7.5/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `regret-2023.7.2/.github/workflows/ci.yml` & `regret-2023.7.5/.github/workflows/ci.yml`

 * *Files 20% similar despite different names*

```diff
@@ -44,33 +44,43 @@
     needs: list
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [macos-latest, ubuntu-latest]
         noxenv: ${{ fromJson(needs.list.outputs.noxenvs) }}
+        posargs: [""]
+        include:
+          - os: ubuntu-latest
+            noxenv: tests-3.11
+            posargs: coverage github
 
     steps:
       - uses: actions/checkout@v3
       - name: Install dependencies
-        run: >
-          sudo apt-get update &&
-          sudo apt-get install -y libenchant-2-dev
+        run: sudo apt-get update && sudo apt-get install -y libenchant-2-dev
         if: runner.os == 'Linux' && startsWith(matrix.noxenv, 'docs')
       - name: Install dependencies
         run: brew install enchant
         if: runner.os == 'macOS' && startsWith(matrix.noxenv, 'docs')
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
-          python-version: "3.x"
+          python-version: |
+            3.8
+            3.9
+            3.10
+            3.11
+            3.12
+            pypy3.10
+          allow-prereleases: true
       - name: Set up nox
         uses: wntrblm/nox@2023.04.22
       - name: Run nox
-        run: nox -s "${{ matrix.noxenv }}"
+        run: nox -s "${{ matrix.noxenv }}" -- ${{ matrix.posargs }}
 
   packaging:
     needs: ci
     runs-on: ubuntu-latest
     environment:
       name: PyPI
       url: https://pypi.org/p/regret
```

### Comparing `regret-2023.7.2/docs/Makefile` & `regret-2023.7.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `regret-2023.7.2/docs/before-you-deprecate.rst` & `regret-2023.7.5/docs/before-you-deprecate.rst`

 * *Files identical despite different names*

### Comparing `regret-2023.7.2/docs/compatibility.rst` & `regret-2023.7.5/docs/compatibility.rst`

 * *Files identical despite different names*

### Comparing `regret-2023.7.2/docs/conf.py` & `regret-2023.7.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `regret-2023.7.2/docs/requirements.txt` & `regret-2023.7.5/docs/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --config=pyproject.toml --resolver=backtracking docs/requirements.in
+#    pip-compile --config=pyproject.toml docs/requirements.in
 #
 alabaster==0.7.13
     # via sphinx
 attrs==23.1.0
     # via regret
 babel==2.12.1
     # via sphinx
 beautifulsoup4==4.12.2
     # via furo
 certifi==2023.5.7
     # via requests
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via requests
 contourpy==1.1.0
     # via matplotlib
 cycler==0.11.0
     # via matplotlib
 docutils==0.20.1
     # via sphinx
-fonttools==4.40.0
+fonttools==4.41.0
     # via matplotlib
 furo==2023.5.20
     # via -r docs/requirements.in
 idna==3.4
     # via requests
 imagesize==1.4.1
     # via sphinx
@@ -34,15 +34,15 @@
     # via sphinx
 kiwisolver==1.4.4
     # via matplotlib
 markupsafe==2.1.3
     # via jinja2
 matplotlib==3.7.2
     # via sphinxext-opengraph
-numpy==1.25.0
+numpy==1.25.1
     # via
     #   contourpy
     #   matplotlib
 packaging==23.1
     # via
     #   matplotlib
     #   sphinx
@@ -75,15 +75,15 @@
     # via
     #   -r docs/requirements.in
     #   furo
     #   sphinx-basic-ng
     #   sphinx-copybutton
     #   sphinxcontrib-spelling
     #   sphinxext-opengraph
-sphinx-basic-ng==1.0.0b1
+sphinx-basic-ng==1.0.0b2
     # via furo
 sphinx-copybutton==0.5.2
     # via -r docs/requirements.in
 sphinxcontrib-applehelp==1.0.4
     # via sphinx
 sphinxcontrib-devhelp==1.0.2
     # via sphinx
```

### Comparing `regret-2023.7.2/docs/what-you-can-deprecate.rst` & `regret-2023.7.5/docs/what-you-can-deprecate.rst`

 * *Files identical despite different names*

### Comparing `regret-2023.7.2/docs/api/regret.rst` & `regret-2023.7.5/docs/api/regret.rst`

 * *Files identical despite different names*

### Comparing `regret-2023.7.2/regret/_api.py` & `regret-2023.7.5/regret/_api.py`

 * *Files identical despite different names*

### Comparing `regret-2023.7.2/regret/_inspect.py` & `regret-2023.7.5/regret/_inspect.py`

 * *Files identical despite different names*

### Comparing `regret-2023.7.2/regret/_sphinx.py` & `regret-2023.7.5/regret/_sphinx.py`

 * *Files identical despite different names*

### Comparing `regret-2023.7.2/regret/emitted.py` & `regret-2023.7.5/regret/emitted.py`

 * *Files identical despite different names*

### Comparing `regret-2023.7.2/regret/testing.py` & `regret-2023.7.5/regret/testing.py`

 * *Files identical despite different names*

### Comparing `regret-2023.7.2/regret/typing.py` & `regret-2023.7.5/regret/typing.py`

 * *Files identical despite different names*

### Comparing `regret-2023.7.2/regret/tests/test_api.py` & `regret-2023.7.5/regret/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `regret-2023.7.2/regret/tests/test_integration.py` & `regret-2023.7.5/regret/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `regret-2023.7.2/regret/tests/test_testing.py` & `regret-2023.7.5/regret/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `regret-2023.7.2/COPYING` & `regret-2023.7.5/COPYING`

 * *Files identical despite different names*

### Comparing `regret-2023.7.2/README.rst` & `regret-2023.7.5/README.rst`

 * *Files identical despite different names*

### Comparing `regret-2023.7.2/pyproject.toml` & `regret-2023.7.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `regret-2023.7.2/PKG-INFO` & `regret-2023.7.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regret
-Version: 2023.7.2
+Version: 2023.7.5
 Summary: You made a thing, but now you wish it'd go away... Deprecations, a love story.
 Project-URL: Documentation, https://regret.readthedocs.io/
 Project-URL: Homepage, https://github.com/Julian/regret
 Project-URL: Issues, https://github.com/Julian/regret/issues/
 Project-URL: Funding, https://github.com/sponsors/Julian
 Project-URL: Source, https://github.com/Julian/regret
 Author: Julian Berman
```

