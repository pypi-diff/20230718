# Comparing `tmp/virtue-2023.7.2.tar.gz` & `tmp/virtue-2023.7.4.tar.gz`

## Comparing `virtue-2023.7.2.tar` & `virtue-2023.7.4.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 virtue-2023.7.2/.coveragerc
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 virtue-2023.7.2/.flake8
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 virtue-2023.7.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 virtue-2023.7.2/.readthedocs.yml
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 virtue-2023.7.2/.testr.conf
--rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 virtue-2023.7.2/noxfile.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 virtue-2023.7.2/.github/FUNDING.yml
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 virtue-2023.7.2/.github/SECURITY.md
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 virtue-2023.7.2/.github/dependabot.yml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 virtue-2023.7.2/.github/release.yml
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 virtue-2023.7.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 virtue-2023.7.2/docs/Makefile
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 virtue-2023.7.2/docs/api.rst
--rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 virtue-2023.7.2/docs/conf.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 virtue-2023.7.2/docs/index.rst
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 virtue-2023.7.2/docs/requirements.in
--rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 virtue-2023.7.2/docs/requirements.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 virtue-2023.7.2/docs/spelling-wordlist.txt
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/__init__.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/__main__.py
--rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/_cli.py
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/loaders.py
--rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/locators.py
--rw-r--r--   0        0        0    15025 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/reporters.py
--rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/runner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/tests/__init__.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/tests/test_cli.py
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/tests/test_loaders.py
--rw-r--r--   0        0        0     7246 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/tests/test_locators.py
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/tests/test_reporters.py
--rw-r--r--   0        0        0    12351 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/tests/test_runner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/tests/samples/__init__.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/tests/samples/dynamic_test.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/tests/samples/failures_and_errors.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/tests/samples/failures_and_unexpected_passes.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/tests/samples/mixin.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/tests/samples/module_for_TestLoaders.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/tests/samples/module_for_TestObjectLocator.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/tests/samples/module_with_exception.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/tests/samples/no_tests.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/tests/samples/one_expected_failure.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/tests/samples/one_expected_failure_mispassing.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/tests/samples/one_successful_test.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/tests/samples/one_unsuccessful_test.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/tests/samples/repeated_similar_output.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/tests/samples/subtests.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/tests/samples/success_and_warning.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/tests/samples/two_unsuccessful_tests.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 virtue-2023.7.2/COPYING
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 virtue-2023.7.2/README.rst
--rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 virtue-2023.7.2/pyproject.toml
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 virtue-2023.7.2/PKG-INFO
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 virtue-2023.7.4/.coveragerc
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 virtue-2023.7.4/.flake8
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 virtue-2023.7.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 virtue-2023.7.4/.readthedocs.yml
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 virtue-2023.7.4/.testr.conf
+-rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 virtue-2023.7.4/noxfile.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 virtue-2023.7.4/.github/FUNDING.yml
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 virtue-2023.7.4/.github/SECURITY.md
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 virtue-2023.7.4/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 virtue-2023.7.4/.github/release.yml
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 virtue-2023.7.4/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 virtue-2023.7.4/docs/Makefile
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 virtue-2023.7.4/docs/api.rst
+-rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 virtue-2023.7.4/docs/conf.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 virtue-2023.7.4/docs/index.rst
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 virtue-2023.7.4/docs/requirements.in
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 virtue-2023.7.4/docs/requirements.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 virtue-2023.7.4/docs/spelling-wordlist.txt
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/__init__.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/__main__.py
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/_cli.py
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/loaders.py
+-rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/locators.py
+-rw-r--r--   0        0        0    15271 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/reporters.py
+-rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/runner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/tests/__init__.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/tests/test_cli.py
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/tests/test_loaders.py
+-rw-r--r--   0        0        0     7246 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/tests/test_locators.py
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/tests/test_reporters.py
+-rw-r--r--   0        0        0    12351 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/tests/test_runner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/tests/samples/__init__.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/tests/samples/dynamic_test.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/tests/samples/failures_and_errors.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/tests/samples/failures_and_unexpected_passes.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/tests/samples/mixin.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/tests/samples/module_for_TestLoaders.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/tests/samples/module_for_TestObjectLocator.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/tests/samples/module_with_exception.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/tests/samples/no_tests.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/tests/samples/one_expected_failure.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/tests/samples/one_expected_failure_mispassing.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/tests/samples/one_successful_test.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/tests/samples/one_unsuccessful_test.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/tests/samples/repeated_similar_output.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/tests/samples/subtests.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/tests/samples/success_and_warning.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/tests/samples/two_unsuccessful_tests.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 virtue-2023.7.4/COPYING
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 virtue-2023.7.4/README.rst
+-rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 virtue-2023.7.4/pyproject.toml
+-rw-r--r--   0        0        0     3199 2020-02-02 00:00:00.000000 virtue-2023.7.4/PKG-INFO
```

### Comparing `virtue-2023.7.2/.flake8` & `virtue-2023.7.4/.flake8`

 * *Files identical despite different names*

### Comparing `virtue-2023.7.2/.pre-commit-config.yaml` & `virtue-2023.7.4/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -8,23 +8,23 @@
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
         args: [--fix, lf]
       - id: trailing-whitespace
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.0.277"
+    rev: "v0.0.278"
     hooks:
       - id: ruff
   - repo: https://github.com/PyCQA/isort
     rev: 5.12.0
     hooks:
       - id: isort
   - repo: https://github.com/psf/black
-    rev: 23.3.0
+    rev: 23.7.0
     hooks:
       - name: black
         id: black
         args: ["--line-length", "79"]
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: "v3.0.0"
     hooks:
```

### Comparing `virtue-2023.7.2/noxfile.py` & `virtue-2023.7.4/noxfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         if default:
             nox.options.sessions.append(kwargs.get("name", fn.__name__))
         return nox.session(**kwargs)(fn)
 
     return _session
 
 
-@session(python=["3.7", "3.8", "3.9", "3.10", "3.11", "pypy3"])
+@session(python=["3.8", "3.9", "3.10", "3.11", "3.12", "pypy3"])
 def tests(session):
     session.install(ROOT)
     if session.posargs and session.posargs[0] == "coverage":
         if len(session.posargs) > 1 and session.posargs[1] == "github":
             posargs = session.posargs[2:]
             github = os.environ["GITHUB_STEP_SUMMARY"]
         else:
@@ -47,17 +47,17 @@
                     "--format=markdown",
                     stdout=summary,
                 )
     else:
         session.run("virtue", *session.posargs, "virtue")
 
 
-@session(python=["3.7", "3.8", "3.9", "3.10", "3.11", "pypy3"])
+@session(python=["3.8", "3.9", "3.10", "3.11", "3.12", "pypy3"])
 def audit(session):
-    session.install("pip_audit", ROOT)
+    session.install("pip-audit", ROOT)
     session.run("python", "-m", "pip_audit")
 
 
 @session(tags=["build"])
 def build(session):
     session.install("build", "twine")
     with TemporaryDirectory() as tmpdir:
```

### Comparing `virtue-2023.7.2/.github/SECURITY.md` & `virtue-2023.7.4/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `virtue-2023.7.2/.github/workflows/ci.yml` & `virtue-2023.7.4/.github/workflows/ci.yml`

 * *Files 3% similar despite different names*

```diff
@@ -61,15 +61,22 @@
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
         run: nox -s "${{ matrix.noxenv }}" -- ${{ matrix.posargs }}
 
   packaging:
     needs: ci
```

### Comparing `virtue-2023.7.2/docs/Makefile` & `virtue-2023.7.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `virtue-2023.7.2/docs/conf.py` & `virtue-2023.7.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `virtue-2023.7.2/docs/requirements.txt` & `virtue-2023.7.4/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `virtue-2023.7.2/virtue/_cli.py` & `virtue-2023.7.4/virtue/_cli.py`

 * *Files identical despite different names*

### Comparing `virtue-2023.7.2/virtue/loaders.py` & `virtue-2023.7.4/virtue/loaders.py`

 * *Files identical despite different names*

### Comparing `virtue-2023.7.2/virtue/locators.py` & `virtue-2023.7.4/virtue/locators.py`

 * *Files identical despite different names*

### Comparing `virtue-2023.7.2/virtue/reporters.py` & `virtue-2023.7.4/virtue/reporters.py`

 * *Files 4% similar despite different names*

```diff
@@ -305,14 +305,17 @@
 
     def addUnexpectedSuccess(self, test):  # noqa: D102
         self.unexpected_successes += 1
 
     def addSuccess(self, test):  # noqa: D102
         self.successes += 1
 
+    def addDuration(self, test, elapsed):  # noqa: D102
+        pass
+
     def addSubTest(self, test, subtest, outcome):  # noqa: D102
         if outcome is None:
             self.subtest_successes += 1
         elif issubclass(outcome[0], test.failureException):
             self.subtest_failures += 1
         else:
             self.subtest_errors += 1
@@ -389,14 +392,17 @@
 
     def addUnexpectedSuccess(self, test):  # noqa: D102
         self.unexpected_successes = self.unexpected_successes.append(test)
 
     def addSuccess(self, test):  # noqa: D102
         self.successes = self.successes.append(test)
 
+    def addDuration(self, test, elapsed):  # noqa: D102
+        pass
+
     def addSubTest(self, test, subtest, outcome):  # noqa: D102
         if outcome is None:
             self.subtest_successes = self.subtest_successes.set(
                 test,
                 self.subtest_successes.get(test, v()).append(subtest),
             )
         elif issubclass(outcome[0], test.failureException):
@@ -486,14 +492,17 @@
             self.outputter.test_unexpectedly_succeeded(test) or "",
         )
 
     def addSuccess(self, test):  # noqa: D102
         self.recorder.addSuccess(test)
         self.stream.writelines(self.outputter.test_succeeded(test) or "")
 
+    def addDuration(self, test, elapsed):  # noqa: D102
+        self.recorder.addDuration(test, elapsed)
+
     def addSubTest(self, test, subtest, outcome):  # noqa: D102
         self.recorder.addSubTest(test, subtest, outcome)
         if outcome is None:
             output = self.outputter.subtest_succeeded(test, subtest)
         elif issubclass(outcome[0], test.failureException):
             output = self.outputter.subtest_failed(test, subtest, outcome)
         else:
```

### Comparing `virtue-2023.7.2/virtue/runner.py` & `virtue-2023.7.4/virtue/runner.py`

 * *Files identical despite different names*

### Comparing `virtue-2023.7.2/virtue/tests/test_cli.py` & `virtue-2023.7.4/virtue/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `virtue-2023.7.2/virtue/tests/test_loaders.py` & `virtue-2023.7.4/virtue/tests/test_loaders.py`

 * *Files identical despite different names*

### Comparing `virtue-2023.7.2/virtue/tests/test_locators.py` & `virtue-2023.7.4/virtue/tests/test_locators.py`

 * *Files identical despite different names*

### Comparing `virtue-2023.7.2/virtue/tests/test_reporters.py` & `virtue-2023.7.4/virtue/tests/test_reporters.py`

 * *Files identical despite different names*

### Comparing `virtue-2023.7.2/virtue/tests/test_runner.py` & `virtue-2023.7.4/virtue/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `virtue-2023.7.2/virtue/tests/samples/subtests.py` & `virtue-2023.7.4/virtue/tests/samples/subtests.py`

 * *Files identical despite different names*

### Comparing `virtue-2023.7.2/COPYING` & `virtue-2023.7.4/COPYING`

 * *Files identical despite different names*

### Comparing `virtue-2023.7.2/README.rst` & `virtue-2023.7.4/README.rst`

 * *Files identical despite different names*

### Comparing `virtue-2023.7.2/pyproject.toml` & `virtue-2023.7.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -6,52 +6,51 @@
 source = "vcs"
 
 [project]
 name = "virtue"
 description = "After trial comes virtue. A test runner for good."
 readme = "README.rst"
 license = {text = "MIT"}
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 keywords = ["testing", "tests", "test runner", "unittest"]
 authors = [
   {email = "Julian+Virtue@GrayVines.com"},
   {name = "Julian Berman"},
 ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dynamic = ["version"]
 dependencies = [
-  "attrs>=19",
+  "attrs>=22.2.0",
   "click",
   "colorama",
   "pyrsistent",
   "twisted",
 
-  "importlib_metadata;python_version<'3.8'",
   "pkgutil_resolve_name>=1.3.10;python_version<'3.9'",
 ]
 
 [project.scripts]
 virtue = "virtue._cli:main"
 
 [project.urls]
-Homepage = "https://github.com/Julian/Virtue"
 Documentation = "https://virtue.readthedocs.io/"
+Homepage = "https://github.com/Julian/Virtue"
 Issues = "https://github.com/Julian/Virtue/issues/"
 Funding = "https://github.com/sponsors/Julian"
 Source = "https://github.com/Julian/Virtue"
 
 [tool.coverage.html]
 show_contexts = true
 skip_covered = false
```

### Comparing `virtue-2023.7.2/PKG-INFO` & `virtue-2023.7.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 Metadata-Version: 2.1
 Name: virtue
-Version: 2023.7.2
+Version: 2023.7.4
 Summary: After trial comes virtue. A test runner for good.
-Project-URL: Homepage, https://github.com/Julian/Virtue
 Project-URL: Documentation, https://virtue.readthedocs.io/
+Project-URL: Homepage, https://github.com/Julian/Virtue
 Project-URL: Issues, https://github.com/Julian/Virtue/issues/
 Project-URL: Funding, https://github.com/sponsors/Julian
 Project-URL: Source, https://github.com/Julian/Virtue
 Author: Julian Berman
 Author-email: Julian+Virtue@GrayVines.com
 License: MIT
 License-File: COPYING
 Keywords: test runner,testing,tests,unittest
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
-Requires-Dist: attrs>=19
+Requires-Python: >=3.8
+Requires-Dist: attrs>=22.2.0
 Requires-Dist: click
 Requires-Dist: colorama
-Requires-Dist: importlib-metadata; python_version < '3.8'
 Requires-Dist: pkgutil-resolve-name>=1.3.10; python_version < '3.9'
 Requires-Dist: pyrsistent
 Requires-Dist: twisted
 Description-Content-Type: text/x-rst
 
 ======
 Virtue
```

