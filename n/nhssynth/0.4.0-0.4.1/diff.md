# Comparing `tmp/nhssynth-0.4.0.tar.gz` & `tmp/nhssynth-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nhssynth-0.4.0.tar", max compression
+gzip compressed data, was "nhssynth-0.4.1.tar", max compression
```

## Comparing `nhssynth-0.4.0.tar` & `nhssynth-0.4.1.tar`

### file list

```diff
@@ -1,49 +1,51 @@
--rw-r--r--   0        0        0     1068 2023-03-31 11:03:40.629205 nhssynth-0.4.0/LICENSE
--rw-r--r--   0        0        0     8773 2023-07-17 19:18:22.721883 nhssynth-0.4.0/README.md
--rw-r--r--   0        0        0     1898 2023-07-18 08:12:24.276413 nhssynth-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       21 2023-03-21 11:15:21.821516 nhssynth-0.4.0/src/nhssynth/cli/__init__.py
--rw-r--r--   0        0        0     3556 2023-07-17 19:18:22.733434 nhssynth-0.4.0/src/nhssynth/cli/common_arguments.py
--rw-r--r--   0        0        0     8854 2023-05-10 13:14:43.837250 nhssynth-0.4.0/src/nhssynth/cli/config.py
--rw-r--r--   0        0        0     1826 2023-04-26 19:31:33.657526 nhssynth-0.4.0/src/nhssynth/cli/model_arguments.py
--rw-r--r--   0        0        0     6820 2023-07-17 19:18:22.733805 nhssynth-0.4.0/src/nhssynth/cli/module_arguments.py
--rw-r--r--   0        0        0     7421 2023-07-17 19:18:22.734062 nhssynth-0.4.0/src/nhssynth/cli/module_setup.py
--rw-r--r--   0        0        0     1396 2023-04-26 19:31:33.658300 nhssynth-0.4.0/src/nhssynth/cli/run.py
--rw-r--r--   0        0        0       82 2023-04-04 13:59:35.254031 nhssynth-0.4.0/src/nhssynth/common/__init__.py
--rw-r--r--   0        0        0      385 2023-04-27 13:22:15.158073 nhssynth-0.4.0/src/nhssynth/common/common.py
--rw-r--r--   0        0        0     3411 2023-07-17 19:18:22.734745 nhssynth-0.4.0/src/nhssynth/common/constants.py
--rw-r--r--   0        0        0      376 2023-04-26 19:31:33.658992 nhssynth-0.4.0/src/nhssynth/common/debugging.py
--rw-r--r--   0        0        0     2369 2023-04-27 13:23:24.877565 nhssynth-0.4.0/src/nhssynth/common/dicts.py
--rw-r--r--   0        0        0     3149 2023-04-27 13:23:45.952265 nhssynth-0.4.0/src/nhssynth/common/io.py
--rw-r--r--   0        0        0      582 2023-04-26 19:31:33.659388 nhssynth-0.4.0/src/nhssynth/common/strings.py
--rw-r--r--   0        0        0        0 2023-03-09 10:01:33.834460 nhssynth-0.4.0/src/nhssynth/modules/__init__.py
--rw-r--r--   0        0        0       21 2023-07-17 19:18:22.735148 nhssynth-0.4.0/src/nhssynth/modules/dataloader/__init__.py
--rw-r--r--   0        0        0     3882 2023-07-17 19:18:22.735402 nhssynth-0.4.0/src/nhssynth/modules/dataloader/io.py
--rw-r--r--   0        0        0    11433 2023-07-17 19:18:22.735655 nhssynth-0.4.0/src/nhssynth/modules/dataloader/metadata.py
--rw-r--r--   0        0        0    11881 2023-07-18 08:11:26.033379 nhssynth-0.4.0/src/nhssynth/modules/dataloader/metatransformer.py
--rw-r--r--   0        0        0     3611 2023-07-17 19:18:22.736200 nhssynth-0.4.0/src/nhssynth/modules/dataloader/missingness.py
--rw-r--r--   0        0        0     1220 2023-07-18 08:11:26.033558 nhssynth-0.4.0/src/nhssynth/modules/dataloader/run.py
--rw-r--r--   0        0        0      125 2023-07-17 19:18:22.736677 nhssynth-0.4.0/src/nhssynth/modules/dataloader/transformers/__init__.py
--rw-r--r--   0        0        0     1315 2023-07-18 08:11:26.033735 nhssynth-0.4.0/src/nhssynth/modules/dataloader/transformers/categorical.py
--rw-r--r--   0        0        0     4128 2023-07-18 08:11:26.033910 nhssynth-0.4.0/src/nhssynth/modules/dataloader/transformers/continuous.py
--rw-r--r--   0        0        0      946 2023-07-18 08:11:26.034078 nhssynth-0.4.0/src/nhssynth/modules/dataloader/transformers/datetime.py
--rw-r--r--   0        0        0     1075 2023-07-18 08:11:26.034216 nhssynth-0.4.0/src/nhssynth/modules/dataloader/transformers/generic.py
--rw-r--r--   0        0        0       21 2023-03-07 10:58:04.573024 nhssynth-0.4.0/src/nhssynth/modules/evaluation/__init__.py
--rw-r--r--   0        0        0    14071 2023-06-07 10:04:58.683189 nhssynth-0.4.0/src/nhssynth/modules/evaluation/full_report.py
--rw-r--r--   0        0        0     2605 2023-07-17 19:18:22.738439 nhssynth-0.4.0/src/nhssynth/modules/evaluation/io.py
--rw-r--r--   0        0        0     3031 2023-04-11 16:04:10.935343 nhssynth-0.4.0/src/nhssynth/modules/evaluation/metrics.py
--rw-r--r--   0        0        0     1835 2023-06-26 13:59:10.658401 nhssynth-0.4.0/src/nhssynth/modules/evaluation/run.py
--rw-r--r--   0        0        0       48 2023-04-26 19:31:33.660900 nhssynth-0.4.0/src/nhssynth/modules/model/__init__.py
--rw-r--r--   0        0        0     6634 2023-07-18 08:11:26.034691 nhssynth-0.4.0/src/nhssynth/modules/model/common/Model.py
--rw-r--r--   0        0        0     4345 2023-07-17 19:18:22.738937 nhssynth-0.4.0/src/nhssynth/modules/model/common/dp.py
--rw-r--r--   0        0        0     3484 2023-07-17 19:18:22.739182 nhssynth-0.4.0/src/nhssynth/modules/model/io.py
--rw-r--r--   0        0        0      129 2023-07-17 19:18:22.739961 nhssynth-0.4.0/src/nhssynth/modules/model/models/__init__.py
--rw-r--r--   0        0        0     1643 2023-07-17 19:18:22.739444 nhssynth-0.4.0/src/nhssynth/modules/model/models/dpvae.py
--rw-r--r--   0        0        0    10165 2023-07-17 19:18:22.739716 nhssynth-0.4.0/src/nhssynth/modules/model/models/vae.py
--rw-r--r--   0        0        0     2337 2023-07-17 19:18:22.740199 nhssynth-0.4.0/src/nhssynth/modules/model/run.py
--rw-r--r--   0        0        0       21 2023-03-07 10:58:07.632275 nhssynth-0.4.0/src/nhssynth/modules/plotting/__init__.py
--rw-r--r--   0        0        0     2589 2023-05-05 14:21:02.303228 nhssynth-0.4.0/src/nhssynth/modules/plotting/io.py
--rw-r--r--   0        0        0     6421 2023-04-13 19:24:58.843577 nhssynth-0.4.0/src/nhssynth/modules/plotting/plots.py
--rw-r--r--   0        0        0      727 2023-04-13 12:33:18.866696 nhssynth-0.4.0/src/nhssynth/modules/plotting/run.py
--rw-r--r--   0        0        0       21 2023-03-07 10:58:13.024183 nhssynth-0.4.0/src/nhssynth/modules/structure/__init__.py
--rw-r--r--   0        0        0       85 2023-03-07 10:58:26.227434 nhssynth-0.4.0/src/nhssynth/modules/structure/run.py
--rw-r--r--   0        0        0    10094 1970-01-01 00:00:00.000000 nhssynth-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-03-31 11:03:40.629205 nhssynth-0.4.1/LICENSE
+-rw-r--r--   0        0        0     8773 2023-07-17 19:18:22.721883 nhssynth-0.4.1/README.md
+-rw-r--r--   0        0        0     1954 2023-07-18 11:32:48.445355 nhssynth-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-03-21 11:15:21.821516 nhssynth-0.4.1/src/nhssynth/cli/__init__.py
+-rw-r--r--   0        0        0       72 2023-07-18 11:25:55.792483 nhssynth-0.4.1/src/nhssynth/cli/__main__.py
+-rw-r--r--   0        0        0     3556 2023-07-17 19:18:22.733434 nhssynth-0.4.1/src/nhssynth/cli/common_arguments.py
+-rw-r--r--   0        0        0     8854 2023-05-10 13:14:43.837250 nhssynth-0.4.1/src/nhssynth/cli/config.py
+-rw-r--r--   0        0        0     1826 2023-04-26 19:31:33.657526 nhssynth-0.4.1/src/nhssynth/cli/model_arguments.py
+-rw-r--r--   0        0        0     6820 2023-07-17 19:18:22.733805 nhssynth-0.4.1/src/nhssynth/cli/module_arguments.py
+-rw-r--r--   0        0        0     7421 2023-07-17 19:18:22.734062 nhssynth-0.4.1/src/nhssynth/cli/module_setup.py
+-rw-r--r--   0        0        0     1410 2023-07-18 10:19:28.644752 nhssynth-0.4.1/src/nhssynth/cli/run.py
+-rw-r--r--   0        0        0       82 2023-04-04 13:59:35.254031 nhssynth-0.4.1/src/nhssynth/common/__init__.py
+-rw-r--r--   0        0        0      385 2023-04-27 13:22:15.158073 nhssynth-0.4.1/src/nhssynth/common/common.py
+-rw-r--r--   0        0        0     3411 2023-07-17 19:18:22.734745 nhssynth-0.4.1/src/nhssynth/common/constants.py
+-rw-r--r--   0        0        0      376 2023-04-26 19:31:33.658992 nhssynth-0.4.1/src/nhssynth/common/debugging.py
+-rw-r--r--   0        0        0     2369 2023-04-27 13:23:24.877565 nhssynth-0.4.1/src/nhssynth/common/dicts.py
+-rw-r--r--   0        0        0     3149 2023-04-27 13:23:45.952265 nhssynth-0.4.1/src/nhssynth/common/io.py
+-rw-r--r--   0        0        0      582 2023-04-26 19:31:33.659388 nhssynth-0.4.1/src/nhssynth/common/strings.py
+-rw-r--r--   0        0        0        0 2023-03-09 10:01:33.834460 nhssynth-0.4.1/src/nhssynth/modules/__init__.py
+-rw-r--r--   0        0        0       21 2023-07-17 19:18:22.735148 nhssynth-0.4.1/src/nhssynth/modules/dataloader/__init__.py
+-rw-r--r--   0        0        0     3882 2023-07-17 19:18:22.735402 nhssynth-0.4.1/src/nhssynth/modules/dataloader/io.py
+-rw-r--r--   0        0        0    11475 2023-07-18 08:54:50.452510 nhssynth-0.4.1/src/nhssynth/modules/dataloader/metadata.py
+-rw-r--r--   0        0        0    11798 2023-07-18 11:18:44.863981 nhssynth-0.4.1/src/nhssynth/modules/dataloader/metatransformer.py
+-rw-r--r--   0        0        0     3606 2023-07-18 11:18:44.864213 nhssynth-0.4.1/src/nhssynth/modules/dataloader/missingness.py
+-rw-r--r--   0        0        0     1220 2023-07-18 08:11:26.033558 nhssynth-0.4.1/src/nhssynth/modules/dataloader/run.py
+-rw-r--r--   0        0        0      125 2023-07-17 19:18:22.736677 nhssynth-0.4.1/src/nhssynth/modules/dataloader/transformers/__init__.py
+-rw-r--r--   0        0        0     1595 2023-07-18 11:18:44.864434 nhssynth-0.4.1/src/nhssynth/modules/dataloader/transformers/categorical.py
+-rw-r--r--   0        0        0     4128 2023-07-18 08:11:26.033910 nhssynth-0.4.1/src/nhssynth/modules/dataloader/transformers/continuous.py
+-rw-r--r--   0        0        0      993 2023-07-18 11:18:44.864634 nhssynth-0.4.1/src/nhssynth/modules/dataloader/transformers/datetime.py
+-rw-r--r--   0        0        0     1075 2023-07-18 08:11:26.034216 nhssynth-0.4.1/src/nhssynth/modules/dataloader/transformers/generic.py
+-rw-r--r--   0        0        0       21 2023-03-07 10:58:04.573024 nhssynth-0.4.1/src/nhssynth/modules/evaluation/__init__.py
+-rw-r--r--   0        0        0    14071 2023-06-07 10:04:58.683189 nhssynth-0.4.1/src/nhssynth/modules/evaluation/full_report.py
+-rw-r--r--   0        0        0     2605 2023-07-17 19:18:22.738439 nhssynth-0.4.1/src/nhssynth/modules/evaluation/io.py
+-rw-r--r--   0        0        0     3031 2023-04-11 16:04:10.935343 nhssynth-0.4.1/src/nhssynth/modules/evaluation/metrics.py
+-rw-r--r--   0        0        0     1835 2023-06-26 13:59:10.658401 nhssynth-0.4.1/src/nhssynth/modules/evaluation/run.py
+-rw-r--r--   0        0        0       48 2023-04-26 19:31:33.660900 nhssynth-0.4.1/src/nhssynth/modules/model/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 11:30:16.337912 nhssynth-0.4.1/src/nhssynth/modules/model/common/__init__.py
+-rw-r--r--   0        0        0     4345 2023-07-17 19:18:22.738937 nhssynth-0.4.1/src/nhssynth/modules/model/common/dp.py
+-rw-r--r--   0        0        0     7747 2023-07-18 09:00:44.494799 nhssynth-0.4.1/src/nhssynth/modules/model/common/model.py
+-rw-r--r--   0        0        0     3484 2023-07-17 19:18:22.739182 nhssynth-0.4.1/src/nhssynth/modules/model/io.py
+-rw-r--r--   0        0        0      129 2023-07-17 19:18:22.739961 nhssynth-0.4.1/src/nhssynth/modules/model/models/__init__.py
+-rw-r--r--   0        0        0     1643 2023-07-18 09:00:44.495313 nhssynth-0.4.1/src/nhssynth/modules/model/models/dpvae.py
+-rw-r--r--   0        0        0    10282 2023-07-18 09:00:44.495583 nhssynth-0.4.1/src/nhssynth/modules/model/models/vae.py
+-rw-r--r--   0        0        0     2337 2023-07-17 19:18:22.740199 nhssynth-0.4.1/src/nhssynth/modules/model/run.py
+-rw-r--r--   0        0        0       21 2023-03-07 10:58:07.632275 nhssynth-0.4.1/src/nhssynth/modules/plotting/__init__.py
+-rw-r--r--   0        0        0     2589 2023-05-05 14:21:02.303228 nhssynth-0.4.1/src/nhssynth/modules/plotting/io.py
+-rw-r--r--   0        0        0     6421 2023-04-13 19:24:58.843577 nhssynth-0.4.1/src/nhssynth/modules/plotting/plots.py
+-rw-r--r--   0        0        0      727 2023-04-13 12:33:18.866696 nhssynth-0.4.1/src/nhssynth/modules/plotting/run.py
+-rw-r--r--   0        0        0       21 2023-03-07 10:58:13.024183 nhssynth-0.4.1/src/nhssynth/modules/structure/__init__.py
+-rw-r--r--   0        0        0       85 2023-03-07 10:58:26.227434 nhssynth-0.4.1/src/nhssynth/modules/structure/run.py
+-rw-r--r--   0        0        0    10140 1970-01-01 00:00:00.000000 nhssynth-0.4.1/PKG-INFO
```

### Comparing `nhssynth-0.4.0/LICENSE` & `nhssynth-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nhssynth-0.4.0/README.md` & `nhssynth-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `nhssynth-0.4.0/pyproject.toml` & `nhssynth-0.4.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nhssynth"
-version = "0.4.0"
+version = "0.4.1"
 description = "Synthetic data generation pipeline leveraging a Differentially Private Variational Auto Encoder assessed using a variety of metrics"
 authors = ["HarrisonWilde <harrisondwilde@outlook.com>"]
 maintainers = ["NHSE TDAU <england.tdau@nhs.net>"]
 license = "MIT"
 readme = ["README.md"]
 repository = "https://github.com/nhsx/NHSSynth"
 keywords = ["synthetic data", "privacy", "fairness", "machine learning"]
@@ -19,28 +19,29 @@
 [tool.poetry.dependencies]
 python = ">=3.9,<3.11"
 pandas = "^2.0.1"
 scikit-learn = "^1.2.2"
 tqdm = "^4.65.0"
 gower = "^0.1.2"
 pyyaml = "^6.0"
-torch = "^2.0.1"
+torch = ">=2.0.0, !=2.0.1"
 opacus = "^1.4.0"
 requests = "^2.31.0"
 tornado = "^6.3.2"
 sdmetrics = "^0.10.1"
+setuptools = "^68.0.0"
 
 [tool.poetry.scripts]
-nhssynth = 'nhssynth.cli:run'
+nhssynth = "nhssynth.cli.__main__:__main__"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-mkdocstrings = {extras = ["python-legacy"], version = "^0.20.0"}
+mkdocstrings = {extras = ["python"], version = "^0.20.0"}
 mkdocs-material = "^9.1.4"
 mkdocs-gen-files = "^0.4.0"
 mkdocs-literate-nav = "^0.6.0"
 mkdocs-section-index = "^0.3.5"
 mkdocs-git-revision-date-localized-plugin = "^1.2.0"
 pymdown-extensions = "^10.0.1"
 
@@ -55,14 +56,15 @@
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 tox = "^4.0.0"
+mock = "^5.1.0"
 
 [tool.pytest.ini_options]
 testpaths = "tests"
 filterwarnings = ["ignore::DeprecationWarning:pkg_resources"]
 
 [tool.coverage.run]
 source = ["src/nhssynth/cli", "src/nhssynth/common", "src/nhssynth/modules"]
```

### Comparing `nhssynth-0.4.0/src/nhssynth/cli/common_arguments.py` & `nhssynth-0.4.1/src/nhssynth/cli/common_arguments.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.4.0/src/nhssynth/cli/config.py` & `nhssynth-0.4.1/src/nhssynth/cli/config.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.4.0/src/nhssynth/cli/model_arguments.py` & `nhssynth-0.4.1/src/nhssynth/cli/model_arguments.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.4.0/src/nhssynth/cli/module_arguments.py` & `nhssynth-0.4.1/src/nhssynth/cli/module_arguments.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.4.0/src/nhssynth/cli/module_setup.py` & `nhssynth-0.4.1/src/nhssynth/cli/module_setup.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.4.0/src/nhssynth/cli/run.py` & `nhssynth-0.4.1/src/nhssynth/cli/run.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import argparse
 import warnings
 
 from nhssynth.cli.config import get_modules_to_run, read_config, write_config
 from nhssynth.cli.module_setup import MODULE_MAP, add_subparser
 
 
-def run() -> None:
+def run(sysargv) -> None:
     parser = argparse.ArgumentParser(
         prog="nhssynth",
         description="CLI for preparing, training and evaluating a synthetic data generator.",
     )
 
     # Below we instantiate one subparser for each module + one for running with a config file and one for
     # doing a full pipeline run with CLI-specified config
     subparsers = parser.add_subparsers()
     all_subparsers = {
         name: add_subparser(subparsers, name, option_config) for name, option_config in MODULE_MAP.items()
     }
 
-    args = parser.parse_args()
+    args = parser.parse_args(sysargv)
 
     executor = vars(args).get("func", None)
     if executor:
         if not args.seed:
             warnings.warn("No seed has been specified, meaning the results of this run may not be reproducible.")
         args.modules_to_run = get_modules_to_run(executor)
         args.module_handover = {}
```

### Comparing `nhssynth-0.4.0/src/nhssynth/common/constants.py` & `nhssynth-0.4.1/src/nhssynth/common/constants.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.4.0/src/nhssynth/common/dicts.py` & `nhssynth-0.4.1/src/nhssynth/common/dicts.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.4.0/src/nhssynth/common/io.py` & `nhssynth-0.4.1/src/nhssynth/common/io.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.4.0/src/nhssynth/common/strings.py` & `nhssynth-0.4.1/src/nhssynth/common/strings.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.4.0/src/nhssynth/modules/dataloader/io.py` & `nhssynth-0.4.1/src/nhssynth/modules/dataloader/io.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.4.0/src/nhssynth/modules/dataloader/metadata.py` & `nhssynth-0.4.1/src/nhssynth/modules/dataloader/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,16 @@
     def __getitem__(self, key: str) -> dict[str, Any]:
         return self._metadata[key]
 
     def __iter__(self) -> Iterator:
         return iter(self._metadata.values())
 
     @classmethod
-    def load(cls, path: str, data: pd.DataFrame):
+    def load(cls, path_str: str, data: pd.DataFrame):
+        path = pathlib.Path(path_str)
         if path.exists():
             with open(path) as stream:
                 metadata = yaml.safe_load(stream)
             # Filter out expanded alias/anchor groups
             metadata = filter_dict(metadata, {"column_types"})
         else:
             warnings.warn(f"No metadata found at {path}...")
```

### Comparing `nhssynth-0.4.0/src/nhssynth/modules/dataloader/metatransformer.py` & `nhssynth-0.4.1/src/nhssynth/modules/dataloader/metatransformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -136,15 +136,17 @@
                     self.missingness_strategy(self.impute_value)
                     if isinstance(self.missingness_strategy, ImputeMissingnessStrategy)
                     else self.missingness_strategy()
                 )
             if not working_data[column_metadata.name].isnull().any():
                 continue
             working_data = column_metadata.missingness_strategy.remove(working_data, column_metadata)
-            if column_metadata.dtype.kind in ["i", "u", "f"]:
+            if column_metadata.dtype.kind in ["i", "u", "f"] and not isinstance(
+                column_metadata.missingness_strategy, AugmentMissingnessStrategy
+            ):
                 working_data[column_metadata.name] = working_data[column_metadata.name].astype(
                     column_metadata.dtype.name.lower()
                 )
         return working_data
 
     def transform(self) -> pd.DataFrame:
         """
@@ -167,21 +169,18 @@
 
         print("")
 
         for column_metadata in tqdm(
             self.metadata, desc="Transforming data", unit="column", total=len(self.metadata.columns)
         ):
             # TODO is there a nicer way of doing this, the transformer and augment strategy create a chicken and egg problem
-            if hasattr(column_metadata.missingness_strategy, "missing_column") and not column_metadata.categorical:
-                transformed_data = column_metadata.transformer.apply(
-                    working_data[column_metadata.name],
-                    working_data[column_metadata.missingness_strategy.missing_column],
-                )
-            else:
-                transformed_data = column_metadata.transformer.apply(working_data[column_metadata.name])
+            transformed_data = column_metadata.transformer.apply(
+                working_data[column_metadata.name],
+                getattr(column_metadata.missingness_strategy, "missingness_carrier", None),
+            )
             if column_metadata.dtype.kind in ["f", "i", "u"]:
                 if isinstance(transformed_data, pd.DataFrame):
                     transformed_data = transformed_data.apply(lambda x: x.astype(column_metadata.dtype.name.lower()))
                 else:
                     transformed_data = transformed_data.astype(column_metadata.dtype.name.lower())
             transformed_columns.append(transformed_data)
             if isinstance(transformed_data, pd.DataFrame) and transformed_data.shape[1] > 1:
@@ -196,27 +195,28 @@
                 self.single_column_indices.append(col_counter)
                 col_counter += 1
 
         print("")
 
         return pd.concat(transformed_columns, axis=1)
 
-    def apply(self) -> None:
+    def apply(self) -> pd.DataFrame:
         """
         Applies the various steps of the MetaTransformer to a passed DataFrame.
 
         Args:
             dataset: The DataFrame to transform.
 
         Returns:
             The transformed dataset.
         """
         self.typed_dataset = self.apply_dtypes()
         self.prepared_dataset = self.apply_missingness_strategy()
         self.transformed_dataset = self.transform()
+        return self.transformed_dataset
 
     def get_typed_dataset(self) -> pd.DataFrame:
         if not hasattr(self, "typed_dataset"):
             raise ValueError(
                 "The typed dataset has not yet been created. Call `mt.apply()` (or `mt.apply_dtypes()`) first."
             )
         return self.typed_dataset
```

### Comparing `nhssynth-0.4.0/src/nhssynth/modules/dataloader/missingness.py` & `nhssynth-0.4.1/src/nhssynth/modules/dataloader/missingness.py`

 * *Files 14% similar despite different names*

```diff
@@ -67,37 +67,36 @@
         data[column_metadata.name].fillna(self.imputation_value, inplace=True)
         return data
 
 
 class AugmentMissingnessStrategy(GenericMissingnessStrategy):
     def __init__(self) -> None:
         super().__init__("augment")
-        self.missing_value = 0.0
+        self.missingness_carrier = 0.0
 
     def remove(self, data: pd.DataFrame, column_metadata: ColumnMetaData) -> pd.DataFrame:
         """Impute missingness with model."""
         if column_metadata.categorical:
             if column_metadata.dtype.kind == "O":
-                self.missing_value = column_metadata.name + "_missing"
+                self.missingness_carrier = column_metadata.name + "_missing"
+            elif column_metadata.dtype.kind == "M":
+                self.missingness_carrier = np.datetime64("NaT")
             else:
-                self.missing_value = data[column_metadata.name].min() - 1
+                self.missingness_carrier = data[column_metadata.name].min() - 1
         else:
-            self.missing_column = column_metadata.name + "_missing"
-            data[self.missing_column] = data[column_metadata.name].isnull().astype(int)
-        if column_metadata.dtype.kind == "M":
-            self.missing_value = np.datetime64("NaT")
-        data[column_metadata.name].fillna(self.missing_value, inplace=True)
+            data[column_metadata.name + "_missing"] = data[column_metadata.name].isnull().astype(int)
+            self.missingness_carrier = data[column_metadata.name + "_missing"]
         return data
 
-    def restore(self, data: pd.DataFrame, column_metadata: ColumnMetaData) -> pd.Series:
-        """Restore missingness."""
-        if column_metadata.categorical:
-            return data.where(data == self.missing_value, np.nan)
-        else:
-            return data.where(data[self.missing_column] == 1, np.nan)
+    # def restore(self, data: pd.DataFrame, column_metadata: ColumnMetaData) -> pd.Series:
+    #     """Restore missingness."""
+    #     if column_metadata.categorical:
+    #         return data.where(data == self.missing_value, np.nan)
+    #     else:
+    #         return data.where(data[self.missing_column] == 1, np.nan)
 
 
 MISSINGNESS_STRATEGIES: Final = {
     "none": NullMissingnessStrategy,
     "impute": ImputeMissingnessStrategy,
     "augment": AugmentMissingnessStrategy,
     "drop": DropMissingnessStrategy,
```

### Comparing `nhssynth-0.4.0/src/nhssynth/modules/dataloader/run.py` & `nhssynth-0.4.1/src/nhssynth/modules/dataloader/run.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.4.0/src/nhssynth/modules/dataloader/transformers/categorical.py` & `nhssynth-0.4.1/src/nhssynth/modules/dataloader/transformers/datetime.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,22 @@
-from typing import Optional, Union
+from typing import Optional
 
 import pandas as pd
-from nhssynth.modules.dataloader.missingness import GenericMissingnessStrategy
-from nhssynth.modules.dataloader.transformers.generic import GenericTransformer
-from sklearn.preprocessing import OneHotEncoder
+from nhssynth.modules.dataloader.transformers.generic import *
 
 
-class OHETransformer(GenericTransformer):
-    def __init__(self, drop: Optional[Union[list, str]] = None) -> None:
-        super().__init__()
-        self._drop = drop
-        self._transformer = OneHotEncoder(handle_unknown="ignore", sparse_output=False, drop=self._drop)
+class DatetimeTransformer(TransformerWrapper):
+    def __init__(self, transformer: GenericTransformer, format: Optional[str] = None) -> None:
+        super().__init__(transformer)
+        self._format = format
 
-    def apply(self, data: pd.Series) -> pd.DataFrame:
-        self.original_column_name = data.name
-        transformed_data = pd.DataFrame(
-            self._transformer.fit_transform(data.values.reshape(-1, 1)),
-            columns=self._transformer.get_feature_names_out(input_features=[data.name]),
-        )
-        self.new_column_names = transformed_data.columns
-        return transformed_data
+    def apply(self, data: pd.Series, missingness_column: Optional[pd.Series] = None, **kwargs) -> pd.DataFrame:
+        self.column_name = data.name
+        numeric_data = pd.Series(data.dt.floor("ns").to_numpy().astype(float), name=data.name)
+        if missingness_column is not None:
+            numeric_data[missingness_column == 1] = 0.0
+        return super().apply(numeric_data, missingness_column, **kwargs)
 
-    def revert(self, data: pd.DataFrame) -> pd.DataFrame:
-        data[self.original_column_name] = pd.Series(
-            self._transformer.inverse_transform(data[self.new_column_names].values).flatten(),
-            index=data.index,
-            name=self.original_column_name,
-        )
-        data.drop(self.new_column_names, axis=1, inplace=True)
+    def revert(self, data: pd.DataFrame, **kwargs) -> pd.DataFrame:
+        reverted_data = super().revert(data, **kwargs)
+        data[self.column_name] = pd.to_datetime(reverted_data[self.column_name].astype("Int64"), unit="ns")
         return data
```

### Comparing `nhssynth-0.4.0/src/nhssynth/modules/dataloader/transformers/continuous.py` & `nhssynth-0.4.1/src/nhssynth/modules/dataloader/transformers/continuous.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.4.0/src/nhssynth/modules/dataloader/transformers/generic.py` & `nhssynth-0.4.1/src/nhssynth/modules/dataloader/transformers/generic.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.4.0/src/nhssynth/modules/evaluation/full_report.py` & `nhssynth-0.4.1/src/nhssynth/modules/evaluation/full_report.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.4.0/src/nhssynth/modules/evaluation/io.py` & `nhssynth-0.4.1/src/nhssynth/modules/evaluation/io.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.4.0/src/nhssynth/modules/evaluation/metrics.py` & `nhssynth-0.4.1/src/nhssynth/modules/evaluation/metrics.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.4.0/src/nhssynth/modules/evaluation/run.py` & `nhssynth-0.4.1/src/nhssynth/modules/evaluation/run.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.4.0/src/nhssynth/modules/model/common/Model.py` & `nhssynth-0.4.1/src/nhssynth/modules/model/common/model.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,55 +1,61 @@
+import argparse
 import time
 import warnings
 from abc import ABC, abstractmethod
 from typing import Optional
 
 import numpy as np
 import pandas as pd
 import torch
 import torch.nn as nn
 from nhssynth.common.strings import add_spaces_before_caps
+from nhssynth.modules.dataloader.metatransformer import MetaTransformer
 from torch.utils.data import DataLoader, TensorDataset
 from tqdm import tqdm
 
 
 class Model(nn.Module, ABC):
     """
     Abstract base class for all NHSSynth models
 
     Args:
         data: The data to train on
         multi_column_indices: A list of lists of column indices, where each sublist containts the indices for a one-hot encoded column
         single_column_indices: Indices of all non-onehot columns
         batch_size: The batch size to use during training
         use_gpu: Flag to determine whether to use the GPU (if available)
+        metatransformer: A `MetaTransformer` to use for converting the generated data to match the original data
 
     Attributes:
         nrows: The number of rows in the `data`
         ncols: The number of columns in the `data`
         columns: The names of the columns in the `data`
         multi_column_indices: A list of lists of column indices, where each sublist containts the indices for a one-hot encoded column
         single_column_indices: Indices of all non-onehot columns
         data_loader: A PyTorch DataLoader for the `data`
         private: Whether the model is private, i.e. whether the `DPMixin` class has been inherited
         device: The device to use for training (CPU or GPU)
+        metatransformer: The `MetaTransformer` (potentially) associated with the model
+        has_metatransformer: Whether the model has a `MetaTransformer` associated
 
     Raises:
         TypeError: If the `Model` class is directly instantiated (i.e. not inherited)
         AssertionError: If the number of columns in the `data` does not match the number of indices in `multi_column_indices` and `single_column_indices`
         UserWarning: If `use_gpu` is True but no GPU is available
     """
 
     def __init__(
         self,
         data: pd.DataFrame,
         multi_column_indices: Optional[list[list[int]]] = [[]],
         single_column_indices: Optional[list[int]] = [],
         batch_size: int = 32,
         use_gpu: bool = False,
+        metatransformer: Optional[MetaTransformer] = None,
     ) -> None:
         if type(self) is Model:
             raise TypeError("Cannot directly instantiate the `Model` class")
         super(Model, self).__init__()
         self.nrows, self.ncols = data.shape
         self.columns: pd.Index = data.columns
         self.multi_column_indices: list[list[int]] = multi_column_indices
@@ -58,14 +64,19 @@
         self.data_loader: DataLoader = DataLoader(
             # Should the data also all be turned into floats?
             TensorDataset(torch.Tensor(data.to_numpy())),
             pin_memory=True,
             batch_size=batch_size,
         )
         self.setup_device(use_gpu)
+        if metatransformer:
+            self.metatransformer = metatransformer
+            self.has_metatransformer = True
+        else:
+            self.has_metatransformer = False
 
     def setup_device(self, use_gpu: bool) -> None:
         """Sets up the device to use for training (CPU or GPU) depending on `use_gpu` and device availability."""
         if use_gpu:
             if torch.cuda.is_available():
                 self.device: torch.device = torch.device("cuda:0")
             else:
@@ -83,23 +94,40 @@
     @classmethod
     @abstractmethod
     def _get_args() -> list[str]:
         """Returns the list of arguments to look for in an `argparse.Namespace`, these must map to the arguments of the inheritor."""
         raise NotImplementedError
 
     @classmethod
-    def from_args(cls, args, data, multi_column_indices, single_column_indices):
+    def from_args(
+        cls,
+        args: argparse.Namespace,
+        data: pd.DataFrame,
+        multi_column_indices: list[list[int]],
+        single_column_indices: list[int],
+    ):
         """Creates an instance from an `argparse.Namespace`."""
         return cls(
             data,
             multi_column_indices,
             single_column_indices,
             **{k: getattr(args, k) for k in ["batch_size", "use_gpu"] + cls._get_args() if getattr(args, k)},
         )
 
+    @classmethod
+    def from_metatransformer(cls, data: pd.DataFrame, metatransformer: MetaTransformer, **kwargs):
+        """Creates an instance from a `MetaTransformer`."""
+        return cls(
+            data,
+            metatransformer.multi_column_indices,
+            metatransformer.single_column_indices,
+            metatransformer=metatransformer,
+            **kwargs,
+        )
+
     def _start_training(self, num_epochs: int, patience: int, tracked_metrics: list[str]) -> None:
         """Initialises the training process."""
         self.num_epochs = num_epochs
         self.patience = patience
         if not hasattr(self, "target_epsilon") and "Privacy" in tracked_metrics:
             tracked_metrics.remove("Privacy")
         self.metrics = {metric: np.empty(0, dtype=float) for metric in tracked_metrics}
```

### Comparing `nhssynth-0.4.0/src/nhssynth/modules/model/common/dp.py` & `nhssynth-0.4.1/src/nhssynth/modules/model/common/dp.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.4.0/src/nhssynth/modules/model/io.py` & `nhssynth-0.4.1/src/nhssynth/modules/model/io.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.4.0/src/nhssynth/modules/model/models/dpvae.py` & `nhssynth-0.4.1/src/nhssynth/modules/model/models/dpvae.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.4.0/src/nhssynth/modules/model/models/vae.py` & `nhssynth-0.4.1/src/nhssynth/modules/model/models/vae.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,15 +186,18 @@
                 ).sample()
 
         x_gen_[:, self.single_column_indices] = x_gen[:, self.single_column_indices] + torch.exp(
             self.noiser(x_gen[:, self.single_column_indices])
         ) * torch.randn_like(x_gen[:, self.single_column_indices])
         if torch.cuda.is_available():
             x_gen_ = x_gen_.cpu()
-        return pd.DataFrame(x_gen_.detach(), columns=self.columns)
+        data = pd.DataFrame(x_gen_.detach(), columns=self.columns)
+        if self.has_metatransformer:
+            data = self.metatransformer.inverse_apply(data)
+        return data
 
     def loss(self, X):
         mu_z, logsigma_z = self.encoder(X)
 
         p = Normal(torch.zeros_like(mu_z), torch.ones_like(mu_z))
         q = Normal(mu_z, torch.exp(logsigma_z))
```

### Comparing `nhssynth-0.4.0/src/nhssynth/modules/model/run.py` & `nhssynth-0.4.1/src/nhssynth/modules/model/run.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.4.0/src/nhssynth/modules/plotting/io.py` & `nhssynth-0.4.1/src/nhssynth/modules/plotting/io.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.4.0/src/nhssynth/modules/plotting/plots.py` & `nhssynth-0.4.1/src/nhssynth/modules/plotting/plots.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.4.0/src/nhssynth/modules/plotting/run.py` & `nhssynth-0.4.1/src/nhssynth/modules/plotting/run.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.4.0/PKG-INFO` & `nhssynth-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nhssynth
-Version: 0.4.0
+Version: 0.4.1
 Summary: Synthetic data generation pipeline leveraging a Differentially Private Variational Auto Encoder assessed using a variety of metrics
 Home-page: https://github.com/nhsx/NHSSynth
 License: MIT
 Keywords: synthetic data,privacy,fairness,machine learning
 Author: HarrisonWilde
 Author-email: harrisondwilde@outlook.com
 Maintainer: NHSE TDAU
@@ -18,15 +18,16 @@
 Requires-Dist: gower (>=0.1.2,<0.2.0)
 Requires-Dist: opacus (>=1.4.0,<2.0.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: sdmetrics (>=0.10.1,<0.11.0)
-Requires-Dist: torch (>=2.0.1,<3.0.0)
+Requires-Dist: setuptools (>=68.0.0,<69.0.0)
+Requires-Dist: torch (>=2.0.0,!=2.0.1)
 Requires-Dist: tornado (>=6.3.2,<7.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Project-URL: Bug Tracker, https://github.com/nhsx/NHSSynth/issues
 Project-URL: Docs, https://nhsx.github.io/NHSSynth
 Project-URL: Repository, https://github.com/nhsx/NHSSynth
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,25 +1,26 @@
-Metadata-Version: 2.1 Name: nhssynth Version: 0.4.0 Summary: Synthetic data
+Metadata-Version: 2.1 Name: nhssynth Version: 0.4.1 Summary: Synthetic data
 generation pipeline leveraging a Differentially Private Variational Auto
 Encoder assessed using a variety of metrics Home-page: https://github.com/nhsx/
 NHSSynth License: MIT Keywords: synthetic data,privacy,fairness,machine
 learning Author: HarrisonWilde Author-email: harrisondwilde@outlook.com
 Maintainer: NHSE TDAU Maintainer-email: england.tdau@nhs.net Requires-Python:
 >=3.9,<3.11 Classifier: Development Status :: 3 - Alpha Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Requires-Dist: gower (>=0.1.2,<0.2.0) Requires-Dist:
 opacus (>=1.4.0,<2.0.0) Requires-Dist: pandas (>=2.0.1,<3.0.0) Requires-Dist:
 pyyaml (>=6.0,<7.0) Requires-Dist: requests (>=2.31.0,<3.0.0) Requires-Dist:
 scikit-learn (>=1.2.2,<2.0.0) Requires-Dist: sdmetrics (>=0.10.1,<0.11.0)
-Requires-Dist: torch (>=2.0.1,<3.0.0) Requires-Dist: tornado (>=6.3.2,<7.0.0)
-Requires-Dist: tqdm (>=4.65.0,<5.0.0) Project-URL: Bug Tracker, https://
-github.com/nhsx/NHSSynth/issues Project-URL: Docs, https://nhsx.github.io/
-NHSSynth Project-URL: Repository, https://github.com/nhsx/NHSSynth Description-
-Content-Type: text/markdown
+Requires-Dist: setuptools (>=68.0.0,<69.0.0) Requires-Dist: torch
+(>=2.0.0,!=2.0.1) Requires-Dist: tornado (>=6.3.2,<7.0.0) Requires-Dist: tqdm
+(>=4.65.0,<5.0.0) Project-URL: Bug Tracker, https://github.com/nhsx/NHSSynth/
+issues Project-URL: Docs, https://nhsx.github.io/NHSSynth Project-URL:
+Repository, https://github.com/nhsx/NHSSynth Description-Content-Type: text/
+markdown
            ![Coverage](https://img.shields.io/endpoint?url=https://
 gist.githubusercontent.com/HarrisonWilde/1ab4eefed81ec381e29f7d4feb9856bc/raw/
  coverage.json) ![Tests Passing](https://img.shields.io/endpoint?url=https://
 gist.githubusercontent.com/HarrisonWilde/1ab4eefed81ec381e29f7d4feb9856bc/raw/
    tests.json) ![Lines of Code](https://img.shields.io/endpoint?url=https://
 gist.githubusercontent.com/HarrisonWilde/1ab4eefed81ec381e29f7d4feb9856bc/raw/
  loc.json) ![Percentage Comments](https://img.shields.io/endpoint?url=https://
```

