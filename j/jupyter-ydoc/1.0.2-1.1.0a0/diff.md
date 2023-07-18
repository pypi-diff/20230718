# Comparing `tmp/jupyter_ydoc-1.0.2.tar.gz` & `tmp/jupyter_ydoc-1.1.0a0.tar.gz`

## Comparing `jupyter_ydoc-1.0.2.tar` & `jupyter_ydoc-1.1.0a0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.2/.licenserc.yaml
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.2/.yarnrc.yml
--rw-r--r--   0        0        0    52487 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.2/CHANGELOG.md
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.2/lerna.json
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.2/package.json
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.2/pytest.ini
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.2/readthedocs.yml
--rw-r--r--   0        0        0   185553 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.2/yarn.lock
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.2/.github/dependabot.yml
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.2/.github/workflows/auto_author_assign.yml
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.2/.github/workflows/check-release.yml
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.2/.github/workflows/enforce-label.yml
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.2/.github/workflows/license-header.yml
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.2/.github/workflows/prep-release.yml
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.2/.github/workflows/publish-release.yml
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.2/.github/workflows/test.yml
--rwxr-xr-x   0        0        0  2212925 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.2/.yarn/releases/yarn-3.4.1.cjs
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.2/docs/Makefile
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.2/docs/make.bat
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.2/docs/source/conf.py
--rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.2/docs/source/custom.md
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.2/docs/source/index.md
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.2/docs/source/javascript_api.rst
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.2/docs/source/overview.md
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.2/docs/source/python_api.rst
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.2/docs/source/schema.md
--rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.2/docs/source/_static/jupyter_logo.svg
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.2/docs/source/_static/logo-icon.png
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.2/javascript/package.json
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.2/jupyter_ydoc/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.2/jupyter_ydoc/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.2/jupyter_ydoc/py.typed
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.2/jupyter_ydoc/utils.py
--rw-r--r--   0        0        0     4004 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.2/jupyter_ydoc/ybasedoc.py
--rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.2/jupyter_ydoc/yblob.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.2/jupyter_ydoc/yfile.py
--rw-r--r--   0        0        0     9241 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.2/jupyter_ydoc/ynotebook.py
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.2/jupyter_ydoc/yunicode.py
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.2/.gitignore
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.2/LICENSE
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.2/README.md
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 jupyter_ydoc-1.1.0a0/.licenserc.yaml
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 jupyter_ydoc-1.1.0a0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyter_ydoc-1.1.0a0/.yarnrc.yml
+-rw-r--r--   0        0        0    53324 2020-02-02 00:00:00.000000 jupyter_ydoc-1.1.0a0/CHANGELOG.md
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 jupyter_ydoc-1.1.0a0/lerna.json
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 jupyter_ydoc-1.1.0a0/package.json
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 jupyter_ydoc-1.1.0a0/pytest.ini
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 jupyter_ydoc-1.1.0a0/readthedocs.yml
+-rw-r--r--   0        0        0   185553 2020-02-02 00:00:00.000000 jupyter_ydoc-1.1.0a0/yarn.lock
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 jupyter_ydoc-1.1.0a0/.github/dependabot.yml
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 jupyter_ydoc-1.1.0a0/.github/workflows/auto_author_assign.yml
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 jupyter_ydoc-1.1.0a0/.github/workflows/check-release.yml
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 jupyter_ydoc-1.1.0a0/.github/workflows/enforce-label.yml
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 jupyter_ydoc-1.1.0a0/.github/workflows/license-header.yml
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 jupyter_ydoc-1.1.0a0/.github/workflows/prep-release.yml
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 jupyter_ydoc-1.1.0a0/.github/workflows/publish-release.yml
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 jupyter_ydoc-1.1.0a0/.github/workflows/test.yml
+-rwxr-xr-x   0        0        0  2212925 2020-02-02 00:00:00.000000 jupyter_ydoc-1.1.0a0/.yarn/releases/yarn-3.4.1.cjs
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 jupyter_ydoc-1.1.0a0/docs/Makefile
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 jupyter_ydoc-1.1.0a0/docs/make.bat
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 jupyter_ydoc-1.1.0a0/docs/source/conf.py
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 jupyter_ydoc-1.1.0a0/docs/source/custom.md
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 jupyter_ydoc-1.1.0a0/docs/source/index.md
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 jupyter_ydoc-1.1.0a0/docs/source/javascript_api.rst
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 jupyter_ydoc-1.1.0a0/docs/source/overview.md
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 jupyter_ydoc-1.1.0a0/docs/source/python_api.rst
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 jupyter_ydoc-1.1.0a0/docs/source/schema.md
+-rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 jupyter_ydoc-1.1.0a0/docs/source/_static/jupyter_logo.svg
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 jupyter_ydoc-1.1.0a0/docs/source/_static/logo-icon.png
+-rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 jupyter_ydoc-1.1.0a0/javascript/package.json
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 jupyter_ydoc-1.1.0a0/jupyter_ydoc/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupyter_ydoc-1.1.0a0/jupyter_ydoc/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_ydoc-1.1.0a0/jupyter_ydoc/py.typed
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 jupyter_ydoc-1.1.0a0/jupyter_ydoc/utils.py
+-rw-r--r--   0        0        0     4004 2020-02-02 00:00:00.000000 jupyter_ydoc-1.1.0a0/jupyter_ydoc/ybasedoc.py
+-rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 jupyter_ydoc-1.1.0a0/jupyter_ydoc/yblob.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyter_ydoc-1.1.0a0/jupyter_ydoc/yfile.py
+-rw-r--r--   0        0        0     9241 2020-02-02 00:00:00.000000 jupyter_ydoc-1.1.0a0/jupyter_ydoc/ynotebook.py
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 jupyter_ydoc-1.1.0a0/jupyter_ydoc/yunicode.py
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 jupyter_ydoc-1.1.0a0/.gitignore
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 jupyter_ydoc-1.1.0a0/LICENSE
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 jupyter_ydoc-1.1.0a0/README.md
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 jupyter_ydoc-1.1.0a0/pyproject.toml
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 jupyter_ydoc-1.1.0a0/PKG-INFO
```

### Comparing `jupyter_ydoc-1.0.2/.licenserc.yaml` & `jupyter_ydoc-1.1.0a0/.licenserc.yaml`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.2/.pre-commit-config.yaml` & `jupyter_ydoc-1.1.0a0/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     rev: 5.12.0
     hooks:
       - id: isort
         files: \.py$
         args: [--profile=black]
 
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.1
+    rev: v3.7.0
     hooks:
       - id: pyupgrade
         args: [--py37-plus]
 
   - repo: https://github.com/PyCQA/doc8
     rev: v1.1.1
     hooks:
```

### Comparing `jupyter_ydoc-1.0.2/CHANGELOG.md` & `jupyter_ydoc-1.1.0a0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,29 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 1.1.0a0
+
+([Full Changelog](https://github.com/jupyter-server/jupyter_ydoc/compare/@jupyter/ydoc@1.0.2...b7a1dc047e9a91a831dab68fdb294d56f46ab168))
+
+### Enhancements made
+
+- Create awareness interface [#171](https://github.com/jupyter-server/jupyter_ydoc/pull/171) ([@hbcarlos](https://github.com/hbcarlos))
+
+### Maintenance and upkeep improvements
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyter-server/jupyter_ydoc/graphs/contributors?from=2023-04-14&to=2023-06-29&type=c))
+
+[@hbcarlos](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_ydoc+involves%3Ahbcarlos+updated%3A2023-04-14..2023-06-29&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_ydoc+involves%3Apre-commit-ci+updated%3A2023-04-14..2023-06-29&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 1.0.2
 
 ([Full Changelog](https://github.com/jupyter-server/jupyter_ydoc/compare/@jupyter/ydoc@1.0.1...3b3a4af50ea46abd886076b69b93ee0dab6b05c5))
 
 ### Enhancements made
 
 - Trust the default cell [#161](https://github.com/jupyter-server/jupyter_ydoc/pull/161) ([@krassowski](https://github.com/krassowski))
@@ -16,16 +34,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyter-server/jupyter_ydoc/graphs/contributors?from=2023-04-11&to=2023-04-14&type=c))
 
 [@davidbrochart](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_ydoc+involves%3Adavidbrochart+updated%3A2023-04-11..2023-04-14&type=Issues) | [@fcollonval](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_ydoc+involves%3Afcollonval+updated%3A2023-04-11..2023-04-14&type=Issues) | [@krassowski](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_ydoc+involves%3Akrassowski+updated%3A2023-04-11..2023-04-14&type=Issues) | [@welcome](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_ydoc+involves%3Awelcome+updated%3A2023-04-11..2023-04-14&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 1.0.1
 
 ([Full Changelog](https://github.com/jupyter-server/jupyter_ydoc/compare/@jupyter/ydoc@1.0.0...6672e3dd27c2980f45ce1037101f0198fac3d9ff))
 
 ### Bugs fixed
 
 - Fix metadata issue [#158](https://github.com/jupyter-server/jupyter_ydoc/pull/158) ([@hbcarlos](https://github.com/hbcarlos))
```

### Comparing `jupyter_ydoc-1.0.2/yarn.lock` & `jupyter_ydoc-1.1.0a0/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.2/.github/workflows/check-release.yml` & `jupyter_ydoc-1.1.0a0/.github/workflows/check-release.yml`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.2/.github/workflows/license-header.yml` & `jupyter_ydoc-1.1.0a0/.github/workflows/license-header.yml`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.2/.github/workflows/prep-release.yml` & `jupyter_ydoc-1.1.0a0/.github/workflows/prep-release.yml`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.2/.github/workflows/publish-release.yml` & `jupyter_ydoc-1.1.0a0/.github/workflows/publish-release.yml`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.2/.github/workflows/test.yml` & `jupyter_ydoc-1.1.0a0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.2/.yarn/releases/yarn-3.4.1.cjs` & `jupyter_ydoc-1.1.0a0/.yarn/releases/yarn-3.4.1.cjs`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.2/docs/Makefile` & `jupyter_ydoc-1.1.0a0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.2/docs/make.bat` & `jupyter_ydoc-1.1.0a0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.2/docs/source/conf.py` & `jupyter_ydoc-1.1.0a0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.2/docs/source/custom.md` & `jupyter_ydoc-1.1.0a0/docs/source/custom.md`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.2/docs/source/overview.md` & `jupyter_ydoc-1.1.0a0/docs/source/overview.md`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.2/docs/source/schema.md` & `jupyter_ydoc-1.1.0a0/docs/source/schema.md`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.2/docs/source/_static/jupyter_logo.svg` & `jupyter_ydoc-1.1.0a0/docs/source/_static/jupyter_logo.svg`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.2/docs/source/_static/logo-icon.png` & `jupyter_ydoc-1.1.0a0/docs/source/_static/logo-icon.png`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.2/javascript/package.json` & `jupyter_ydoc-1.1.0a0/javascript/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9705882352941176%*

 * *Differences: {"'version'": "'1.1.0-a0'"}*

```diff
@@ -60,9 +60,9 @@
         "test:cov": "jest --collect-coverage",
         "test:debug": "node --inspect-brk node_modules/.bin/jest --runInBand",
         "test:debug:watch": "node --inspect-brk node_modules/.bin/jest --runInBand --watch",
         "watch": "tsc -b --watch"
     },
     "type": "module",
     "types": "lib/index.d.ts",
-    "version": "1.0.2"
+    "version": "1.1.0-a0"
 }
```

### Comparing `jupyter_ydoc-1.0.2/jupyter_ydoc/__init__.py` & `jupyter_ydoc-1.1.0a0/jupyter_ydoc/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.2/jupyter_ydoc/utils.py` & `jupyter_ydoc-1.1.0a0/jupyter_ydoc/utils.py`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.2/jupyter_ydoc/ybasedoc.py` & `jupyter_ydoc-1.1.0a0/jupyter_ydoc/ybasedoc.py`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.2/jupyter_ydoc/yblob.py` & `jupyter_ydoc-1.1.0a0/jupyter_ydoc/yblob.py`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.2/jupyter_ydoc/ynotebook.py` & `jupyter_ydoc-1.1.0a0/jupyter_ydoc/ynotebook.py`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.2/jupyter_ydoc/yunicode.py` & `jupyter_ydoc-1.1.0a0/jupyter_ydoc/yunicode.py`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.2/.gitignore` & `jupyter_ydoc-1.1.0a0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.2/LICENSE` & `jupyter_ydoc-1.1.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.2/README.md` & `jupyter_ydoc-1.1.0a0/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.2/pyproject.toml` & `jupyter_ydoc-1.1.0a0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.2/PKG-INFO` & `jupyter_ydoc-1.1.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-ydoc
-Version: 1.0.2
+Version: 1.1.0a0
 Summary: Document structures for collaborative editing using Ypy
 Project-URL: Homepage, https://jupyter.org
 Project-URL: Source, https://github.com/jupyter-server/jupyter_ydoc
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: LICENSE
 Keywords: jupyter,ypy
```

