# Comparing `tmp/nhssynth-0.3.1.tar.gz` & `tmp/nhssynth-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nhssynth-0.3.1.tar", max compression
+gzip compressed data, was "nhssynth-0.4.0.tar", max compression
```

## Comparing `nhssynth-0.3.1.tar` & `nhssynth-0.4.0.tar`

### file list

```diff
@@ -1,43 +1,49 @@
--rw-r--r--   0        0        0     1068 2023-03-31 11:03:40.629205 nhssynth-0.3.1/LICENSE
--rw-r--r--   0        0        0     8859 2023-05-04 19:45:30.956684 nhssynth-0.3.1/README.md
--rw-r--r--   0        0        0     1867 2023-05-05 15:52:55.455154 nhssynth-0.3.1/pyproject.toml
--rw-r--r--   0        0        0       21 2023-03-21 11:15:21.821516 nhssynth-0.3.1/src/nhssynth/cli/__init__.py
--rw-r--r--   0        0        0     3437 2023-04-26 19:31:33.656962 nhssynth-0.3.1/src/nhssynth/cli/common_arguments.py
--rw-r--r--   0        0        0     8854 2023-04-27 13:25:22.472512 nhssynth-0.3.1/src/nhssynth/cli/config.py
--rw-r--r--   0        0        0     1826 2023-04-26 19:31:33.657526 nhssynth-0.3.1/src/nhssynth/cli/model_arguments.py
--rw-r--r--   0        0        0     6768 2023-04-26 19:31:33.657824 nhssynth-0.3.1/src/nhssynth/cli/module_arguments.py
--rw-r--r--   0        0        0     7421 2023-05-05 14:21:02.300157 nhssynth-0.3.1/src/nhssynth/cli/module_setup.py
--rw-r--r--   0        0        0     1396 2023-04-26 19:31:33.658300 nhssynth-0.3.1/src/nhssynth/cli/run.py
--rw-r--r--   0        0        0       82 2023-04-04 13:59:35.254031 nhssynth-0.3.1/src/nhssynth/common/__init__.py
--rw-r--r--   0        0        0      385 2023-04-27 13:22:15.158073 nhssynth-0.3.1/src/nhssynth/common/common.py
--rw-r--r--   0        0        0     3613 2023-04-26 19:31:33.658743 nhssynth-0.3.1/src/nhssynth/common/constants.py
--rw-r--r--   0        0        0      376 2023-04-26 19:31:33.658992 nhssynth-0.3.1/src/nhssynth/common/debugging.py
--rw-r--r--   0        0        0     2369 2023-04-27 13:23:24.877565 nhssynth-0.3.1/src/nhssynth/common/dicts.py
--rw-r--r--   0        0        0     3149 2023-04-27 13:23:45.952265 nhssynth-0.3.1/src/nhssynth/common/io.py
--rw-r--r--   0        0        0      582 2023-04-26 19:31:33.659388 nhssynth-0.3.1/src/nhssynth/common/strings.py
--rw-r--r--   0        0        0        0 2023-03-09 10:01:33.834460 nhssynth-0.3.1/src/nhssynth/modules/__init__.py
--rw-r--r--   0        0        0       20 2023-03-06 16:05:17.363712 nhssynth-0.3.1/src/nhssynth/modules/dataloader/__init__.py
--rw-r--r--   0        0        0     4082 2023-04-12 15:32:23.986086 nhssynth-0.3.1/src/nhssynth/modules/dataloader/io.py
--rw-r--r--   0        0        0     5253 2023-04-12 15:46:13.535858 nhssynth-0.3.1/src/nhssynth/modules/dataloader/metadata.py
--rw-r--r--   0        0        0    17033 2023-05-05 14:21:02.300580 nhssynth-0.3.1/src/nhssynth/modules/dataloader/metatransformer.py
--rw-r--r--   0        0        0     1328 2023-05-05 14:21:02.301252 nhssynth-0.3.1/src/nhssynth/modules/dataloader/run.py
--rw-r--r--   0        0        0       21 2023-03-07 10:58:04.573024 nhssynth-0.3.1/src/nhssynth/modules/evaluation/__init__.py
--rw-r--r--   0        0        0    14071 2023-04-26 19:31:33.660200 nhssynth-0.3.1/src/nhssynth/modules/evaluation/full_report.py
--rw-r--r--   0        0        0     2622 2023-05-05 14:21:02.301903 nhssynth-0.3.1/src/nhssynth/modules/evaluation/io.py
--rw-r--r--   0        0        0     3031 2023-04-11 16:04:10.935343 nhssynth-0.3.1/src/nhssynth/modules/evaluation/metrics.py
--rw-r--r--   0        0        0     1835 2023-04-26 19:31:33.660620 nhssynth-0.3.1/src/nhssynth/modules/evaluation/run.py
--rw-r--r--   0        0        0       48 2023-04-26 19:31:33.660900 nhssynth-0.3.1/src/nhssynth/modules/model/__init__.py
--rw-r--r--   0        0        0     4345 2023-04-28 11:01:27.969421 nhssynth-0.3.1/src/nhssynth/modules/model/common/DPMixin.py
--rw-r--r--   0        0        0     6391 2023-05-05 15:47:58.057779 nhssynth-0.3.1/src/nhssynth/modules/model/common/Model.py
--rw-r--r--   0        0        0     3425 2023-05-05 14:21:02.302352 nhssynth-0.3.1/src/nhssynth/modules/model/io.py
--rw-r--r--   0        0        0     1648 2023-04-26 19:31:33.661707 nhssynth-0.3.1/src/nhssynth/modules/model/models/DPVAE.py
--rw-r--r--   0        0        0     9945 2023-05-05 15:52:45.345428 nhssynth-0.3.1/src/nhssynth/modules/model/models/VAE.py
--rw-r--r--   0        0        0      129 2023-04-26 19:31:33.662043 nhssynth-0.3.1/src/nhssynth/modules/model/models/__init__.py
--rw-r--r--   0        0        0     2238 2023-05-05 14:21:02.302796 nhssynth-0.3.1/src/nhssynth/modules/model/run.py
--rw-r--r--   0        0        0       21 2023-03-07 10:58:07.632275 nhssynth-0.3.1/src/nhssynth/modules/plotting/__init__.py
--rw-r--r--   0        0        0     2589 2023-05-05 14:21:02.303228 nhssynth-0.3.1/src/nhssynth/modules/plotting/io.py
--rw-r--r--   0        0        0     6421 2023-04-13 19:24:58.843577 nhssynth-0.3.1/src/nhssynth/modules/plotting/plots.py
--rw-r--r--   0        0        0      727 2023-04-13 12:33:18.866696 nhssynth-0.3.1/src/nhssynth/modules/plotting/run.py
--rw-r--r--   0        0        0       21 2023-03-07 10:58:13.024183 nhssynth-0.3.1/src/nhssynth/modules/structure/__init__.py
--rw-r--r--   0        0        0       85 2023-03-07 10:58:26.227434 nhssynth-0.3.1/src/nhssynth/modules/structure/run.py
--rw-r--r--   0        0        0    10163 1970-01-01 00:00:00.000000 nhssynth-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-03-31 11:03:40.629205 nhssynth-0.4.0/LICENSE
+-rw-r--r--   0        0        0     8773 2023-07-17 19:18:22.721883 nhssynth-0.4.0/README.md
+-rw-r--r--   0        0        0     1898 2023-07-18 08:12:24.276413 nhssynth-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-03-21 11:15:21.821516 nhssynth-0.4.0/src/nhssynth/cli/__init__.py
+-rw-r--r--   0        0        0     3556 2023-07-17 19:18:22.733434 nhssynth-0.4.0/src/nhssynth/cli/common_arguments.py
+-rw-r--r--   0        0        0     8854 2023-05-10 13:14:43.837250 nhssynth-0.4.0/src/nhssynth/cli/config.py
+-rw-r--r--   0        0        0     1826 2023-04-26 19:31:33.657526 nhssynth-0.4.0/src/nhssynth/cli/model_arguments.py
+-rw-r--r--   0        0        0     6820 2023-07-17 19:18:22.733805 nhssynth-0.4.0/src/nhssynth/cli/module_arguments.py
+-rw-r--r--   0        0        0     7421 2023-07-17 19:18:22.734062 nhssynth-0.4.0/src/nhssynth/cli/module_setup.py
+-rw-r--r--   0        0        0     1396 2023-04-26 19:31:33.658300 nhssynth-0.4.0/src/nhssynth/cli/run.py
+-rw-r--r--   0        0        0       82 2023-04-04 13:59:35.254031 nhssynth-0.4.0/src/nhssynth/common/__init__.py
+-rw-r--r--   0        0        0      385 2023-04-27 13:22:15.158073 nhssynth-0.4.0/src/nhssynth/common/common.py
+-rw-r--r--   0        0        0     3411 2023-07-17 19:18:22.734745 nhssynth-0.4.0/src/nhssynth/common/constants.py
+-rw-r--r--   0        0        0      376 2023-04-26 19:31:33.658992 nhssynth-0.4.0/src/nhssynth/common/debugging.py
+-rw-r--r--   0        0        0     2369 2023-04-27 13:23:24.877565 nhssynth-0.4.0/src/nhssynth/common/dicts.py
+-rw-r--r--   0        0        0     3149 2023-04-27 13:23:45.952265 nhssynth-0.4.0/src/nhssynth/common/io.py
+-rw-r--r--   0        0        0      582 2023-04-26 19:31:33.659388 nhssynth-0.4.0/src/nhssynth/common/strings.py
+-rw-r--r--   0        0        0        0 2023-03-09 10:01:33.834460 nhssynth-0.4.0/src/nhssynth/modules/__init__.py
+-rw-r--r--   0        0        0       21 2023-07-17 19:18:22.735148 nhssynth-0.4.0/src/nhssynth/modules/dataloader/__init__.py
+-rw-r--r--   0        0        0     3882 2023-07-17 19:18:22.735402 nhssynth-0.4.0/src/nhssynth/modules/dataloader/io.py
+-rw-r--r--   0        0        0    11433 2023-07-17 19:18:22.735655 nhssynth-0.4.0/src/nhssynth/modules/dataloader/metadata.py
+-rw-r--r--   0        0        0    11881 2023-07-18 08:11:26.033379 nhssynth-0.4.0/src/nhssynth/modules/dataloader/metatransformer.py
+-rw-r--r--   0        0        0     3611 2023-07-17 19:18:22.736200 nhssynth-0.4.0/src/nhssynth/modules/dataloader/missingness.py
+-rw-r--r--   0        0        0     1220 2023-07-18 08:11:26.033558 nhssynth-0.4.0/src/nhssynth/modules/dataloader/run.py
+-rw-r--r--   0        0        0      125 2023-07-17 19:18:22.736677 nhssynth-0.4.0/src/nhssynth/modules/dataloader/transformers/__init__.py
+-rw-r--r--   0        0        0     1315 2023-07-18 08:11:26.033735 nhssynth-0.4.0/src/nhssynth/modules/dataloader/transformers/categorical.py
+-rw-r--r--   0        0        0     4128 2023-07-18 08:11:26.033910 nhssynth-0.4.0/src/nhssynth/modules/dataloader/transformers/continuous.py
+-rw-r--r--   0        0        0      946 2023-07-18 08:11:26.034078 nhssynth-0.4.0/src/nhssynth/modules/dataloader/transformers/datetime.py
+-rw-r--r--   0        0        0     1075 2023-07-18 08:11:26.034216 nhssynth-0.4.0/src/nhssynth/modules/dataloader/transformers/generic.py
+-rw-r--r--   0        0        0       21 2023-03-07 10:58:04.573024 nhssynth-0.4.0/src/nhssynth/modules/evaluation/__init__.py
+-rw-r--r--   0        0        0    14071 2023-06-07 10:04:58.683189 nhssynth-0.4.0/src/nhssynth/modules/evaluation/full_report.py
+-rw-r--r--   0        0        0     2605 2023-07-17 19:18:22.738439 nhssynth-0.4.0/src/nhssynth/modules/evaluation/io.py
+-rw-r--r--   0        0        0     3031 2023-04-11 16:04:10.935343 nhssynth-0.4.0/src/nhssynth/modules/evaluation/metrics.py
+-rw-r--r--   0        0        0     1835 2023-06-26 13:59:10.658401 nhssynth-0.4.0/src/nhssynth/modules/evaluation/run.py
+-rw-r--r--   0        0        0       48 2023-04-26 19:31:33.660900 nhssynth-0.4.0/src/nhssynth/modules/model/__init__.py
+-rw-r--r--   0        0        0     6634 2023-07-18 08:11:26.034691 nhssynth-0.4.0/src/nhssynth/modules/model/common/Model.py
+-rw-r--r--   0        0        0     4345 2023-07-17 19:18:22.738937 nhssynth-0.4.0/src/nhssynth/modules/model/common/dp.py
+-rw-r--r--   0        0        0     3484 2023-07-17 19:18:22.739182 nhssynth-0.4.0/src/nhssynth/modules/model/io.py
+-rw-r--r--   0        0        0      129 2023-07-17 19:18:22.739961 nhssynth-0.4.0/src/nhssynth/modules/model/models/__init__.py
+-rw-r--r--   0        0        0     1643 2023-07-17 19:18:22.739444 nhssynth-0.4.0/src/nhssynth/modules/model/models/dpvae.py
+-rw-r--r--   0        0        0    10165 2023-07-17 19:18:22.739716 nhssynth-0.4.0/src/nhssynth/modules/model/models/vae.py
+-rw-r--r--   0        0        0     2337 2023-07-17 19:18:22.740199 nhssynth-0.4.0/src/nhssynth/modules/model/run.py
+-rw-r--r--   0        0        0       21 2023-03-07 10:58:07.632275 nhssynth-0.4.0/src/nhssynth/modules/plotting/__init__.py
+-rw-r--r--   0        0        0     2589 2023-05-05 14:21:02.303228 nhssynth-0.4.0/src/nhssynth/modules/plotting/io.py
+-rw-r--r--   0        0        0     6421 2023-04-13 19:24:58.843577 nhssynth-0.4.0/src/nhssynth/modules/plotting/plots.py
+-rw-r--r--   0        0        0      727 2023-04-13 12:33:18.866696 nhssynth-0.4.0/src/nhssynth/modules/plotting/run.py
+-rw-r--r--   0        0        0       21 2023-03-07 10:58:13.024183 nhssynth-0.4.0/src/nhssynth/modules/structure/__init__.py
+-rw-r--r--   0        0        0       85 2023-03-07 10:58:26.227434 nhssynth-0.4.0/src/nhssynth/modules/structure/run.py
+-rw-r--r--   0        0        0    10094 1970-01-01 00:00:00.000000 nhssynth-0.4.0/PKG-INFO
```

### Comparing `nhssynth-0.3.1/LICENSE` & `nhssynth-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nhssynth-0.3.1/README.md` & `nhssynth-0.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ![Lines of Code](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/HarrisonWilde/1ab4eefed81ec381e29f7d4feb9856bc/raw/loc.json)
 ![Percentage Comments](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/HarrisonWilde/1ab4eefed81ec381e29f7d4feb9856bc/raw/comments.json)
 [![Snyk Package Health](https://snyk.io/advisor/python/nhssynth/badge.svg)](https://snyk.io/advisor/python/nhssynth)
 
 </div>
 <div align="center">
 
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nhssynth)](https://www.python.org/downloads/release/python-3100/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nhssynth)](https://www.python.org/downloads/release/python-3113/)
 [![PyPI - Package Status](https://img.shields.io/pypi/status/nhssynth)](https://pypi.org/project/nhssynth/)
 [![PyPI - Latest Release](https://img.shields.io/pypi/v/nhssynth)](https://pypi.org/project/nhssynth/)
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/nhssynth)](https://pypi.org/project/nhssynth/)
 [![PyPI - License](https://img.shields.io/pypi/l/nhssynth)](https://github.com/nhsx/nhssynth/blob/main/LICENSE)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1)](https://pycqa.github.io/isort/)
 
@@ -33,16 +33,14 @@
 
 # NHS Synth
 
 ## About
 
 This repository currently consists of a Python package alongside research and investigative materials covering the effectiveness of the package and synthetic data more generally when applied to NHS use cases. See the internal [project description](https://nhsx.github.io/nhsx-internship-projects/synthetic-data-exploration-vae/) for more information.
 
-_**Note:** No data, public or private are shared in this repository._
-
 ## Getting Started
 
 ### Project Structure
 
 - The main package and codebase is found in [`src/nhssynth`](src/nhssynth/) (see [Usage](#usage) below for more information)
 - Accompanying materials are available in the [`docs`](docs/) folder:
   - The components used to create the GitHub Pages [documentation site](https://nhsx.github.io/NHSSynth/)
@@ -64,15 +62,15 @@
 git clone git@github.com:pytorch/csprng.git
 cd csprng
 git branch release "v0.2.2-rc1"
 git checkout release
 python setup.py install
 ```
 
-#### Advanced Usage
+#### Advanced Installation
 
 If you intend on contributing or working with the codebase directly, or if you want to reproduce the results of this project, follow the steps below:
 
 1. Clone the repo
 2. Ensure one of the required versions of Python is installed
 3. Install [`poetry`](https://python-poetry.org/docs/#installation)
 4. Instantiate a virtual environment, e.g. via `python -m venv nhssynth`
@@ -106,15 +104,15 @@
 
 ### Roadmap
 
 See the [open issues](https://github.com/nhsx/NHSSynth/issues) for a list of proposed features (and known bugs). Our [milestones](https://github.com/nhsx/NHSSynth/milestones) represent longer term goals for the project.
 
 ### Contributing
 
-Any contributions you wish to make are **greatly appreciated**, we encourage you to first raise an issue to discuss with the maintainers. If you are interested in contributing, please follow these steps:
+Contributions are welcome! We encourage you to first raise an issue with your proposed contribution to enable discussion with the maintainers. After that, please follow these steps:
 
 1. Fork the project
 2. Create your branch (`git checkout -b <yourusername>/<featurename>`)
 3. Commit your changes (`git commit -m 'Add some amazing feature'`)
 4. Push to the branch (`git push origin <yourusername>/<featurename>`)
 5. Open a PR and we will try to get it merged!
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
    tests.json) ![Lines of Code](https://img.shields.io/endpoint?url=https://
 gist.githubusercontent.com/HarrisonWilde/1ab4eefed81ec381e29f7d4feb9856bc/raw/
  loc.json) ![Percentage Comments](https://img.shields.io/endpoint?url=https://
 gist.githubusercontent.com/HarrisonWilde/1ab4eefed81ec381e29f7d4feb9856bc/raw/
 comments.json) [![Snyk Package Health](https://snyk.io/advisor/python/nhssynth/
              badge.svg)](https://snyk.io/advisor/python/nhssynth)
   [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nhssynth)]
-   (https://www.python.org/downloads/release/python-3100/) [![PyPI - Package
+   (https://www.python.org/downloads/release/python-3113/) [![PyPI - Package
 Status](https://img.shields.io/pypi/status/nhssynth)](https://pypi.org/project/
  nhssynth/) [![PyPI - Latest Release](https://img.shields.io/pypi/v/nhssynth)]
  (https://pypi.org/project/nhssynth/) [![PyPI - Wheel](https://img.shields.io/
  pypi/wheel/nhssynth)](https://pypi.org/project/nhssynth/) [![PyPI - License]
   (https://img.shields.io/pypi/l/nhssynth)](https://github.com/nhsx/nhssynth/
     blob/main/LICENSE) [![Code style: black](https://img.shields.io/badge/
  code%20style-black-000000)](https://github.com/psf/black) [![Imports: isort]
@@ -22,84 +22,83 @@
                                     [Logo]
                              Explore_the_docs_Â»
 
 # NHS Synth ## About This repository currently consists of a Python package
 alongside research and investigative materials covering the effectiveness of
 the package and synthetic data more generally when applied to NHS use cases.
 See the internal [project description](https://nhsx.github.io/nhsx-internship-
-projects/synthetic-data-exploration-vae/) for more information. _**Note:** No
-data, public or private are shared in this repository._ ## Getting Started ###
-Project Structure - The main package and codebase is found in [`src/nhssynth`]
-(src/nhssynth/) (see [Usage](#usage) below for more information) - Accompanying
-materials are available in the [`docs`](docs/) folder: - The components used to
-create the GitHub Pages [documentation site](https://nhsx.github.io/NHSSynth/
-) - A [report](docs/reports/report.pdf) summarising the previous iteration of
-this project - A [model card](docs/model_card.md) providing more information
-about the VAE with Differential Privacy - Numerous exemplar configurations are
-found in [`config`](config/) - Empty [`data`](data/) and [`experiments`]
-(experiments/) folders are provided; these are the default locations for inputs
-and outputs when running the project using the provided [CLI](../src/nhssynth/
-cli/) module - Pre-processing notebooks for specific datasets used to assess
-the approach and other non-core code can be found in [`auxiliary`](../
-auxiliary/) ### Installation For general usage, we recommend installing the
-package via `pip install nhssynth` in a supported python version environment.
-You can then `import` the package's [modules](src/nhssynth/modules/) and use
-them in your projects, or interact with the package directly via the [CLI](src/
-nhssynth/cli/), which is accessed using the `nhssynth` command (see [Usage]
-(#usage) for more information). #### Secure Mode Note that in order to train a
-generator in *secure mode* (see the [documentation](https://nhsx.github.io/
-NHSSynth/secure_mode/) for details) you will need to install the PyTorch
-extension package [`csprng`](https://github.com/pytorch/csprng) separately.
-Currently this package's dependencies are not compatible with recent versions
-of PyTorch (the author's plan on rectifying this - watch this space), so you
-will need to install it manually; for this we recommend following the
-instructions below: ```bash git clone git@github.com:pytorch/csprng.git cd
-csprng git branch release "v0.2.2-rc1" git checkout release python setup.py
-install ``` #### Advanced Usage If you intend on contributing or working with
-the codebase directly, or if you want to reproduce the results of this project,
-follow the steps below: 1. Clone the repo 2. Ensure one of the required
-versions of Python is installed 3. Install [`poetry`](https://python-
-poetry.org/docs/#installation) 4. Instantiate a virtual environment, e.g. via
-`python -m venv nhssynth` 3. Activate the virtual environment, e.g. via `source
-nhssynth/bin/activate` 4. Install the project dependencies with `poetry
-install` (optionally install the dev dependencies `--with dev` to work with the
-[auxiliary notebooks](auxiliary/), or `--with docs` to work with the
-[documentation](docs/)) 5. You can then interact with the package in one of two
-ways: - Via the [CLI](src/nhssynth/cli/) module using `nhssynth ...` - Through
-building the package with `poetry build` and using it in an existing project
-(`import nhssynth`). You can then actively develop the package and test it. ###
-Usage This package comprises a set of modules that can be run individually, as
-part of a pipeline, or via a configuration file. These options are available
-via the `nhssynth` command: ``` nhssynth  -- nhssynth pipeline -- nhssynth
-config -c  -- ``` To see the modules that are available and their corresponding
-arguments, run `nhssynth --help` and `nhssynth  --help` respectively.
-Configuration files can be used to run the pipeline or a chosen set of modules.
-They should be placed in the [`config`](config/) folder and their layout should
-match that of the examples provided. They can be run as in the latter case
-above by providing their filename (without the `.yaml` extension). You can also
-override any of the arguments provided in the configuration file by passing
-them as arguments in the command line. To ensure reproducibility, you should
-always specify a `--seed` value and provide the `--save-config` flag to dump
-the exact configuration specified / inferred for the run. This configuration
-file can then be used in the future to reproduce the exact same run or shared
-with others to run the same configuration on their dataset, etc. The figure
-below shows the structure and workflow of the package and its modules. ![]
-(docs/modules.png) View a visualisation of the codebase [here](https://mango-
-dune-07a8b7110.1.azurestaticapps.net/?repo=nhsx%2Fnhssynth)! ### Roadmap See
-the [open issues](https://github.com/nhsx/NHSSynth/issues) for a list of
-proposed features (and known bugs). Our [milestones](https://github.com/nhsx/
-NHSSynth/milestones) represent longer term goals for the project. ###
-Contributing Any contributions you wish to make are **greatly appreciated**, we
-encourage you to first raise an issue to discuss with the maintainers. If you
-are interested in contributing, please follow these steps: 1. Fork the project
-2. Create your branch (`git checkout -b /`) 3. Commit your changes (`git commit
--m 'Add some amazing feature'`) 4. Push to the branch (`git push origin /`) 5.
-Open a PR and we will try to get it merged! _See [CONTRIBUTING.md](./
-CONTRIBUTING.md) for detailed guidance._ Thanks to everyone that has
-contributed so far!
+projects/synthetic-data-exploration-vae/) for more information. ## Getting
+Started ### Project Structure - The main package and codebase is found in
+[`src/nhssynth`](src/nhssynth/) (see [Usage](#usage) below for more
+information) - Accompanying materials are available in the [`docs`](docs/
+) folder: - The components used to create the GitHub Pages [documentation site]
+(https://nhsx.github.io/NHSSynth/) - A [report](docs/reports/report.pdf)
+summarising the previous iteration of this project - A [model card](docs/
+model_card.md) providing more information about the VAE with Differential
+Privacy - Numerous exemplar configurations are found in [`config`](config/) -
+Empty [`data`](data/) and [`experiments`](experiments/) folders are provided;
+these are the default locations for inputs and outputs when running the project
+using the provided [CLI](../src/nhssynth/cli/) module - Pre-processing
+notebooks for specific datasets used to assess the approach and other non-core
+code can be found in [`auxiliary`](../auxiliary/) ### Installation For general
+usage, we recommend installing the package via `pip install nhssynth` in a
+supported python version environment. You can then `import` the package's
+[modules](src/nhssynth/modules/) and use them in your projects, or interact
+with the package directly via the [CLI](src/nhssynth/cli/), which is accessed
+using the `nhssynth` command (see [Usage](#usage) for more information). ####
+Secure Mode Note that in order to train a generator in *secure mode* (see the
+[documentation](https://nhsx.github.io/NHSSynth/secure_mode/) for details) you
+will need to install the PyTorch extension package [`csprng`](https://
+github.com/pytorch/csprng) separately. Currently this package's dependencies
+are not compatible with recent versions of PyTorch (the author's plan on
+rectifying this - watch this space), so you will need to install it manually;
+for this we recommend following the instructions below: ```bash git clone
+git@github.com:pytorch/csprng.git cd csprng git branch release "v0.2.2-rc1" git
+checkout release python setup.py install ``` #### Advanced Installation If you
+intend on contributing or working with the codebase directly, or if you want to
+reproduce the results of this project, follow the steps below: 1. Clone the
+repo 2. Ensure one of the required versions of Python is installed 3. Install
+[`poetry`](https://python-poetry.org/docs/#installation) 4. Instantiate a
+virtual environment, e.g. via `python -m venv nhssynth` 3. Activate the virtual
+environment, e.g. via `source nhssynth/bin/activate` 4. Install the project
+dependencies with `poetry install` (optionally install the dev dependencies `--
+with dev` to work with the [auxiliary notebooks](auxiliary/), or `--with docs`
+to work with the [documentation](docs/)) 5. You can then interact with the
+package in one of two ways: - Via the [CLI](src/nhssynth/cli/) module using
+`nhssynth ...` - Through building the package with `poetry build` and using it
+in an existing project (`import nhssynth`). You can then actively develop the
+package and test it. ### Usage This package comprises a set of modules that can
+be run individually, as part of a pipeline, or via a configuration file. These
+options are available via the `nhssynth` command: ``` nhssynth  -- nhssynth
+pipeline -- nhssynth config -c  -- ``` To see the modules that are available
+and their corresponding arguments, run `nhssynth --help` and `nhssynth  --help`
+respectively. Configuration files can be used to run the pipeline or a chosen
+set of modules. They should be placed in the [`config`](config/) folder and
+their layout should match that of the examples provided. They can be run as in
+the latter case above by providing their filename (without the `.yaml`
+extension). You can also override any of the arguments provided in the
+configuration file by passing them as arguments in the command line. To ensure
+reproducibility, you should always specify a `--seed` value and provide the `--
+save-config` flag to dump the exact configuration specified / inferred for the
+run. This configuration file can then be used in the future to reproduce the
+exact same run or shared with others to run the same configuration on their
+dataset, etc. The figure below shows the structure and workflow of the package
+and its modules. ![](docs/modules.png) View a visualisation of the codebase
+[here](https://mango-dune-07a8b7110.1.azurestaticapps.net/
+?repo=nhsx%2Fnhssynth)! ### Roadmap See the [open issues](https://github.com/
+nhsx/NHSSynth/issues) for a list of proposed features (and known bugs). Our
+[milestones](https://github.com/nhsx/NHSSynth/milestones) represent longer term
+goals for the project. ### Contributing Contributions are welcome! We encourage
+you to first raise an issue with your proposed contribution to enable
+discussion with the maintainers. After that, please follow these steps: 1. Fork
+the project 2. Create your branch (`git checkout -b /`) 3. Commit your changes
+(`git commit -m 'Add some amazing feature'`) 4. Push to the branch (`git push
+origin /`) 5. Open a PR and we will try to get it merged! _See
+[CONTRIBUTING.md](./CONTRIBUTING.md) for detailed guidance._ Thanks to everyone
+that has contributed so far!
                [https://contrib.rocks/image?repo=nhsx/nhssynth]
 This codebase builds on previous NHSX Analytics Unit PhD internships
 contextualising and investigating the potential use of Variational Auto
 Encoders (VAEs) for synthetic data generation. These were undertaken by Dominic
 Danks and David Brind. ### License Distributed under the MIT License. _See
 [LICENSE](./LICENSE) for more information._ ### Contact This project is under
 active development by [@HarrisonWilde](https://github.com/HarrisonWilde). For
```

### Comparing `nhssynth-0.3.1/pyproject.toml` & `nhssynth-0.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nhssynth"
-version = "0.3.1"
+version = "0.4.0"
 description = "Synthetic data generation pipeline leveraging a Differentially Private Variational Auto Encoder assessed using a variety of metrics"
 authors = ["HarrisonWilde <harrisondwilde@outlook.com>"]
 maintainers = ["NHSE TDAU <england.tdau@nhs.net>"]
 license = "MIT"
 readme = ["README.md"]
 repository = "https://github.com/nhsx/NHSSynth"
 keywords = ["synthetic data", "privacy", "fairness", "machine learning"]
@@ -14,46 +14,47 @@
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/nhsx/NHSSynth/issues"
 "Docs" = "https://nhsx.github.io/NHSSynth"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.11"
-setuptools = "^67.6.1"
+pandas = "^2.0.1"
+scikit-learn = "^1.2.2"
 tqdm = "^4.65.0"
 gower = "^0.1.2"
 pyyaml = "^6.0"
-sdmetrics = "^0.9.3"
-pandas = "^1.5.3"
-rdt = "^1.4.0"
-sdv = "^1.0.0"
-torch = "1.13.1"
+torch = "^2.0.1"
 opacus = "^1.4.0"
+requests = "^2.31.0"
+tornado = "^6.3.2"
+sdmetrics = "^0.10.1"
 
 [tool.poetry.scripts]
 nhssynth = 'nhssynth.cli:run'
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 mkdocstrings = {extras = ["python-legacy"], version = "^0.20.0"}
 mkdocs-material = "^9.1.4"
 mkdocs-gen-files = "^0.4.0"
 mkdocs-literate-nav = "^0.6.0"
 mkdocs-section-index = "^0.3.5"
 mkdocs-git-revision-date-localized-plugin = "^1.2.0"
-pymdown-extensions = "^9.10"
+pymdown-extensions = "^10.0.1"
 
 [tool.poetry.group.aux]
 optional = true
 
 [tool.poetry.group.aux.dependencies]
 jupyter = "^1.0.0"
 notebook = "^6.5.4"
+pycox = "^0.2.3"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
```

### Comparing `nhssynth-0.3.1/src/nhssynth/cli/common_arguments.py` & `nhssynth-0.4.0/src/nhssynth/cli/common_arguments.py`

 * *Files 9% similar despite different names*

```diff
@@ -75,17 +75,31 @@
     return get_parser
 
 
 COMMON_PARSERS: Final = {
     "dataset": get_dataset_parser,
     "core": get_core_parser,
     "metadata": suffix_parser_generator(
-        "metadata", "filename of the metadata, NOTE that `dataloader` attempts to read this from `<DATA_DIR>`"
+        "metadata",
+        "filename of the metadata, NOTE that `dataloader` attempts to read this from `<DATA_DIR>`",
+    ),
+    "typed": suffix_parser_generator(
+        "typed",
+        "filename of the typed data",
+    ),
+    "transformed": suffix_parser_generator(
+        "transformed",
+        "filename of the transformed data",
     ),
-    "typed": suffix_parser_generator("typed", "filename of the typed data"),
-    "prepared": suffix_parser_generator("prepared", "filename of the prepared data"),
     "metatransformer": suffix_parser_generator(
-        "metatransformer", "filename of the `MetaTransformer` used to prepare the data"
+        "metatransformer",
+        "filename of the `MetaTransformer` used to prepare the data",
+    ),
+    "synthetic": suffix_parser_generator(
+        "synthetic",
+        "filename of the synthetic data",
+    ),
+    "report": suffix_parser_generator(
+        "report",
+        "filename of the (collection of) report(s)",
     ),
-    "synthetic": suffix_parser_generator("synthetic", "filename of the synthetic data"),
-    "report": suffix_parser_generator("report", "filename of the (collection of) report(s)"),
 }
```

### Comparing `nhssynth-0.3.1/src/nhssynth/cli/config.py` & `nhssynth-0.4.0/src/nhssynth/cli/config.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.3.1/src/nhssynth/cli/model_arguments.py` & `nhssynth-0.4.0/src/nhssynth/cli/model_arguments.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.3.1/src/nhssynth/cli/module_arguments.py` & `nhssynth-0.4.0/src/nhssynth/cli/module_arguments.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Define arguments for each of the modules' CLI sub-parsers."""
 import argparse
 
 from nhssynth.cli.model_arguments import add_model_specific_args
 from nhssynth.common.constants import *
+from nhssynth.modules.dataloader.metadata import MISSINGNESS_STRATEGIES
 from nhssynth.modules.model import MODELS
 
 
 class AllChoicesDefault(argparse.Action):
     """
     Customized argparse action for defaulting to the full list of choices if only the flag is supplied.
 
@@ -38,29 +39,30 @@
     group.add_argument(
         "--index-col",
         default=None,
         choices=[None, 0],
         help="indicate whether the csv file's 0th column is an index column, such that pandas can ignore it",
     )
     group.add_argument(
-        "--allow-null-transformers",
-        action="store_true",
-        help="allow null / None transformers, i.e. leave some columns as they are",
-    )
-    group.add_argument(
         "--collapse-yaml",
         action="store_true",
         help="use aliases and anchors in the output metadata yaml, this will make it much more compact",
     )
     group.add_argument(
-        "--synthesizer",
+        "--missingness",
         type=str,
-        default="TVAE",
-        choices=list(SDV_SYNTHESIZERS.keys()),
-        help="pick a synthesizer to use (note this can also be specified in the model module, these must match)",
+        default="augment",
+        choices=MISSINGNESS_STRATEGIES,
+        help="how to handle missing values in the dataset",
+    )
+    group.add_argument(
+        "--impute",
+        type=str,
+        default=None,
+        help="the imputation strategy to use, ONLY USED if <MISSINGNESS> is set to 'impute', choose from: 'mean', 'median', 'mode', or any specific value (e.g. '0')",
     )
 
 
 def add_structure_args(parser: argparse.ArgumentParser, group_title: str, overrides: bool = False) -> None:
     pass
 
 
@@ -68,15 +70,15 @@
     """Adds arguments to an existing model module sub-parser instance."""
     group = parser.add_argument_group(title=group_title)
     group.add_argument(
         "--architecture",
         type=str,
         nargs="+",
         default=["VAE"],
-        choices=list(MODELS.keys()),
+        choices=MODELS,
         help="the model architecture(s) to train",
     )
     group.add_argument(
         "--repeats",
         type=int,
         default=1,
         help="how many times to repeat the training process per model architecture (<SEED> is incremented each time)",
@@ -154,16 +156,16 @@
 def generate_evaluation_arg(group, name):
     group.add_argument(
         f"--{'-'.join(name.split()).lower()}-metrics",
         type=str,
         default=None,
         nargs="*",
         action=AllChoicesDefault,
-        const=list(SDV_METRICS[name].keys()),
-        choices=list(SDV_METRICS[name].keys()),
+        const=SDV_METRICS[name],
+        choices=SDV_METRICS[name],
         help=f"run the {name.lower()} evaluation",
     )
 
 
 def add_evaluation_args(parser: argparse.ArgumentParser, group_title: str, overrides: bool = False) -> None:
     """Adds arguments to an existing evaluation module sub-parser instance."""
     group = parser.add_argument_group(title=group_title)
```

### Comparing `nhssynth-0.3.1/src/nhssynth/cli/module_setup.py` & `nhssynth-0.4.0/src/nhssynth/cli/module_setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,55 +90,55 @@
     "plotting",
 ]  # NOTE this determines the order of a pipeline run
 
 MODULE_MAP: Final = {
     "dataloader": ModuleConfig(
         func=dataloader.run,
         add_args=add_dataloader_args,
-        description="Run the Data Loader module, to prepare the chosen dataset for use in other modules.",
+        description="run the data loader module, to prepare the chosen dataset for use in other modules",
         help="prepare the dataset",
-        common_parsers=["metadata", "typed", "prepared", "metatransformer"],
+        common_parsers=["metadata", "typed", "transformed", "metatransformer"],
     ),
     "structure": ModuleConfig(
         func=structure.run,
         add_args=add_structure_args,
-        description="Run the Structural Discovery module, to learn a structural model for use in training and evaluation.",
+        description="run the structural discovery module, to learn a structural model for use in training and evaluation",
         help="discover structure",
     ),
     "model": ModuleConfig(
         func=model.run,
         add_args=add_model_args,
-        description="Run the Model Architecture module, to train a synthetic data generator.",
+        description="run the model architecture module, to train a synthetic data generator",
         help="train a model",
-        common_parsers=["prepared", "metatransformer", "synthetic"],
+        common_parsers=["transformed", "metatransformer", "synthetic"],
     ),
     "evaluation": ModuleConfig(
         func=evaluation.run,
         add_args=add_evaluation_args,
-        description="Run the Evaluation module, to evaluate an experiment.",
+        description="run the evaluation module, to evaluate an experiment",
         help="evaluate an experiment",
         common_parsers=["metadata", "typed", "synthetic", "report"],
     ),
     "plotting": ModuleConfig(
         func=plotting.run,
         add_args=add_plotting_args,
-        description="Run the Plotting module, to generate plots for a given model and / or evaluation.",
+        description="run the plotting module, to generate plots for a given model and / or evaluation",
         help="generate plots",
         common_parsers=["typed", "synthetic", "report"],
     ),
     "pipeline": ModuleConfig(
         func=run_pipeline,
         add_args=add_pipeline_args,
-        description="Run the full pipeline.",
+        description="run the full pipeline.",
         help="run the full pipeline",
     ),
     "config": ModuleConfig(
         func=None,
         add_args=add_config_args,
-        description="Run module(s) according to configuration specified by a file in `config/`. Note that you can override parts of the configuration on the fly by using the usual CLI flags.",
+        description="run module(s) according to configuration specified by a file in `config/`; note that you can override parts of the configuration on the fly by using the usual CLI flags",
         help="run module(s) in line with a passed configuration file",
     ),
 }
 
 ### EDIT ABOVE HERE TO ADD MODULES / ALTER PIPELINE BEHAVIOUR
 
 VALID_MODULES = {x for x in MODULE_MAP.keys() if x not in {"pipeline", "config"}}
```

### Comparing `nhssynth-0.3.1/src/nhssynth/cli/run.py` & `nhssynth-0.4.0/src/nhssynth/cli/run.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.3.1/src/nhssynth/common/constants.py` & `nhssynth-0.4.0/src/nhssynth/common/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Define all of the common constants used throughout the project."""
 from time import strftime
 from typing import Final
 
 import torch.nn as nn
 from sdmetrics.single_table import *
-from sdv.single_table import *
 
 TIME: Final = strftime("%Y_%m_%d___%H_%M_%S")
 
 TRACKED_METRICS: Final = [
     "ELBO",
     "KLD",
     "ReconstructionLoss",
@@ -22,21 +21,14 @@
     "relu": nn.ReLU,
     "selu": nn.SELU,
     "leaky_relu": nn.LeakyReLU,
     "tanh": nn.Tanh,
     "sigmoid": nn.Sigmoid,
 }
 
-SDV_SYNTHESIZERS: Final = {
-    "TVAE": TVAESynthesizer,
-    "CTGAN": CTGANSynthesizer,
-    "CopulaGAN": CopulaGANSynthesizer,
-    "Copula": GaussianCopulaSynthesizer,
-}
-
 SDV_DETECTION_METRIC_CHOICES: Final = {
     "LogisticDetection": LogisticDetection,
     "SVCDetection": SVCDetection,
 }
 
 SDV_BINARY_METRIC_CHOICES: Final = {
     "BinaryAdaBoostClassifier": BinaryAdaBoostClassifier,
```

### Comparing `nhssynth-0.3.1/src/nhssynth/common/dicts.py` & `nhssynth-0.4.0/src/nhssynth/common/dicts.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.3.1/src/nhssynth/common/io.py` & `nhssynth-0.4.0/src/nhssynth/common/io.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.3.1/src/nhssynth/common/strings.py` & `nhssynth-0.4.0/src/nhssynth/common/strings.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.3.1/src/nhssynth/modules/evaluation/full_report.py` & `nhssynth-0.4.0/src/nhssynth/modules/evaluation/full_report.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.3.1/src/nhssynth/modules/evaluation/io.py` & `nhssynth-0.4.0/src/nhssynth/modules/evaluation/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import argparse
 import pickle
 from pathlib import Path
 from typing import Any
 
 import pandas as pd
 from nhssynth.common.io import *
-from nhssynth.modules.dataloader.metadata import get_sdtypes, load_metadata
+from nhssynth.modules.dataloader.metadata import MetaData
 
 
 def check_input_paths(
     fn_dataset: str, fn_typed: str, fn_synthetic: str, fn_metadata: str, dir_experiment: Path
 ) -> tuple[str, str]:
     """
     Sets up the input and output paths for the model files.
@@ -58,10 +58,10 @@
             args.dataset, args.typed, args.synthetic, args.metadata, dir_experiment
         )
 
         with open(dir_experiment / fn_typed, "rb") as f:
             real_data = pickle.load(f)
         with open(dir_experiment / fn_synthetic, "rb") as f:
             synthetic_data = pickle.load(f)
-        sdtypes = get_sdtypes(load_metadata(dir_experiment / fn_metadata, real_data))
+        sdtypes = MetaData.load(dir_experiment / fn_metadata, real_data).get_sdtypes()
 
         return fn_dataset, real_data, synthetic_data, sdtypes
```

### Comparing `nhssynth-0.3.1/src/nhssynth/modules/evaluation/metrics.py` & `nhssynth-0.4.0/src/nhssynth/modules/evaluation/metrics.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.3.1/src/nhssynth/modules/evaluation/run.py` & `nhssynth-0.4.0/src/nhssynth/modules/evaluation/run.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.3.1/src/nhssynth/modules/model/common/DPMixin.py` & `nhssynth-0.4.0/src/nhssynth/modules/model/common/dp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import warnings
 from abc import ABC
 from typing import Optional
 
 import numpy as np
 import torch.nn as nn
-from nhssynth.modules.model.common.Model import Model
+from nhssynth.modules.model.common.model import Model
 from opacus import GradSampleModule, PrivacyEngine
 
 
 class DPMixin(ABC):
     """
     Mixin class to make a [`Model`][nhssynth.modules.model.common.DPMixin.DPMixin] differentially private
```

### Comparing `nhssynth-0.3.1/src/nhssynth/modules/model/common/Model.py` & `nhssynth-0.4.0/src/nhssynth/modules/model/common/Model.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,51 +14,51 @@
 
 class Model(nn.Module, ABC):
     """
     Abstract base class for all NHSSynth models
 
     Args:
         data: The data to train on
-        onehots: A list of lists of column indices, where each sublist containts the indices for a one-hot encoded column
-        singles: Indices of all non-onehot columns
+        multi_column_indices: A list of lists of column indices, where each sublist containts the indices for a one-hot encoded column
+        single_column_indices: Indices of all non-onehot columns
         batch_size: The batch size to use during training
         use_gpu: Flag to determine whether to use the GPU (if available)
 
     Attributes:
         nrows: The number of rows in the `data`
         ncols: The number of columns in the `data`
         columns: The names of the columns in the `data`
-        onehots: A list of lists of column indices, where each sublist containts the indices for a one-hot encoded column
-        singles: Indices of all non-onehot columns
+        multi_column_indices: A list of lists of column indices, where each sublist containts the indices for a one-hot encoded column
+        single_column_indices: Indices of all non-onehot columns
         data_loader: A PyTorch DataLoader for the `data`
         private: Whether the model is private, i.e. whether the `DPMixin` class has been inherited
         device: The device to use for training (CPU or GPU)
 
     Raises:
         TypeError: If the `Model` class is directly instantiated (i.e. not inherited)
-        AssertionError: If the number of columns in the `data` does not match the number of indices in `onehots` and `singles`
+        AssertionError: If the number of columns in the `data` does not match the number of indices in `multi_column_indices` and `single_column_indices`
         UserWarning: If `use_gpu` is True but no GPU is available
     """
 
     def __init__(
         self,
         data: pd.DataFrame,
-        onehots: Optional[list[list[int]]] = [[]],
-        singles: Optional[list[int]] = [],
+        multi_column_indices: Optional[list[list[int]]] = [[]],
+        single_column_indices: Optional[list[int]] = [],
         batch_size: int = 32,
         use_gpu: bool = False,
     ) -> None:
         if type(self) is Model:
             raise TypeError("Cannot directly instantiate the `Model` class")
         super(Model, self).__init__()
         self.nrows, self.ncols = data.shape
         self.columns: pd.Index = data.columns
-        self.onehots: list[list[int]] = onehots
-        self.singles: list[int] = singles
-        assert len(singles) + sum([len(x) for x in onehots]) == self.ncols
+        self.multi_column_indices: list[list[int]] = multi_column_indices
+        self.single_column_indices: list[int] = single_column_indices
+        assert len(single_column_indices) + sum([len(x) for x in multi_column_indices]) == self.ncols
         self.data_loader: DataLoader = DataLoader(
             # Should the data also all be turned into floats?
             TensorDataset(torch.Tensor(data.to_numpy())),
             pin_memory=True,
             batch_size=batch_size,
         )
         self.setup_device(use_gpu)
@@ -83,20 +83,20 @@
     @classmethod
     @abstractmethod
     def _get_args() -> list[str]:
         """Returns the list of arguments to look for in an `argparse.Namespace`, these must map to the arguments of the inheritor."""
         raise NotImplementedError
 
     @classmethod
-    def from_args(cls, args, data, onehots, singles):
+    def from_args(cls, args, data, multi_column_indices, single_column_indices):
         """Creates an instance from an `argparse.Namespace`."""
         return cls(
             data,
-            onehots,
-            singles,
+            multi_column_indices,
+            single_column_indices,
             **{k: getattr(args, k) for k in ["batch_size", "use_gpu"] + cls._get_args() if getattr(args, k)},
         )
 
     def _start_training(self, num_epochs: int, patience: int, tracked_metrics: list[str]) -> None:
         """Initialises the training process."""
         self.num_epochs = num_epochs
         self.patience = patience
```

### Comparing `nhssynth-0.3.1/src/nhssynth/modules/model/models/DPVAE.py` & `nhssynth-0.4.0/src/nhssynth/modules/model/models/dpvae.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Optional
 
-from nhssynth.modules.model.common.DPMixin import DPMixin
-from nhssynth.modules.model.models.VAE import VAE
+from nhssynth.modules.model.common.dp import DPMixin
+from nhssynth.modules.model.models.vae import VAE
 from opacus import GradSampleModule
 
 
 class DPVAE(DPMixin, VAE):
     """
     A differentially private VAE. Accepts [`VAE`][nhssynth.modules.model.models.VAE.VAE] arguments
     as well as [`DPMixin`][nhssynth.modules.model.common.DPMixin.DPMixin] arguments.
```

### Comparing `nhssynth-0.3.1/src/nhssynth/modules/model/models/VAE.py` & `nhssynth-0.4.0/src/nhssynth/modules/model/models/vae.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Optional
 
 import numpy as np
 import pandas as pd
 import torch
 import torch.nn as nn
 from nhssynth.common.constants import ACTIVATION_FUNCTIONS
-from nhssynth.modules.model.common.Model import Model
+from nhssynth.modules.model.common.model import Model
 from torch.distributions.normal import Normal
 from tqdm import tqdm
 
 
 class Encoder(nn.Module):
     """Encoder, takes in x and outputs mu_z, sigma_z (diagonal Gaussian variational posterior assumed)"""
 
@@ -70,18 +70,18 @@
     def forward(self, z):
         return self.net(z)
 
 
 class Noiser(nn.Module):
     def __init__(
         self,
-        num_singles: list[int],
+        num_single_column_indices: list[int],
     ) -> None:
         super().__init__()
-        self.output_logsigma_fn = nn.Linear(num_singles, num_singles, bias=True)
+        self.output_logsigma_fn = nn.Linear(num_single_column_indices, num_single_column_indices, bias=True)
         torch.nn.init.zeros_(self.output_logsigma_fn.weight)
         torch.nn.init.zeros_(self.output_logsigma_fn.bias)
         self.output_logsigma_fn.weight.requires_grad = False
 
     def forward(self, X):
         return self.output_logsigma_fn(X)
 
@@ -132,15 +132,15 @@
             decoder_latent_dim,
             decoder_hidden_dim,
             decoder_activation,
             decoder_learning_rate,
             self.shared_optimizer,
         ).to(self.device)
         self.noiser = Noiser(
-            len(self.singles),
+            len(self.single_column_indices),
         ).to(self.device)
         if self.shared_optimizer:
             assert (
                 encoder_learning_rate == decoder_learning_rate
             ), "If `shared_optimizer` is True, `encoder_learning_rate` must equal `decoder_learning_rate`"
             self.optim = torch.optim.Adam(
                 list(self.encoder.parameters()) + list(self.decoder.parameters()),
@@ -175,23 +175,23 @@
         N = N or self.nrows
         z_samples = torch.randn_like(torch.ones((N, self.encoder.latent_dim)), device=self.device)
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore", message="Using a non-full backward hook")
             x_gen = self.decoder(z_samples)
         x_gen_ = torch.ones_like(x_gen, device=self.device)
 
-        if self.onehots != [[]]:
-            for cat_idxs in self.onehots:
+        if self.multi_column_indices != [[]]:
+            for cat_idxs in self.multi_column_indices:
                 x_gen_[:, cat_idxs] = torch.distributions.one_hot_categorical.OneHotCategorical(
                     logits=x_gen[:, cat_idxs]
                 ).sample()
 
-        x_gen_[:, self.singles] = x_gen[:, self.singles] + torch.exp(
-            self.noiser(x_gen[:, self.singles])
-        ) * torch.randn_like(x_gen[:, self.singles])
+        x_gen_[:, self.single_column_indices] = x_gen[:, self.single_column_indices] + torch.exp(
+            self.noiser(x_gen[:, self.single_column_indices])
+        ) * torch.randn_like(x_gen[:, self.single_column_indices])
         if torch.cuda.is_available():
             x_gen_ = x_gen_.cpu()
         return pd.DataFrame(x_gen_.detach(), columns=self.columns)
 
     def loss(self, X):
         mu_z, logsigma_z = self.encoder(X)
 
@@ -203,29 +203,29 @@
         s = torch.randn_like(mu_z)
         z_samples = mu_z + s * torch.exp(logsigma_z)
 
         x_recon = self.decoder(z_samples)
 
         categoric_loglik = 0
 
-        if self.onehots != [[]]:
-            for cat_idxs in self.onehots:
+        if self.multi_column_indices != [[]]:
+            for cat_idxs in self.multi_column_indices:
                 categoric_loglik += -torch.nn.functional.cross_entropy(
                     x_recon[:, cat_idxs],
                     torch.max(X[:, cat_idxs], 1)[1],
                 ).sum()
 
         gauss_loglik = 0
-        if self.singles:
+        if self.single_column_indices:
             gauss_loglik = (
                 Normal(
-                    loc=x_recon[:, self.singles],
-                    scale=torch.exp(self.noiser(x_recon[:, self.singles])),
+                    loc=x_recon[:, self.single_column_indices],
+                    scale=torch.exp(self.noiser(x_recon[:, self.single_column_indices])),
                 )
-                .log_prob(X[:, self.singles])
+                .log_prob(X[:, self.single_column_indices])
                 .sum()
             )
 
         reconstruction_loss = -(categoric_loglik + gauss_loglik)
 
         elbo = kld + reconstruction_loss
```

### Comparing `nhssynth-0.3.1/src/nhssynth/modules/model/run.py` & `nhssynth-0.4.0/src/nhssynth/modules/model/run.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,22 +16,22 @@
     num_epochs_list = []
     for architecture in args.architecture:
         for i in range(args.repeats):
             print(f"\nModel architecture: {architecture}\nRepeat: {i + 1} of {args.repeats}")
 
             set_seed(args.seed + i if args.seed else None)
 
-            fn_dataset, prepared_dataset, mt = load_required_data(args, dir_experiment)
-            onehots, singles = mt.get_onehots_and_singles()
+            fn_dataset, transformed_dataset, mt = load_required_data(args, dir_experiment)
+            multi_column_indices, single_column_indices = mt.get_multi_and_single_column_indices()
 
             model = MODELS[architecture].from_args(
                 args=args,
-                data=prepared_dataset,
-                onehots=onehots,
-                singles=singles,
+                data=transformed_dataset,
+                multi_column_indices=multi_column_indices,
+                single_column_indices=single_column_indices,
             )
             num_epochs, results = model.train(
                 num_epochs=args.num_epochs,
                 patience=args.patience,
                 tracked_metrics=args.tracked_metrics,
             )
             synthetic = mt.inverse_apply(model.generate())
```

### Comparing `nhssynth-0.3.1/src/nhssynth/modules/plotting/io.py` & `nhssynth-0.4.0/src/nhssynth/modules/plotting/io.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.3.1/src/nhssynth/modules/plotting/plots.py` & `nhssynth-0.4.0/src/nhssynth/modules/plotting/plots.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.3.1/src/nhssynth/modules/plotting/run.py` & `nhssynth-0.4.0/src/nhssynth/modules/plotting/run.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.3.1/PKG-INFO` & `nhssynth-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nhssynth
-Version: 0.3.1
+Version: 0.4.0
 Summary: Synthetic data generation pipeline leveraging a Differentially Private Variational Auto Encoder assessed using a variety of metrics
 Home-page: https://github.com/nhsx/NHSSynth
 License: MIT
 Keywords: synthetic data,privacy,fairness,machine learning
 Author: HarrisonWilde
 Author-email: harrisondwilde@outlook.com
 Maintainer: NHSE TDAU
@@ -13,21 +13,21 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: gower (>=0.1.2,<0.2.0)
 Requires-Dist: opacus (>=1.4.0,<2.0.0)
-Requires-Dist: pandas (>=1.5.3,<2.0.0)
+Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
-Requires-Dist: rdt (>=1.4.0,<2.0.0)
-Requires-Dist: sdmetrics (>=0.9.3,<0.10.0)
-Requires-Dist: sdv (>=1.0.0,<2.0.0)
-Requires-Dist: setuptools (>=67.6.1,<68.0.0)
-Requires-Dist: torch (==1.13.1)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
+Requires-Dist: sdmetrics (>=0.10.1,<0.11.0)
+Requires-Dist: torch (>=2.0.1,<3.0.0)
+Requires-Dist: tornado (>=6.3.2,<7.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Project-URL: Bug Tracker, https://github.com/nhsx/NHSSynth/issues
 Project-URL: Docs, https://nhsx.github.io/NHSSynth
 Project-URL: Repository, https://github.com/nhsx/NHSSynth
 Description-Content-Type: text/markdown
 
 <!-- PROJECT SHIELDS -->
@@ -38,15 +38,15 @@
 ![Lines of Code](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/HarrisonWilde/1ab4eefed81ec381e29f7d4feb9856bc/raw/loc.json)
 ![Percentage Comments](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/HarrisonWilde/1ab4eefed81ec381e29f7d4feb9856bc/raw/comments.json)
 [![Snyk Package Health](https://snyk.io/advisor/python/nhssynth/badge.svg)](https://snyk.io/advisor/python/nhssynth)
 
 </div>
 <div align="center">
 
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nhssynth)](https://www.python.org/downloads/release/python-3100/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nhssynth)](https://www.python.org/downloads/release/python-3113/)
 [![PyPI - Package Status](https://img.shields.io/pypi/status/nhssynth)](https://pypi.org/project/nhssynth/)
 [![PyPI - Latest Release](https://img.shields.io/pypi/v/nhssynth)](https://pypi.org/project/nhssynth/)
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/nhssynth)](https://pypi.org/project/nhssynth/)
 [![PyPI - License](https://img.shields.io/pypi/l/nhssynth)](https://github.com/nhsx/nhssynth/blob/main/LICENSE)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1)](https://pycqa.github.io/isort/)
 
@@ -65,16 +65,14 @@
 
 # NHS Synth
 
 ## About
 
 This repository currently consists of a Python package alongside research and investigative materials covering the effectiveness of the package and synthetic data more generally when applied to NHS use cases. See the internal [project description](https://nhsx.github.io/nhsx-internship-projects/synthetic-data-exploration-vae/) for more information.
 
-_**Note:** No data, public or private are shared in this repository._
-
 ## Getting Started
 
 ### Project Structure
 
 - The main package and codebase is found in [`src/nhssynth`](src/nhssynth/) (see [Usage](#usage) below for more information)
 - Accompanying materials are available in the [`docs`](docs/) folder:
   - The components used to create the GitHub Pages [documentation site](https://nhsx.github.io/NHSSynth/)
@@ -96,15 +94,15 @@
 git clone git@github.com:pytorch/csprng.git
 cd csprng
 git branch release "v0.2.2-rc1"
 git checkout release
 python setup.py install
 ```
 
-#### Advanced Usage
+#### Advanced Installation
 
 If you intend on contributing or working with the codebase directly, or if you want to reproduce the results of this project, follow the steps below:
 
 1. Clone the repo
 2. Ensure one of the required versions of Python is installed
 3. Install [`poetry`](https://python-poetry.org/docs/#installation)
 4. Instantiate a virtual environment, e.g. via `python -m venv nhssynth`
@@ -138,15 +136,15 @@
 
 ### Roadmap
 
 See the [open issues](https://github.com/nhsx/NHSSynth/issues) for a list of proposed features (and known bugs). Our [milestones](https://github.com/nhsx/NHSSynth/milestones) represent longer term goals for the project.
 
 ### Contributing
 
-Any contributions you wish to make are **greatly appreciated**, we encourage you to first raise an issue to discuss with the maintainers. If you are interested in contributing, please follow these steps:
+Contributions are welcome! We encourage you to first raise an issue with your proposed contribution to enable discussion with the maintainers. After that, please follow these steps:
 
 1. Fork the project
 2. Create your branch (`git checkout -b <yourusername>/<featurename>`)
 3. Commit your changes (`git commit -m 'Add some amazing feature'`)
 4. Push to the branch (`git push origin <yourusername>/<featurename>`)
 5. Open a PR and we will try to get it merged!
```

#### html2text {}

```diff
@@ -1,37 +1,37 @@
-Metadata-Version: 2.1 Name: nhssynth Version: 0.3.1 Summary: Synthetic data
+Metadata-Version: 2.1 Name: nhssynth Version: 0.4.0 Summary: Synthetic data
 generation pipeline leveraging a Differentially Private Variational Auto
 Encoder assessed using a variety of metrics Home-page: https://github.com/nhsx/
 NHSSynth License: MIT Keywords: synthetic data,privacy,fairness,machine
 learning Author: HarrisonWilde Author-email: harrisondwilde@outlook.com
 Maintainer: NHSE TDAU Maintainer-email: england.tdau@nhs.net Requires-Python:
 >=3.9,<3.11 Classifier: Development Status :: 3 - Alpha Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Requires-Dist: gower (>=0.1.2,<0.2.0) Requires-Dist:
-opacus (>=1.4.0,<2.0.0) Requires-Dist: pandas (>=1.5.3,<2.0.0) Requires-Dist:
-pyyaml (>=6.0,<7.0) Requires-Dist: rdt (>=1.4.0,<2.0.0) Requires-Dist:
-sdmetrics (>=0.9.3,<0.10.0) Requires-Dist: sdv (>=1.0.0,<2.0.0) Requires-Dist:
-setuptools (>=67.6.1,<68.0.0) Requires-Dist: torch (==1.13.1) Requires-Dist:
-tqdm (>=4.65.0,<5.0.0) Project-URL: Bug Tracker, https://github.com/nhsx/
-NHSSynth/issues Project-URL: Docs, https://nhsx.github.io/NHSSynth Project-URL:
-Repository, https://github.com/nhsx/NHSSynth Description-Content-Type: text/
-markdown
+opacus (>=1.4.0,<2.0.0) Requires-Dist: pandas (>=2.0.1,<3.0.0) Requires-Dist:
+pyyaml (>=6.0,<7.0) Requires-Dist: requests (>=2.31.0,<3.0.0) Requires-Dist:
+scikit-learn (>=1.2.2,<2.0.0) Requires-Dist: sdmetrics (>=0.10.1,<0.11.0)
+Requires-Dist: torch (>=2.0.1,<3.0.0) Requires-Dist: tornado (>=6.3.2,<7.0.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0) Project-URL: Bug Tracker, https://
+github.com/nhsx/NHSSynth/issues Project-URL: Docs, https://nhsx.github.io/
+NHSSynth Project-URL: Repository, https://github.com/nhsx/NHSSynth Description-
+Content-Type: text/markdown
            ![Coverage](https://img.shields.io/endpoint?url=https://
 gist.githubusercontent.com/HarrisonWilde/1ab4eefed81ec381e29f7d4feb9856bc/raw/
  coverage.json) ![Tests Passing](https://img.shields.io/endpoint?url=https://
 gist.githubusercontent.com/HarrisonWilde/1ab4eefed81ec381e29f7d4feb9856bc/raw/
    tests.json) ![Lines of Code](https://img.shields.io/endpoint?url=https://
 gist.githubusercontent.com/HarrisonWilde/1ab4eefed81ec381e29f7d4feb9856bc/raw/
  loc.json) ![Percentage Comments](https://img.shields.io/endpoint?url=https://
 gist.githubusercontent.com/HarrisonWilde/1ab4eefed81ec381e29f7d4feb9856bc/raw/
 comments.json) [![Snyk Package Health](https://snyk.io/advisor/python/nhssynth/
              badge.svg)](https://snyk.io/advisor/python/nhssynth)
   [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nhssynth)]
-   (https://www.python.org/downloads/release/python-3100/) [![PyPI - Package
+   (https://www.python.org/downloads/release/python-3113/) [![PyPI - Package
 Status](https://img.shields.io/pypi/status/nhssynth)](https://pypi.org/project/
  nhssynth/) [![PyPI - Latest Release](https://img.shields.io/pypi/v/nhssynth)]
  (https://pypi.org/project/nhssynth/) [![PyPI - Wheel](https://img.shields.io/
  pypi/wheel/nhssynth)](https://pypi.org/project/nhssynth/) [![PyPI - License]
   (https://img.shields.io/pypi/l/nhssynth)](https://github.com/nhsx/nhssynth/
     blob/main/LICENSE) [![Code style: black](https://img.shields.io/badge/
  code%20style-black-000000)](https://github.com/psf/black) [![Imports: isort]
@@ -40,84 +40,83 @@
                                     [Logo]
                              Explore_the_docs_Â»
 
 # NHS Synth ## About This repository currently consists of a Python package
 alongside research and investigative materials covering the effectiveness of
 the package and synthetic data more generally when applied to NHS use cases.
 See the internal [project description](https://nhsx.github.io/nhsx-internship-
-projects/synthetic-data-exploration-vae/) for more information. _**Note:** No
-data, public or private are shared in this repository._ ## Getting Started ###
-Project Structure - The main package and codebase is found in [`src/nhssynth`]
-(src/nhssynth/) (see [Usage](#usage) below for more information) - Accompanying
-materials are available in the [`docs`](docs/) folder: - The components used to
-create the GitHub Pages [documentation site](https://nhsx.github.io/NHSSynth/
-) - A [report](docs/reports/report.pdf) summarising the previous iteration of
-this project - A [model card](docs/model_card.md) providing more information
-about the VAE with Differential Privacy - Numerous exemplar configurations are
-found in [`config`](config/) - Empty [`data`](data/) and [`experiments`]
-(experiments/) folders are provided; these are the default locations for inputs
-and outputs when running the project using the provided [CLI](../src/nhssynth/
-cli/) module - Pre-processing notebooks for specific datasets used to assess
-the approach and other non-core code can be found in [`auxiliary`](../
-auxiliary/) ### Installation For general usage, we recommend installing the
-package via `pip install nhssynth` in a supported python version environment.
-You can then `import` the package's [modules](src/nhssynth/modules/) and use
-them in your projects, or interact with the package directly via the [CLI](src/
-nhssynth/cli/), which is accessed using the `nhssynth` command (see [Usage]
-(#usage) for more information). #### Secure Mode Note that in order to train a
-generator in *secure mode* (see the [documentation](https://nhsx.github.io/
-NHSSynth/secure_mode/) for details) you will need to install the PyTorch
-extension package [`csprng`](https://github.com/pytorch/csprng) separately.
-Currently this package's dependencies are not compatible with recent versions
-of PyTorch (the author's plan on rectifying this - watch this space), so you
-will need to install it manually; for this we recommend following the
-instructions below: ```bash git clone git@github.com:pytorch/csprng.git cd
-csprng git branch release "v0.2.2-rc1" git checkout release python setup.py
-install ``` #### Advanced Usage If you intend on contributing or working with
-the codebase directly, or if you want to reproduce the results of this project,
-follow the steps below: 1. Clone the repo 2. Ensure one of the required
-versions of Python is installed 3. Install [`poetry`](https://python-
-poetry.org/docs/#installation) 4. Instantiate a virtual environment, e.g. via
-`python -m venv nhssynth` 3. Activate the virtual environment, e.g. via `source
-nhssynth/bin/activate` 4. Install the project dependencies with `poetry
-install` (optionally install the dev dependencies `--with dev` to work with the
-[auxiliary notebooks](auxiliary/), or `--with docs` to work with the
-[documentation](docs/)) 5. You can then interact with the package in one of two
-ways: - Via the [CLI](src/nhssynth/cli/) module using `nhssynth ...` - Through
-building the package with `poetry build` and using it in an existing project
-(`import nhssynth`). You can then actively develop the package and test it. ###
-Usage This package comprises a set of modules that can be run individually, as
-part of a pipeline, or via a configuration file. These options are available
-via the `nhssynth` command: ``` nhssynth  -- nhssynth pipeline -- nhssynth
-config -c  -- ``` To see the modules that are available and their corresponding
-arguments, run `nhssynth --help` and `nhssynth  --help` respectively.
-Configuration files can be used to run the pipeline or a chosen set of modules.
-They should be placed in the [`config`](config/) folder and their layout should
-match that of the examples provided. They can be run as in the latter case
-above by providing their filename (without the `.yaml` extension). You can also
-override any of the arguments provided in the configuration file by passing
-them as arguments in the command line. To ensure reproducibility, you should
-always specify a `--seed` value and provide the `--save-config` flag to dump
-the exact configuration specified / inferred for the run. This configuration
-file can then be used in the future to reproduce the exact same run or shared
-with others to run the same configuration on their dataset, etc. The figure
-below shows the structure and workflow of the package and its modules. ![]
-(docs/modules.png) View a visualisation of the codebase [here](https://mango-
-dune-07a8b7110.1.azurestaticapps.net/?repo=nhsx%2Fnhssynth)! ### Roadmap See
-the [open issues](https://github.com/nhsx/NHSSynth/issues) for a list of
-proposed features (and known bugs). Our [milestones](https://github.com/nhsx/
-NHSSynth/milestones) represent longer term goals for the project. ###
-Contributing Any contributions you wish to make are **greatly appreciated**, we
-encourage you to first raise an issue to discuss with the maintainers. If you
-are interested in contributing, please follow these steps: 1. Fork the project
-2. Create your branch (`git checkout -b /`) 3. Commit your changes (`git commit
--m 'Add some amazing feature'`) 4. Push to the branch (`git push origin /`) 5.
-Open a PR and we will try to get it merged! _See [CONTRIBUTING.md](./
-CONTRIBUTING.md) for detailed guidance._ Thanks to everyone that has
-contributed so far!
+projects/synthetic-data-exploration-vae/) for more information. ## Getting
+Started ### Project Structure - The main package and codebase is found in
+[`src/nhssynth`](src/nhssynth/) (see [Usage](#usage) below for more
+information) - Accompanying materials are available in the [`docs`](docs/
+) folder: - The components used to create the GitHub Pages [documentation site]
+(https://nhsx.github.io/NHSSynth/) - A [report](docs/reports/report.pdf)
+summarising the previous iteration of this project - A [model card](docs/
+model_card.md) providing more information about the VAE with Differential
+Privacy - Numerous exemplar configurations are found in [`config`](config/) -
+Empty [`data`](data/) and [`experiments`](experiments/) folders are provided;
+these are the default locations for inputs and outputs when running the project
+using the provided [CLI](../src/nhssynth/cli/) module - Pre-processing
+notebooks for specific datasets used to assess the approach and other non-core
+code can be found in [`auxiliary`](../auxiliary/) ### Installation For general
+usage, we recommend installing the package via `pip install nhssynth` in a
+supported python version environment. You can then `import` the package's
+[modules](src/nhssynth/modules/) and use them in your projects, or interact
+with the package directly via the [CLI](src/nhssynth/cli/), which is accessed
+using the `nhssynth` command (see [Usage](#usage) for more information). ####
+Secure Mode Note that in order to train a generator in *secure mode* (see the
+[documentation](https://nhsx.github.io/NHSSynth/secure_mode/) for details) you
+will need to install the PyTorch extension package [`csprng`](https://
+github.com/pytorch/csprng) separately. Currently this package's dependencies
+are not compatible with recent versions of PyTorch (the author's plan on
+rectifying this - watch this space), so you will need to install it manually;
+for this we recommend following the instructions below: ```bash git clone
+git@github.com:pytorch/csprng.git cd csprng git branch release "v0.2.2-rc1" git
+checkout release python setup.py install ``` #### Advanced Installation If you
+intend on contributing or working with the codebase directly, or if you want to
+reproduce the results of this project, follow the steps below: 1. Clone the
+repo 2. Ensure one of the required versions of Python is installed 3. Install
+[`poetry`](https://python-poetry.org/docs/#installation) 4. Instantiate a
+virtual environment, e.g. via `python -m venv nhssynth` 3. Activate the virtual
+environment, e.g. via `source nhssynth/bin/activate` 4. Install the project
+dependencies with `poetry install` (optionally install the dev dependencies `--
+with dev` to work with the [auxiliary notebooks](auxiliary/), or `--with docs`
+to work with the [documentation](docs/)) 5. You can then interact with the
+package in one of two ways: - Via the [CLI](src/nhssynth/cli/) module using
+`nhssynth ...` - Through building the package with `poetry build` and using it
+in an existing project (`import nhssynth`). You can then actively develop the
+package and test it. ### Usage This package comprises a set of modules that can
+be run individually, as part of a pipeline, or via a configuration file. These
+options are available via the `nhssynth` command: ``` nhssynth  -- nhssynth
+pipeline -- nhssynth config -c  -- ``` To see the modules that are available
+and their corresponding arguments, run `nhssynth --help` and `nhssynth  --help`
+respectively. Configuration files can be used to run the pipeline or a chosen
+set of modules. They should be placed in the [`config`](config/) folder and
+their layout should match that of the examples provided. They can be run as in
+the latter case above by providing their filename (without the `.yaml`
+extension). You can also override any of the arguments provided in the
+configuration file by passing them as arguments in the command line. To ensure
+reproducibility, you should always specify a `--seed` value and provide the `--
+save-config` flag to dump the exact configuration specified / inferred for the
+run. This configuration file can then be used in the future to reproduce the
+exact same run or shared with others to run the same configuration on their
+dataset, etc. The figure below shows the structure and workflow of the package
+and its modules. ![](docs/modules.png) View a visualisation of the codebase
+[here](https://mango-dune-07a8b7110.1.azurestaticapps.net/
+?repo=nhsx%2Fnhssynth)! ### Roadmap See the [open issues](https://github.com/
+nhsx/NHSSynth/issues) for a list of proposed features (and known bugs). Our
+[milestones](https://github.com/nhsx/NHSSynth/milestones) represent longer term
+goals for the project. ### Contributing Contributions are welcome! We encourage
+you to first raise an issue with your proposed contribution to enable
+discussion with the maintainers. After that, please follow these steps: 1. Fork
+the project 2. Create your branch (`git checkout -b /`) 3. Commit your changes
+(`git commit -m 'Add some amazing feature'`) 4. Push to the branch (`git push
+origin /`) 5. Open a PR and we will try to get it merged! _See
+[CONTRIBUTING.md](./CONTRIBUTING.md) for detailed guidance._ Thanks to everyone
+that has contributed so far!
                [https://contrib.rocks/image?repo=nhsx/nhssynth]
 This codebase builds on previous NHSX Analytics Unit PhD internships
 contextualising and investigating the potential use of Variational Auto
 Encoders (VAEs) for synthetic data generation. These were undertaken by Dominic
 Danks and David Brind. ### License Distributed under the MIT License. _See
 [LICENSE](./LICENSE) for more information._ ### Contact This project is under
 active development by [@HarrisonWilde](https://github.com/HarrisonWilde). For
```

