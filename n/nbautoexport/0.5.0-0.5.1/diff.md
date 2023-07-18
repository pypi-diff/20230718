# Comparing `tmp/nbautoexport-0.5.0.tar.gz` & `tmp/nbautoexport-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbautoexport-0.5.0.tar", last modified: Wed Mar 16 20:22:24 2022, max compression
+gzip compressed data, was "nbautoexport-0.5.1.tar", last modified: Tue Jul 18 18:17:44 2023, max compression
```

## Comparing `nbautoexport-0.5.0.tar` & `nbautoexport-0.5.1.tar`

### file list

```diff
@@ -1,47 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:22:24.082962 nbautoexport-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)     6356 2022-03-16 20:21:47.000000 nbautoexport-0.5.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     3061 2022-03-16 20:21:47.000000 nbautoexport-0.5.0/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (121)     1055 2022-03-16 20:21:47.000000 nbautoexport-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-03-16 20:21:47.000000 nbautoexport-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    13024 2022-03-16 20:22:24.082962 nbautoexport-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7080 2022-03-16 20:21:47.000000 nbautoexport-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:22:24.082962 nbautoexport-0.5.0/nbautoexport/
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-03-16 20:21:47.000000 nbautoexport-0.5.0/nbautoexport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-03-16 20:21:47.000000 nbautoexport-0.5.0/nbautoexport/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-03-16 20:22:24.082962 nbautoexport-0.5.0/nbautoexport/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     4602 2022-03-16 20:21:47.000000 nbautoexport-0.5.0/nbautoexport/clean.py
--rw-r--r--   0 runner    (1001) docker     (121)     5219 2022-03-16 20:21:47.000000 nbautoexport-0.5.0/nbautoexport/export.py
--rw-r--r--   0 runner    (1001) docker     (121)     4811 2022-03-16 20:21:47.000000 nbautoexport-0.5.0/nbautoexport/jupyter_config.py
--rw-r--r--   0 runner    (1001) docker     (121)    13661 2022-03-16 20:21:47.000000 nbautoexport-0.5.0/nbautoexport/nbautoexport.py
--rw-r--r--   0 runner    (1001) docker     (121)     1785 2022-03-16 20:21:47.000000 nbautoexport-0.5.0/nbautoexport/sentinel.py
--rw-r--r--   0 runner    (1001) docker     (121)     3145 2022-03-16 20:21:47.000000 nbautoexport-0.5.0/nbautoexport/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:22:24.078962 nbautoexport-0.5.0/nbautoexport.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    13024 2022-03-16 20:22:23.000000 nbautoexport-0.5.0/nbautoexport.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      942 2022-03-16 20:22:23.000000 nbautoexport-0.5.0/nbautoexport.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-16 20:22:23.000000 nbautoexport-0.5.0/nbautoexport.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-03-16 20:22:23.000000 nbautoexport-0.5.0/nbautoexport.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-16 20:22:23.000000 nbautoexport-0.5.0/nbautoexport.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-03-16 20:22:23.000000 nbautoexport-0.5.0/nbautoexport.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-03-16 20:22:23.000000 nbautoexport-0.5.0/nbautoexport.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-03-16 20:21:47.000000 nbautoexport-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-03-16 20:21:47.000000 nbautoexport-0.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      636 2022-03-16 20:22:24.082962 nbautoexport-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2296 2022-03-16 20:21:47.000000 nbautoexport-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:22:24.082962 nbautoexport-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-03-16 20:21:47.000000 nbautoexport-0.5.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 20:22:24.082962 nbautoexport-0.5.0/tests/assets/
--rw-r--r--   0 runner    (1001) docker     (121)    18553 2022-03-16 20:21:47.000000 nbautoexport-0.5.0/tests/assets/the_notebook.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)      534 2022-03-16 20:21:47.000000 nbautoexport-0.5.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1404 2022-03-16 20:21:47.000000 nbautoexport-0.5.0/tests/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (121)     2895 2022-03-16 20:21:47.000000 nbautoexport-0.5.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     9734 2022-03-16 20:21:47.000000 nbautoexport-0.5.0/tests/test_cli_clean.py
--rw-r--r--   0 runner    (1001) docker     (121)     5169 2022-03-16 20:21:47.000000 nbautoexport-0.5.0/tests/test_cli_configure.py
--rw-r--r--   0 runner    (1001) docker     (121)     9691 2022-03-16 20:21:47.000000 nbautoexport-0.5.0/tests/test_cli_export.py
--rw-r--r--   0 runner    (1001) docker     (121)     2191 2022-03-16 20:21:47.000000 nbautoexport-0.5.0/tests/test_cli_install.py
--rw-r--r--   0 runner    (1001) docker     (121)     5633 2022-03-16 20:21:47.000000 nbautoexport-0.5.0/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (121)    11730 2022-03-16 20:21:47.000000 nbautoexport-0.5.0/tests/test_jupyter_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     4809 2022-03-16 20:21:47.000000 nbautoexport-0.5.0/tests/test_post_save.py
--rw-r--r--   0 runner    (1001) docker     (121)      836 2022-03-16 20:21:47.000000 nbautoexport-0.5.0/tests/test_sentinel.py
--rw-r--r--   0 runner    (1001) docker     (121)     4299 2022-03-16 20:21:47.000000 nbautoexport-0.5.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      628 2022-03-16 20:21:47.000000 nbautoexport-0.5.0/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    68611 2022-03-16 20:21:47.000000 nbautoexport-0.5.0/versioneer.py
+-rw-r--r--   0        0        0     1055 2023-07-18 18:17:02.665674 nbautoexport-0.5.1/LICENSE
+-rw-r--r--   0        0        0     7080 2023-07-18 18:17:02.665674 nbautoexport-0.5.1/README.md
+-rw-r--r--   0        0        0      159 2023-07-18 18:17:02.665674 nbautoexport-0.5.1/nbautoexport/__init__.py
+-rw-r--r--   0        0        0       83 2023-07-18 18:17:02.665674 nbautoexport-0.5.1/nbautoexport/__main__.py
+-rw-r--r--   0        0        0     4602 2023-07-18 18:17:02.665674 nbautoexport-0.5.1/nbautoexport/clean.py
+-rw-r--r--   0        0        0     5219 2023-07-18 18:17:02.665674 nbautoexport-0.5.1/nbautoexport/export.py
+-rw-r--r--   0        0        0     4837 2023-07-18 18:17:02.665674 nbautoexport-0.5.1/nbautoexport/jupyter_config.py
+-rw-r--r--   0        0        0    13661 2023-07-18 18:17:02.665674 nbautoexport-0.5.1/nbautoexport/nbautoexport.py
+-rw-r--r--   0        0        0     2249 2023-07-18 18:17:02.665674 nbautoexport-0.5.1/nbautoexport/sentinel.py
+-rw-r--r--   0        0        0     3583 2023-07-18 18:17:02.665674 nbautoexport-0.5.1/nbautoexport/utils.py
+-rw-r--r--   0        0        0     2097 2023-07-18 18:17:02.665674 nbautoexport-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0       42 2023-07-18 18:17:02.665674 nbautoexport-0.5.1/tests/__init__.py
+-rw-r--r--   0        0        0    18553 2023-07-18 18:17:02.669674 nbautoexport-0.5.1/tests/assets/the_notebook.ipynb
+-rw-r--r--   0        0        0      731 2023-07-18 18:17:02.669674 nbautoexport-0.5.1/tests/conftest.py
+-rw-r--r--   0        0        0     1404 2023-07-18 18:17:02.669674 nbautoexport-0.5.1/tests/test_clean.py
+-rw-r--r--   0        0        0     2953 2023-07-18 18:17:02.669674 nbautoexport-0.5.1/tests/test_cli.py
+-rw-r--r--   0        0        0     9795 2023-07-18 18:17:02.669674 nbautoexport-0.5.1/tests/test_cli_clean.py
+-rw-r--r--   0        0        0     5248 2023-07-18 18:17:02.669674 nbautoexport-0.5.1/tests/test_cli_configure.py
+-rw-r--r--   0        0        0     9757 2023-07-18 18:17:02.669674 nbautoexport-0.5.1/tests/test_cli_export.py
+-rw-r--r--   0        0        0     2191 2023-07-18 18:17:02.669674 nbautoexport-0.5.1/tests/test_cli_install.py
+-rw-r--r--   0        0        0     5633 2023-07-18 18:17:02.669674 nbautoexport-0.5.1/tests/test_export.py
+-rw-r--r--   0        0        0    11730 2023-07-18 18:17:02.669674 nbautoexport-0.5.1/tests/test_jupyter_config.py
+-rw-r--r--   0        0        0     4809 2023-07-18 18:17:02.669674 nbautoexport-0.5.1/tests/test_post_save.py
+-rw-r--r--   0        0        0      836 2023-07-18 18:17:02.669674 nbautoexport-0.5.1/tests/test_sentinel.py
+-rw-r--r--   0        0        0     4299 2023-07-18 18:17:02.669674 nbautoexport-0.5.1/tests/test_utils.py
+-rw-r--r--   0        0        0      628 2023-07-18 18:17:02.669674 nbautoexport-0.5.1/tests/utils.py
+-rw-r--r--   0        0        0     8293 1970-01-01 00:00:00.000000 nbautoexport-0.5.1/PKG-INFO
```

### Comparing `nbautoexport-0.5.0/LICENSE` & `nbautoexport-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nbautoexport-0.5.0/PKG-INFO` & `nbautoexport-0.5.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,247 +1,201 @@
 Metadata-Version: 2.1
 Name: nbautoexport
-Version: 0.5.0
+Version: 0.5.1
 Summary: Automatically export Jupyter notebooks to various file formats (.py, .html, and more) on save.
-Home-page: https://github.com/drivendataorg/nbautoexport
-Author: DrivenData
-Author-email: info@drivendata.org
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/drivendataorg/nbautoexport/issues
-Project-URL: Documentation, https://nbautoexport.drivendata.org/
-Project-URL: Source Code, https://github.com/drivendataorg/nbautoexport
-Description: # nbautoexport
-        
-        [![Docs Status](https://img.shields.io/badge/docs-stable-informational)](https://nbautoexport.drivendata.org/)
-        [![PyPI](https://img.shields.io/pypi/v/nbautoexport.svg)](https://pypi.org/project/nbautoexport/)
-        [![conda-forge](https://img.shields.io/conda/vn/conda-forge/nbautoexport.svg)](https://anaconda.org/conda-forge/nbautoexport)
-        [![tests](https://github.com/drivendataorg/nbautoexport/workflows/tests/badge.svg?branch=master)](https://github.com/drivendataorg/nbautoexport/actions?query=workflow%3Atests+branch%3Amaster)
-        [![codecov](https://codecov.io/gh/drivendataorg/nbautoexport/branch/master/graph/badge.svg)](https://codecov.io/gh/drivendataorg/nbautoexport)
-        
-        > Making it easier to code review Jupyter notebooks, one script at a time.
-        
-        `nbautoexport` automatically exports Jupyter notebooks to various file formats (.py, .html, and more) upon save while using Jupyter. One great use case is to automatically have script versions of your notebooks to [facilitate code review commenting](https://www.drivendata.co/blog/nbautoexport-jupyter-code-review/).
-        
-        ## Installation
-        
-        First, you will need to install `nbautoexport`. This should be installed in the same environment you are running Jupyter Notebook or Jupyter Lab from. `nbautoexport` is available either from [PyPI](https://pypi.org/project/nbautoexport/) via `pip` or from [conda-forge](https://github.com/conda-forge/nbautoexport-feedstock) via `conda`.
-        
-        ```bash
-        pip install nbautoexport
-        ```
-        
-        ```bash
-        conda install nbautoexport --channel conda-forge
-        ```
-        
-        Then, to register `nbautoexport` to run automatically while using Jupyter Notebook or Jupyter Lab, run:
-        
-        ```bash
-        nbautoexport install
-        ```
-        
-        If you already have a Jupyter server running, you will need to restart it for this to take effect.
-        
-        ## Simple usage
-        
-        Let's say you have a project and keep your notebooks in a `notebooks/` subdirectory.
-        
-        To configure that directory for automatic exporting, run the following command:
-        
-        ```bash
-        nbautoexport configure notebooks
-        ```
-        
-        This will create a configuration file `notebooks/.nbautoexport`.
-        
-        If you've set up `nbautoexport` to work with Jupyter (using the `install` command as detailed in the previous section), then any time you save a notebook in Jupyter, a hook will run that checks whether there is a `.nbautoexport` configuration file in the same directory as the notebook. If so, it will use the settings specified in that file to export your notebook. By default, it will generate a script version of your notebook named after the notebook (with the `.py` extension) and saved in the directory `notebooks/script`.
-        
-        If everything is working, your notebooks directory should end up with files like the below example:
-        
-        ```text
-        notebooks
-        ├──0.1-ejm-data-exploration.ipynb
-        ├──0.2-ejm-feature-creation.ipynb
-        └── script
-            └── 0.1-ejm-data-exploration.py
-            └── 0.2-ejm-feature-creation.py
-        ```
-        
-        ## Configuring export options
-        
-        The default `.nbautoexport` configuration file looks like this:
-        
-        ```json
-        {
-          "export_formats": [
-            "script"
-          ],
-          "organize_by": "extension"
-        }
-        ```
-        
-        Upon save, this will lead to notebooks being exported to scripts which saved to the `notebooks/script` directory.
-        
-        ```text
-        notebooks
-        ├──0.1-ejm-data-exploration.ipynb
-        ├──0.2-ejm-feature-creation.ipynb
-        └── script
-            └── 0.1-ejm-data-exploration.py
-            └── 0.2-ejm-feature-creation.py
-        ```
-        
-        An alternative way to organize exported files is to create a directory for each notebook. This can be handy for matching both the notebook and subdirectory when tab-completing and then globbing with `*` after the part that completed.
-        
-        ```bash
-        nbautoexport configure notebooks --organize-by notebook
-        ```
-        
-        ```text
-        notebooks
-        ├── 0.1-ejm-data-exploration
-        │   └── 0.1-ejm-data-exploration.py
-        ├── 0.2-ejm-feature-creation
-        │   └── 0.2-ejm-feature-creation.py
-        ├──0.1-ejm-data-exploration.ipynb
-        └──0.2-ejm-feature-creation.ipynb
-        ```
-        
-        If you do not like the settings you selected, you can always change them by either 1) re-running the `nbautoexport` command with new arguments and the `--overwrite` flag, or 2) manually editing the `.nbautoexport` file.
-        
-        You can also specify as many export formats as you'd like. We support most of the export formats available from [`nbconvert`](https://nbconvert.readthedocs.io/en/latest/), such as `html`, `md`, and `pdf`. To specify formats, use the `--export-format` for each format you want to include.
-        
-        
-        ### Advanced example
-        
-        ```bash
-        nbautoexport configure sprint_one_notebooks -f script -f html --organize-by extension
-        ```
-        
-        Upon save, this creates `.py` and `.html` versions of the Jupyter notebooks in `sprint_one_notebooks` folder and results in the following organization:
-        
-        ```text
-        notebooks
-        ├──0.1-ejm-data-exploration.ipynb
-        ├──0.2-ejm-feature-creation.ipynb
-        ├── script
-        │   └── 0.1-ejm-data-exploration.py
-        │   └── 0.1-ejm-features-creation.py
-        └── html
-            └── 0.1-ejm-data-exploration.html
-            └── 0.1-ejm-features-creation.html
-        ```
-        
-        ## More functionality
-        
-        The `nbautoexport` CLI has two additional commands:
-        
-        - `export` is for ad hoc exporting of a notebook or directory of notebooks
-        - `clean` (EXPERIMENTAL) will delete files in a directory that are not generated by the current `.nbautoexport` configuration
-        
-        Use the `--help` flag to see the documentation.
-        
-        ## Command-line help
-        
-        ```bash
-        nbautoexport --help
-        ```
-        
-        ```text
-        Usage: nbautoexport [OPTIONS] COMMAND [ARGS]...
-        
-          Automatically export Jupyter notebooks to various file formats (.py,
-          .html, and more) upon save. One great use case is to automatically have
-          script versions of your notebooks to facilitate code review commenting.
-        
-          To set up, first use the 'install' command to register nbautoexport with
-          Jupyter. If you already have a Jupyter server running, you will need to
-          restart it.
-        
-          Next, you will need to use the 'configure' command to create a
-          .nbautoexport configuration file in the same directory as the notebooks
-          you want to have export automatically.
-        
-          Once nbautoexport is installed with the first step, exporting will run
-          automatically when saving a notebook in Jupyter for any notebook where
-          there is a .nbautoexport configuration file in the same directory.
-        
-        Options:
-          --version             Show nbautoexport version.
-          --install-completion  Install completion for the current shell.
-          --show-completion     Show completion for the current shell, to copy it or
-                                customize the installation.
-        
-          --help                Show this message and exit.
-        
-        Commands:
-          clean      (EXPERIMENTAL) Remove subfolders/files not matching...
-          configure  Create a .nbautoexport configuration file in a directory.
-          export     Manually export notebook or directory of notebooks.
-          install    Register nbautoexport post-save hook with Jupyter.
-        ```
-        
-        ---
-        
-        This repository was initially created using [Cookiecutter](https://github.com/audreyr/cookiecutter) with [`audreyr/cookiecutter-pypackage`](https://github.com/audreyr/cookiecutter-pypackage).
-        
-        
-        # History
-        
-        ## 0.5.0 (2022-02-16)
-        
-        - Removes support for Python 3.6.
-        - Removes explicit dependency on `pywinpty` for Windows environments.
-        
-        ## 0.4.1 (2022-02-15)
-        
-        This will be the last version of `nbautoexport` that will have been tested on and officially support Python 3.6.
-        
-        - Adds dependency on `pywinpty` for Windows environments with a version ceiling on the last version that works with Python 3.6. ([Issue #90](https://github.com/drivendataorg/nbautoexport/issues/90), [PR #92](https://github.com/drivendataorg/nbautoexport/issues/92))
-        
-        ## 0.4.0 (2021-10-29)
-        
-        - Logging improvements. ([Issue #74](https://github.com/drivendataorg/nbautoexport/issues/74), [PR #80](https://github.com/drivendataorg/nbautoexport/pull/80))
-          - Adds additional log statements during post-save hook initialization and execution to facilitate debugging.
-          - Changes runtime errors in post-save hook to be caught gracefully instead of interrupting user with an alert dialog in the Jupyter UI.
-          - Adds logging integration with active Jupyter applications. Logs will use Jupyter formatting.
-          - Changes `--verbose`/`-v` flag to work as a counter. `-v` will set log level to INFO, and `-vv` will set log level to `DEBUG`.
-        
-        ## 0.3.1 (2021-03-10)
-        
-        - Remove extraneous dependency on `jupyter_contrib_nbextensions`. Add `traitlets`, `notebook`, `jupyter_core`, and `nbformat` as explicit dependencies; previously they were treated as transitive dependencies even though they are actually direct dependencies. ([Issue #68](https://github.com/drivendataorg/nbautoexport/issues/68))
-        
-        ## 0.3.0 (2021-02-18)
-        
-        - Explicitly set all input and output file encodings to UTF-8, which fixes a bug with HTML exports on Windows with `nbconvert` v6.0. This version removes the version ceiling on <6.
-          - This is not expected to cause any backwards compatibility issues. However, in the _very_ unlikely instance that your `jupyter_notebook_config.py` file or your `nbautoexport.json` config file is Windows-1252-encoded _and_ contains non-ASCII characters, you will need to convert them to UTF-8. ([Issue #57](https://github.com/drivendataorg/nbautoexport/issues/57), [PR #61](https://github.com/drivendataorg/nbautoexport/pull/61))
-        
-        ## 0.2.1 (2020-09-18)
-        
-        - `nbconvert` released version 6, which may break HTML exports on Windows. Pinning to `nbconvert<6` until we can address [Issue #57](https://github.com/drivendataorg/nbautoexport/issues/57).
-        
-        ## 0.2.0 (2020-09-04)
-        
-        - Add option to specify glob-style patterns to exclude files from deletion when using `clean`. See [documentation](https://nbautoexport.drivendata.org/stable/cleaning/#excluding-files) for more details. ([Issue #46](https://github.com/drivendataorg/nbautoexport/issues/46), [PR #54](https://github.com/drivendataorg/nbautoexport/pull/54))
-        
-        ## 0.1.1 (2020-08-06)
-        
-        - Fixes missing `requirements.txt` bug when installing from source distribution. ([Issue #50](https://github.com/drivendataorg/nbautoexport/issues/50), [PR #52](https://github.com/drivendataorg/nbautoexport/pull/52))
-        
-        ## 0.1.0 (2020-08-05)
-        
-        - First release on PyPI.
-        
+License: MIT
 Keywords: nbautoexport,jupyter,nbconvert
-Platform: UNKNOWN
+Author-email: DrivenData <info@drivendata.org>
+Requires-Python: >=3.7
 Classifier: Framework :: Jupyter
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Project-URL: Bug Tracker, https://github.com/drivendataorg/nbautoexport/issues
+Project-URL: Changelog, https://nbautoexport.drivendata.org/stable/changelog/
+Project-URL: Documentation, https://nbautoexport.drivendata.org/
+Project-URL: Homepage, https://github.com/drivendataorg/nbautoexport
+Project-URL: Repository, https://github.com/drivendataorg/nbautoexport
 Description-Content-Type: text/markdown
+
+# nbautoexport
+
+[![Docs Status](https://img.shields.io/badge/docs-stable-informational)](https://nbautoexport.drivendata.org/)
+[![PyPI](https://img.shields.io/pypi/v/nbautoexport.svg)](https://pypi.org/project/nbautoexport/)
+[![conda-forge](https://img.shields.io/conda/vn/conda-forge/nbautoexport.svg)](https://anaconda.org/conda-forge/nbautoexport)
+[![tests](https://github.com/drivendataorg/nbautoexport/workflows/tests/badge.svg?branch=master)](https://github.com/drivendataorg/nbautoexport/actions?query=workflow%3Atests+branch%3Amaster)
+[![codecov](https://codecov.io/gh/drivendataorg/nbautoexport/branch/master/graph/badge.svg)](https://codecov.io/gh/drivendataorg/nbautoexport)
+
+> Making it easier to code review Jupyter notebooks, one script at a time.
+
+`nbautoexport` automatically exports Jupyter notebooks to various file formats (.py, .html, and more) upon save while using Jupyter. One great use case is to automatically have script versions of your notebooks to [facilitate code review commenting](https://www.drivendata.co/blog/nbautoexport-jupyter-code-review/).
+
+## Installation
+
+First, you will need to install `nbautoexport`. This should be installed in the same environment you are running Jupyter Notebook or Jupyter Lab from. `nbautoexport` is available either from [PyPI](https://pypi.org/project/nbautoexport/) via `pip` or from [conda-forge](https://github.com/conda-forge/nbautoexport-feedstock) via `conda`.
+
+```bash
+pip install nbautoexport
+```
+
+```bash
+conda install nbautoexport --channel conda-forge
+```
+
+Then, to register `nbautoexport` to run automatically while using Jupyter Notebook or Jupyter Lab, run:
+
+```bash
+nbautoexport install
+```
+
+If you already have a Jupyter server running, you will need to restart it for this to take effect.
+
+## Simple usage
+
+Let's say you have a project and keep your notebooks in a `notebooks/` subdirectory.
+
+To configure that directory for automatic exporting, run the following command:
+
+```bash
+nbautoexport configure notebooks
+```
+
+This will create a configuration file `notebooks/.nbautoexport`.
+
+If you've set up `nbautoexport` to work with Jupyter (using the `install` command as detailed in the previous section), then any time you save a notebook in Jupyter, a hook will run that checks whether there is a `.nbautoexport` configuration file in the same directory as the notebook. If so, it will use the settings specified in that file to export your notebook. By default, it will generate a script version of your notebook named after the notebook (with the `.py` extension) and saved in the directory `notebooks/script`.
+
+If everything is working, your notebooks directory should end up with files like the below example:
+
+```text
+notebooks
+├──0.1-ejm-data-exploration.ipynb
+├──0.2-ejm-feature-creation.ipynb
+└── script
+    └── 0.1-ejm-data-exploration.py
+    └── 0.2-ejm-feature-creation.py
+```
+
+## Configuring export options
+
+The default `.nbautoexport` configuration file looks like this:
+
+```json
+{
+  "export_formats": [
+    "script"
+  ],
+  "organize_by": "extension"
+}
+```
+
+Upon save, this will lead to notebooks being exported to scripts which saved to the `notebooks/script` directory.
+
+```text
+notebooks
+├──0.1-ejm-data-exploration.ipynb
+├──0.2-ejm-feature-creation.ipynb
+└── script
+    └── 0.1-ejm-data-exploration.py
+    └── 0.2-ejm-feature-creation.py
+```
+
+An alternative way to organize exported files is to create a directory for each notebook. This can be handy for matching both the notebook and subdirectory when tab-completing and then globbing with `*` after the part that completed.
+
+```bash
+nbautoexport configure notebooks --organize-by notebook
+```
+
+```text
+notebooks
+├── 0.1-ejm-data-exploration
+│   └── 0.1-ejm-data-exploration.py
+├── 0.2-ejm-feature-creation
+│   └── 0.2-ejm-feature-creation.py
+├──0.1-ejm-data-exploration.ipynb
+└──0.2-ejm-feature-creation.ipynb
+```
+
+If you do not like the settings you selected, you can always change them by either 1) re-running the `nbautoexport` command with new arguments and the `--overwrite` flag, or 2) manually editing the `.nbautoexport` file.
+
+You can also specify as many export formats as you'd like. We support most of the export formats available from [`nbconvert`](https://nbconvert.readthedocs.io/en/latest/), such as `html`, `md`, and `pdf`. To specify formats, use the `--export-format` for each format you want to include.
+
+
+### Advanced example
+
+```bash
+nbautoexport configure sprint_one_notebooks -f script -f html --organize-by extension
+```
+
+Upon save, this creates `.py` and `.html` versions of the Jupyter notebooks in `sprint_one_notebooks` folder and results in the following organization:
+
+```text
+notebooks
+├──0.1-ejm-data-exploration.ipynb
+├──0.2-ejm-feature-creation.ipynb
+├── script
+│   └── 0.1-ejm-data-exploration.py
+│   └── 0.1-ejm-features-creation.py
+└── html
+    └── 0.1-ejm-data-exploration.html
+    └── 0.1-ejm-features-creation.html
+```
+
+## More functionality
+
+The `nbautoexport` CLI has two additional commands:
+
+- `export` is for ad hoc exporting of a notebook or directory of notebooks
+- `clean` (EXPERIMENTAL) will delete files in a directory that are not generated by the current `.nbautoexport` configuration
+
+Use the `--help` flag to see the documentation.
+
+## Command-line help
+
+```bash
+nbautoexport --help
+```
+
+```text
+Usage: nbautoexport [OPTIONS] COMMAND [ARGS]...
+
+  Automatically export Jupyter notebooks to various file formats (.py,
+  .html, and more) upon save. One great use case is to automatically have
+  script versions of your notebooks to facilitate code review commenting.
+
+  To set up, first use the 'install' command to register nbautoexport with
+  Jupyter. If you already have a Jupyter server running, you will need to
+  restart it.
+
+  Next, you will need to use the 'configure' command to create a
+  .nbautoexport configuration file in the same directory as the notebooks
+  you want to have export automatically.
+
+  Once nbautoexport is installed with the first step, exporting will run
+  automatically when saving a notebook in Jupyter for any notebook where
+  there is a .nbautoexport configuration file in the same directory.
+
+Options:
+  --version             Show nbautoexport version.
+  --install-completion  Install completion for the current shell.
+  --show-completion     Show completion for the current shell, to copy it or
+                        customize the installation.
+
+  --help                Show this message and exit.
+
+Commands:
+  clean      (EXPERIMENTAL) Remove subfolders/files not matching...
+  configure  Create a .nbautoexport configuration file in a directory.
+  export     Manually export notebook or directory of notebooks.
+  install    Register nbautoexport post-save hook with Jupyter.
+```
+
+---
+
+This repository was initially created using [Cookiecutter](https://github.com/audreyr/cookiecutter) with [`audreyr/cookiecutter-pypackage`](https://github.com/audreyr/cookiecutter-pypackage).
+
```

### Comparing `nbautoexport-0.5.0/README.md` & `nbautoexport-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `nbautoexport-0.5.0/nbautoexport/clean.py` & `nbautoexport-0.5.1/nbautoexport/clean.py`

 * *Files identical despite different names*

### Comparing `nbautoexport-0.5.0/nbautoexport/export.py` & `nbautoexport-0.5.1/nbautoexport/export.py`

 * *Files identical despite different names*

### Comparing `nbautoexport-0.5.0/nbautoexport/jupyter_config.py` & `nbautoexport-0.5.1/nbautoexport/jupyter_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         if version_match:
             existing_version = version_match.group()
             logger.debug(f"Existing post-save hook is version {existing_version}")
         else:
             existing_version = ""
             logger.debug("Existing post-save hook predates versioning.")
 
-        if parse_version(existing_version) < parse_version(__version__):
+        if existing_version == "" or parse_version(existing_version) < parse_version(__version__):
             logger.info(f"Updating nbautoexport post-save hook with version {__version__}...")
             with config_path.open("w", encoding="utf-8") as fp:
                 # Open as w replaces existing file. We're replacing entire config.
                 escaped_init = post_save_hook_initialize_block.replace(
                     "\\", r"\\"
                 )  # escape metachars
                 fp.write(block_regex.sub(escaped_init, config))
```

### Comparing `nbautoexport-0.5.0/nbautoexport/nbautoexport.py` & `nbautoexport-0.5.1/nbautoexport/nbautoexport.py`

 * *Files identical despite different names*

### Comparing `nbautoexport-0.5.0/nbautoexport/sentinel.py` & `nbautoexport-0.5.1/nbautoexport/sentinel.py`

 * *Files 16% similar despite different names*

```diff
@@ -46,14 +46,28 @@
     export_formats: List[ExportFormat] = [ExportFormat(fmt) for fmt in DEFAULT_EXPORT_FORMATS]
     organize_by: OrganizeBy = OrganizeBy(DEFAULT_ORGANIZE_BY)
     clean: CleanConfig = CleanConfig()
 
     class Config:
         extra = "forbid"
 
+    # deprecated in pydantic v2.0
+    def json(self, *args, **kwargs):
+        if hasattr(self, "model_dump_json"):
+            return self.model_dump_json(*args, **kwargs)
+        else:
+            return super().json(*args, **kwargs)
+
+    # deprecated in pydantic v2.0
+    def dict(self, *args, **kwargs):
+        if hasattr(self, "model_dump"):
+            return self.model_dump(*args, **kwargs)
+        else:
+            return super().dict(*args, **kwargs)
+
 
 def install_sentinel(directory: Path, config: NbAutoexportConfig, overwrite: bool):
     """Writes the configuration file to a specified directory."""
     sentinel_path = directory / SAVE_PROGRESS_INDICATOR_FILE
 
     if sentinel_path.exists() and (not overwrite):
         raise FileExistsError(
```

### Comparing `nbautoexport-0.5.0/nbautoexport/utils.py` & `nbautoexport-0.5.1/nbautoexport/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,23 +2,26 @@
 import logging
 import os
 from pathlib import Path
 import sys
 from typing import List
 from warnings import warn
 
+if sys.version_info[:2] >= (3, 8):
+    import importlib.metadata as importlib_metadata
+else:
+    import importlib_metadata
+
 from pydantic import BaseModel
 from nbconvert.exporters import get_export_names, get_exporter
 import nbformat
 from jupyter_core.application import JupyterApp
 
-from nbautoexport._version import get_versions
-
 
-__version__ = get_versions()["version"]
+__version__ = importlib_metadata.version("nbautoexport")
 
 
 def get_logger():
     if JupyterApp.initialized():
         return JupyterApp.instance().log
     else:
         logger = logging.getLogger("nbautoexport")
@@ -26,14 +29,18 @@
         return logger
 
 
 class JupyterNotebook(BaseModel):
     path: Path
     metadata: nbformat.notebooknode.NotebookNode
 
+    class Config:
+        # NotebookNode not pydantic v2 compatible
+        arbitrary_types_allowed = True
+
     def get_script_extension(self):
         # Match logic of nbconvert.exporters.script.ScriptExporter
         # Order of precedence is: nb_convert_exporter, language, file_extension, .txt
         lang_info = self.metadata.get("language_info", {})
         if "nbconvert_exporter" in lang_info:
             return get_exporter(lang_info.nbconvert_exporter)().file_extension
         if "name" in lang_info and lang_info.name in get_export_names():
@@ -46,14 +53,21 @@
 
     @classmethod
     def from_file(cls, path):
         notebook = nbformat.read(path, as_version=nbformat.NO_CONVERT)
         nbformat.validate(notebook)
         return cls(path=path, metadata=notebook.metadata)
 
+    # deprecated in pydantic v2.0
+    def json(self, *args, **kwargs):
+        if hasattr(self, "model_dump_json"):
+            return self.model_dump_json(*args, **kwargs)
+        else:
+            return super().json(*args, **kwargs)
+
     def __hash__(self):
         return hash(self.json())
 
 
 def find_notebooks(directory: Path) -> List[JupyterNotebook]:
     """Finds Jupyter notebooks in a directory. Not recursive.
```

### Comparing `nbautoexport-0.5.0/setup.py` & `nbautoexport-0.5.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,66 +1,88 @@
-#!/usr/bin/env python
-
-"""The setup script."""
-
-from setuptools import setup, find_packages
-from pathlib import Path
-
-import versioneer
-
-
-def load_requirements(path: Path):
-    requirements = []
-    with path.open("r", encoding="utf-8") as fp:
-        for line in fp.readlines():
-            if line.startswith("-r"):
-                requirements += load_requirements(line.split(" ")[1].strip())
-            else:
-                requirement = line.strip()
-                if requirement and not requirement.startswith("#"):
-                    requirements.append(requirement)
-    return requirements
-
-
-readme = Path("README.md").read_text()
-history = Path("HISTORY.md").read_text()
-
-requirements = load_requirements(Path(__file__).parent / "requirements.txt")
-
-setup(
-    author="DrivenData",
-    author_email="info@drivendata.org",
-    python_requires=">=3.7",
-    classifiers=[
-        "Framework :: Jupyter",
-        "Intended Audience :: Developers",
-        "Intended Audience :: Science/Research",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-    ],
-    description=(
-        "Automatically export Jupyter notebooks to various file formats (.py, .html, and more) on "
-        "save."
-    ),
-    entry_points={"console_scripts": ["nbautoexport=nbautoexport.nbautoexport:app"]},
-    install_requires=requirements,
-    long_description=readme + "\n\n" + history,
-    long_description_content_type="text/markdown",
-    include_package_data=True,
-    keywords=["nbautoexport", "jupyter", "nbconvert"],
-    name="nbautoexport",
-    packages=find_packages(include=["nbautoexport", "nbautoexport.*"]),
-    project_urls={
-        "Bug Tracker": "https://github.com/drivendataorg/nbautoexport/issues",
-        "Documentation": "https://nbautoexport.drivendata.org/",
-        "Source Code": "https://github.com/drivendataorg/nbautoexport",
-    },
-    url="https://github.com/drivendataorg/nbautoexport",
-    version=versioneer.get_version(),
-    cmdclass=versioneer.get_cmdclass(),
-    zip_safe=False,
-)
+[build-system]
+requires = [
+    "pdm-pep517",
+]
+build-backend = "pdm.pep517.api"
+
+[project]
+name = "nbautoexport"
+dynamic = []
+description = "Automatically export Jupyter notebooks to various file formats (.py, .html, and more) on save."
+readme = "README.md"
+authors = [
+    { name = "DrivenData", email = "info@drivendata.org" },
+]
+license = "MIT"
+keywords = [
+    "nbautoexport",
+    "jupyter",
+    "nbconvert",
+]
+classifiers = [
+    "Framework :: Jupyter",
+    "Intended Audience :: Developers",
+    "Intended Audience :: Science/Research",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+]
+requires-python = ">=3.7"
+dependencies = [
+    "importlib_metadata ; python_version < '3.8'",
+    "jupyter_core",
+    "nbconvert>=5.6.1",
+    "nbformat",
+    "notebook",
+    "packaging",
+    "pydantic",
+    "traitlets",
+    "typer>=0.3.0",
+]
+version = "0.5.1"
+
+[project.scripts]
+nbautoexport = "nbautoexport.nbautoexport:app"
+
+[project.urls]
+Homepage = "https://github.com/drivendataorg/nbautoexport"
+Repository = "https://github.com/drivendataorg/nbautoexport"
+Documentation = "https://nbautoexport.drivendata.org/"
+"Bug Tracker" = "https://github.com/drivendataorg/nbautoexport/issues"
+Changelog = "https://nbautoexport.drivendata.org/stable/changelog/"
+
+[tool.pdm.version]
+source = "scm"
+
+[tool.black]
+line-length = 99
+include = "\\.pyi?$"
+exclude = "/(\n    \\.git\n  | \\.venv\n)/\n"
+
+[tool.mypy]
+ignore_missing_imports = true
+allow_redefinition = true
+
+[tool.mypy-nbautoexport._version]
+ignore_errors = true
+
+[tool.pytest.ini_options]
+minversion = "6.0"
+addopts = "--cov=nbautoexport --cov-report=term --cov-report=html --cov-report=xml"
+testpaths = [
+    "tests",
+]
+
+[tool.coverage.run]
+source = [
+    "nbautoexport",
+]
+
+[tool.coverage.report]
+include = [
+    "nbautoexport/**/*.py",
+]
```

### Comparing `nbautoexport-0.5.0/tests/assets/the_notebook.ipynb` & `nbautoexport-0.5.1/tests/assets/the_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `nbautoexport-0.5.0/tests/test_clean.py` & `nbautoexport-0.5.1/tests/test_clean.py`

 * *Files identical despite different names*

### Comparing `nbautoexport-0.5.0/tests/test_cli.py` & `nbautoexport-0.5.1/tests/test_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 
 
 def test_no_command():
     """Test the CLI errors with no command."""
     runner = CliRunner()
     result = runner.invoke(app)
     assert result.exit_code > 0
-    assert "Error: Missing command." in result.output
+    assert "Error" in result.output
+    assert "Missing command." in result.output
 
 
 def test_help():
     """Test the CLI main callback with --help flag."""
     runner = CliRunner()
     result = runner.invoke(app, ["--help"])
     assert result.exit_code == 0
@@ -37,15 +38,16 @@
     result = subprocess.run(
         ["python", "-m", "nbautoexport"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         universal_newlines=True,
     )
     assert result.returncode > 0
-    assert "Error: Missing command." in result.stderr
+    assert "Error" in result.stderr
+    assert "Missing command." in result.stderr
     assert result.stderr.startswith("Usage: python -m nbautoexport")
     assert "Usage: __main__.py" not in result.stderr
 
 
 def test_version_python_m():
     result = subprocess.run(
         ["python", "-m", "nbautoexport", "--version"],
```

### Comparing `nbautoexport-0.5.0/tests/test_cli_clean.py` & `nbautoexport-0.5.1/tests/test_cli_clean.py`

 * *Files 4% similar despite different names*

```diff
@@ -202,15 +202,15 @@
     with sentinel_path.open("w", encoding="utf-8") as fp:
         fp.write(NbAutoexportConfig(export_formats=EXPECTED_FORMATS).json())
 
     starting_files = set(notebooks_dir.glob("**/*"))
 
     result = CliRunner().invoke(app, ["clean", str(notebooks_dir)], input="n")
     assert result.exit_code == 1
-    assert result.stdout.endswith("Aborted!\n")
+    assert "Aborted" in result.stdout.strip()[-8:]
 
     ending_files = set(notebooks_dir.glob("**/*"))
 
     # no files deleted
     assert starting_files == ending_files
 
 
@@ -230,24 +230,26 @@
     assert starting_files == ending_files
 
 
 def test_clean_no_directory_error():
     result = CliRunner().invoke(app, ["clean"])
 
     assert result.exit_code == 2
-    assert "Error: Missing argument 'DIRECTORY'." in result.stdout
+    assert "Error" in result.stdout
+    assert "Missing argument 'DIRECTORY'." in result.stdout
 
 
 def test_clean_missing_config_error(notebooks_dir):
     sentinel_path = notebooks_dir / SAVE_PROGRESS_INDICATOR_FILE
 
     starting_files = set(notebooks_dir.glob("**/*"))
 
     result = CliRunner().invoke(app, ["clean", str(notebooks_dir)])
     assert result.exit_code == 1
-    assert "Error: Missing expected nbautoexport config file" in result.stdout
+    assert "Error" in result.stdout
+    assert "Missing expected nbautoexport config file" in result.stdout
     assert str(sentinel_path.resolve()) in result.stdout
 
     ending_files = set(notebooks_dir.glob("**/*"))
 
     # no files deleted
     assert starting_files == ending_files
```

### Comparing `nbautoexport-0.5.0/tests/test_cli_configure.py` & `nbautoexport-0.5.1/tests/test_cli_configure.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,15 +60,16 @@
     assert config == expected_config
 
 
 def test_invalid_export_format():
     runner = CliRunner()
     result = runner.invoke(app, ["configure", "-f", "invalid-output-format"])
     assert result.exit_code == 2
-    assert "Error: Invalid value for '--export-format' / '-f'" in result.output
+    assert "Error" in result.output
+    assert "Invalid value for '--export-format' / '-f'" in result.output
     assert "invalid-output-format" in result.output
 
 
 def test_invalid_organize_by():
     runner = CliRunner()
     result = runner.invoke(app, ["configure", "-b", "invalid-organize-by"])
     assert result.exit_code == 2
@@ -90,15 +91,17 @@
     result = runner.invoke(
         app, ["configure", str(tmp_path), "-o", "-f", "script", "-f", "html", "-b", "notebook"]
     )
     assert result.exit_code == 0
     with (tmp_path / ".nbautoexport").open("r", encoding="utf-8") as fp:
         config = json.load(fp)
 
-    expected_config = NbAutoexportConfig(export_formats=["script", "html"], organize_by="notebook")
+    expected_config = NbAutoexportConfig(
+        export_formats=["script", "html"], organize_by="notebook"
+    ).dict()
     assert config == expected_config
 
 
 def test_configure_no_jupyter_config_warning(tmp_path, monkeypatch):
     monkeypatch.setenv("JUPYTER_CONFIG_DIR", str(tmp_path))
 
     result = CliRunner().invoke(app, ["configure", str(tmp_path)])
@@ -148,8 +151,9 @@
     assert "Warning:" not in result.output
 
 
 def test_configure_no_directory_error():
     result = CliRunner().invoke(app, ["configure"])
 
     assert result.exit_code == 2
-    assert "Error: Missing argument 'DIRECTORY'." in result.stdout
+    assert "Error" in result.stdout
+    assert "Missing argument 'DIRECTORY'." in result.stdout
```

### Comparing `nbautoexport-0.5.0/tests/test_cli_export.py` & `nbautoexport-0.5.1/tests/test_cli_export.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from itertools import chain, product
 from pathlib import Path
+import re
 import shutil
 
 import pytest
 from typer.testing import CliRunner
 
 from nbautoexport.clean import get_expected_exports
 from nbautoexport.nbautoexport import app
@@ -221,15 +222,16 @@
 
 
 def test_export_notebook_doesnt_exist_error(tmp_path):
     nonexistent_notebook = tmp_path / "anne_hughes_diary.ipynb"
     assert not nonexistent_notebook.exists()
     result = CliRunner().invoke(app, ["export", str(nonexistent_notebook)])
     assert result.exit_code == 2
-    assert "does not exist" in result.stdout
+    assert re.search("does[^a-zA-Z]+not[^a-zA-Z]+exist", result.stdout)
 
 
 def test_export_no_input_error():
     result = CliRunner().invoke(app, ["export"])
 
     assert result.exit_code == 2
-    assert "Error: Missing argument 'INPUT'." in result.stdout
+    assert "Error" in result.stdout
+    assert "Missing argument 'INPUT'." in result.stdout
```

### Comparing `nbautoexport-0.5.0/tests/test_cli_install.py` & `nbautoexport-0.5.1/tests/test_cli_install.py`

 * *Files identical despite different names*

### Comparing `nbautoexport-0.5.0/tests/test_export.py` & `nbautoexport-0.5.1/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `nbautoexport-0.5.0/tests/test_jupyter_config.py` & `nbautoexport-0.5.1/tests/test_jupyter_config.py`

 * *Files identical despite different names*

### Comparing `nbautoexport-0.5.0/tests/test_post_save.py` & `nbautoexport-0.5.1/tests/test_post_save.py`

 * *Files identical despite different names*

### Comparing `nbautoexport-0.5.0/tests/test_sentinel.py` & `nbautoexport-0.5.1/tests/test_sentinel.py`

 * *Files identical despite different names*

### Comparing `nbautoexport-0.5.0/tests/test_utils.py` & `nbautoexport-0.5.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `nbautoexport-0.5.0/tests/utils.py` & `nbautoexport-0.5.1/tests/utils.py`

 * *Files identical despite different names*

