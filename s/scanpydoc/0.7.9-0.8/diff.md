# Comparing `tmp/scanpydoc-0.7.9.tar.gz` & `tmp/scanpydoc-0.8.tar.gz`

## Comparing `scanpydoc-0.7.9.tar` & `scanpydoc-0.8.tar`

### file list

```diff
@@ -1,36 +1,37 @@
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/.editorconfig
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/.pre-commit-config.yaml
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/.prettierrc
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/.readthedocs.yml
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/.github/workflows/ci.yml
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/.vscode/settings.json
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/docs/conf.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/docs/index.rst
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/docs/_templates/autosummary/base.rst
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/docs/_templates/autosummary/module.rst
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/src/scanpydoc/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/src/scanpydoc/_version.py
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/src/scanpydoc/autosummary_generate_imported.py
--rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/src/scanpydoc/definition_list_typed_field.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/src/scanpydoc/py.typed
--rw-r--r--   0        0        0     5393 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/src/scanpydoc/rtd_github_links.py
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/src/scanpydoc/elegant_typehints/__init__.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/src/scanpydoc/elegant_typehints/autodoc_patch.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/src/scanpydoc/elegant_typehints/example.py
--rw-r--r--   0        0        0     5153 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/src/scanpydoc/elegant_typehints/formatting.py
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/src/scanpydoc/elegant_typehints/return_tuple.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/src/scanpydoc/elegant_typehints/static/typehints.css
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/src/scanpydoc/theme/__init__.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/src/scanpydoc/theme/layout.html
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/src/scanpydoc/theme/theme.conf
--rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/src/scanpydoc/theme/static/css/scanpy.css
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/tests/conftest.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/tests/test_base.py
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/tests/test_definition_list_typed_field.py
--rw-r--r--   0        0        0     9756 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/tests/test_elegant_typehints.py
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/tests/test_rtd_github_links.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/.gitignore
--rw-r--r--   0        0        0    32422 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/LICENSE
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/README.rst
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/pyproject.toml
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 scanpydoc-0.7.9/PKG-INFO
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 scanpydoc-0.8/.editorconfig
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 scanpydoc-0.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 scanpydoc-0.8/.prettierrc.yaml
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 scanpydoc-0.8/.readthedocs.yml
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 scanpydoc-0.8/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 scanpydoc-0.8/.vscode/settings.json
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 scanpydoc-0.8/docs/conf.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 scanpydoc-0.8/docs/index.rst
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 scanpydoc-0.8/docs/_templates/autosummary/base.rst
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 scanpydoc-0.8/docs/_templates/autosummary/module.rst
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 scanpydoc-0.8/src/scanpydoc/__init__.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 scanpydoc-0.8/src/scanpydoc/_version.py
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 scanpydoc-0.8/src/scanpydoc/autosummary_generate_imported.py
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 scanpydoc-0.8/src/scanpydoc/definition_list_typed_field.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scanpydoc-0.8/src/scanpydoc/py.typed
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 scanpydoc-0.8/src/scanpydoc/elegant_typehints/__init__.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 scanpydoc-0.8/src/scanpydoc/elegant_typehints/autodoc_patch.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 scanpydoc-0.8/src/scanpydoc/elegant_typehints/example.py
+-rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 scanpydoc-0.8/src/scanpydoc/elegant_typehints/formatting.py
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 scanpydoc-0.8/src/scanpydoc/elegant_typehints/return_tuple.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 scanpydoc-0.8/src/scanpydoc/elegant_typehints/static/typehints.css
+-rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 scanpydoc-0.8/src/scanpydoc/rtd_github_links/__init__.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 scanpydoc-0.8/src/scanpydoc/rtd_github_links/_linkcode.py
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 scanpydoc-0.8/src/scanpydoc/theme/__init__.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 scanpydoc-0.8/src/scanpydoc/theme/layout.html
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 scanpydoc-0.8/src/scanpydoc/theme/theme.conf
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 scanpydoc-0.8/src/scanpydoc/theme/static/styles/scanpy.css
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 scanpydoc-0.8/tests/conftest.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 scanpydoc-0.8/tests/test_base.py
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 scanpydoc-0.8/tests/test_definition_list_typed_field.py
+-rw-r--r--   0        0        0     9756 2020-02-02 00:00:00.000000 scanpydoc-0.8/tests/test_elegant_typehints.py
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 scanpydoc-0.8/tests/test_rtd_github_links.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 scanpydoc-0.8/.gitignore
+-rw-r--r--   0        0        0    32422 2020-02-02 00:00:00.000000 scanpydoc-0.8/LICENSE
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 scanpydoc-0.8/README.rst
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 scanpydoc-0.8/pyproject.toml
+-rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 scanpydoc-0.8/PKG-INFO
```

### Comparing `scanpydoc-0.7.9/.github/workflows/ci.yml` & `scanpydoc-0.8/.github/workflows/ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -24,10 +24,10 @@
           path: |
             ~/.cache/pip
             ~/.cache/pre-commit
           key: ${{ runner.os }}-pip-${{ hashFiles('pyproject.toml') }}
       - name: dependencies
         run: |
           pip install --upgrade pip wheel
-          pip install .[test,typehints]
+          pip install -e .[test,typehints]
       - name: tests
         run: pytest --color=yes
```

### Comparing `scanpydoc-0.7.9/docs/conf.py` & `scanpydoc-0.8/docs/conf.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,68 +1,70 @@
 import sys
 from datetime import datetime
+from importlib.metadata import metadata
 from pathlib import Path
 
 from sphinx.application import Sphinx
 
 
-# Allow importing scanpydoc itself
 HERE = Path(__file__).parent
-sys.path.insert(0, str(HERE.parent))
-import scanpydoc  # noqa
 
+# necessary for rtd_gh_links’ linkcode support
+sys.path.insert(0, HERE.parent / "src")
 
 # Clean build env
 for file in HERE.glob("scanpydoc.*.rst"):
     file.unlink()
 
-
-needs_sphinx = "1.7"  # autosummary bugfix
 extensions = [
     "sphinx.ext.intersphinx",
     "sphinx.ext.napoleon",
     "sphinx_autodoc_typehints",  # needs to be after napoleon
     "sphinx.ext.autodoc",
     "sphinx.ext.autosummary",
     "scanpydoc",
+    "sphinx.ext.linkcode",  # needs to be after scanpydoc
 ]
 
 intersphinx_mapping = dict(
     python=("https://docs.python.org/3", None),
     jinja=("https://jinja.palletsprojects.com/en/2.10.x/", None),
     sphinx=("https://www.sphinx-doc.org/en/master/", None),
-    sphinx_rtd_theme=("https://sphinx-rtd-theme.readthedocs.io/en/stable/", None),
+    sphinx_book_theme=("https://sphinx-book-theme.readthedocs.io/en/stable/", None),
     # examples
     numpy=("https://numpy.org/doc/stable/", None),
     anndata=("https://anndata.readthedocs.io/en/latest/", None),
     pandas=("https://pandas.pydata.org/pandas-docs/stable/", None),
     scipy=("https://docs.scipy.org/doc/scipy/", None),
 )
 
 # general information
-project = scanpydoc.__name__
-author = "Philipp Angerer"
+meta = metadata("scanpydoc")
+project = meta["name"]
+author = meta["author-email"].split(" <")[0]
 copyright = f"{datetime.now():%Y}, {author}."
-version = release = scanpydoc.__version__
+version = release = meta["version"]
 
 master_doc = "index"
 templates_path = ["_templates"]
 
 # Generate .rst stubs for modules using autosummary
 autosummary_generate = True
 # Don’t add module paths to documented functions’ names
 add_module_names = False
 
 html_theme = "scanpydoc"
 html_context = dict(
-    github_user="theislab", github_repo="scanpydoc", github_version="main"
+    repository_url="https://github.com/theislab/scanpydoc",
+    repository_branch="main",
+    use_repository_button=True,
 )
 
-# proj/doc/conf.py/../.. → proj
-project_dir = Path(__file__).parent.parent
+# proj/doc/.. → proj
+project_dir = HERE.parent
 
 
 def setup(app: Sphinx):
     app.add_object_type(
         "confval",
         "confval",
         objname="configuration value",
```

### Comparing `scanpydoc-0.7.9/docs/_templates/autosummary/module.rst` & `scanpydoc-0.8/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.7.9/src/scanpydoc/__init__.py` & `scanpydoc-0.8/src/scanpydoc/__init__.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.7.9/src/scanpydoc/autosummary_generate_imported.py` & `scanpydoc-0.8/src/scanpydoc/autosummary_generate_imported.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.7.9/src/scanpydoc/definition_list_typed_field.py` & `scanpydoc-0.8/src/scanpydoc/definition_list_typed_field.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,35 +44,41 @@
 
         def make_refs(role_name, name, node):
             return self.make_xrefs(role_name, domain, name, node, env=env, **kw)
 
         def handle_item(
             fieldarg: str, content: list[nodes.inline]
         ) -> nodes.definition_list_item:
-            head = nodes.term()
-            head += make_refs(self.rolename, fieldarg, addnodes.literal_strong)
+            term = nodes.term()
+            term += make_refs(self.rolename, fieldarg, addnodes.literal_strong)
+
             field_type = types.pop(fieldarg, None)
             if field_type is not None:
-                head += nodes.Text(" : ")
                 if len(field_type) == 1 and isinstance(field_type[0], nodes.Text):
                     (text_node,) = field_type  # type: nodes.Text
-                    head += make_refs(
+                    classifier_content = make_refs(
                         self.typerolename, text_node.astext(), addnodes.literal_emphasis
                     )
                 else:
-                    head += field_type
+                    classifier_content = field_type
+                term += [
+                    # https://github.com/sphinx-doc/sphinx/issues/10815
+                    nodes.Text(" "),
+                    # Sphinx tries to fixup classifiers without rawsource,
+                    # but for this expects attributes we don’t have. Thus “×”.
+                    nodes.classifier("×", "", *classifier_content),
+                ]
 
-            body_content = nodes.paragraph("", "", *content)
-            body = nodes.definition("", body_content)
+            def_content = nodes.paragraph("", "", *content)
+            definition = nodes.definition("", def_content)
 
-            return nodes.definition_list_item("", head, body)
+            return nodes.definition_list_item("", term, definition)
 
         field_name = nodes.field_name("", self.label)
         assert not self.can_collapse
-        # “simple” for pydata sphinx theme
         body_node = self.list_type(classes=["simple"])
         for field_arg, content in items:
             body_node += handle_item(field_arg, content)
         field_body = nodes.field_body("", body_node)
         return nodes.field("", field_name, field_body)
```

### Comparing `scanpydoc-0.7.9/src/scanpydoc/rtd_github_links.py` & `scanpydoc-0.8/src/scanpydoc/rtd_github_links/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,72 +1,103 @@
 """GitHub URLs for class and method pages.
 
-This extension registers a :ref:`Jinja filter <jinja:filters>` called :func:`github_url`
-that you can use to convert a module path into a GitHub URL
+This extension does two things:
+
+#. It registers a :ref:`Jinja filter <jinja:filters>` called :func:`github_url`
+   that you can use to convert a module path into a GitHub URL.
+#. It configures :mod:`sphinx.ext.linkcode` for you if loaded after it in ``conf.py``:
+
+   .. code:: python
+
+      import sys
+      from pathlib import Path
+
+      HERE = Path(__file__).parent
+      # make sure modules are import from the right place
+      sys.path.insert(0, HERE.parent / "src")
+
+      extensions = [
+          "scanpydoc",
+          "sphinx.ext.linkcode",
+      ]
+
+      # no need to define `linkcode_resolve`
 
 Configuration
 -------------
 
 Uses the following config values in ``conf.py``::
 
     project_dir: Path = ...  # default: Path.cwd()
+
+    # sphinx book theme style
+    html_context = dict(
+        repository_url=...,
+        repository_branch=...,
+    )
+    # or RTD theme style:
     html_context = dict(
         github_user=...,
         github_repo=...,
         github_version=...,
     )
 
 The ``project_dir`` is used to figure out the .py file path relative to the git root,
 that is to construct the path in the github URL.
 
-The ``html_context`` is e.g. also used like this in the sphinx_rtd_theme_.
+Which ``html_context`` style you want to use depends on your theme, e.g.
+:doc:`Sphinx Book Theme <sphinx_book_theme:index>`.
 
-Usage
------
+``:github_url:`` usage
+----------------------
 
 You can use the filter e.g. in `autosummary templates`_.
-To configure the sphinx_rtd_theme_,
+To configure the :doc:`Sphinx Book Theme <sphinx_book_theme:index>`,
 override the ``autosummary/base.rst`` template like this:
 
 .. code:: restructuredtext
 
     :github_url: {{ fullname | github_url }}
 
     {% extends "!autosummary/base.rst" %}
 
 .. _autosummary templates: \
    http://www.sphinx-doc.org/en/master/usage/extensions/autosummary.html#customizing-templates
-.. _sphinx_rtd_theme: https://sphinx-rtd-theme.readthedocs.io/en/latest/
 """
 from __future__ import annotations
 
 import inspect
 import sys
 from pathlib import Path, PurePosixPath
 from types import ModuleType
 from typing import Any
 
 from jinja2.defaults import DEFAULT_FILTERS
 from sphinx.application import Sphinx
 from sphinx.config import Config
 
-from . import _setup_sig, metadata
+from .. import _setup_sig, metadata
 
 
 project_dir = None  # type: Path
 github_base_url = None  # type: str
 
 
 def _init_vars(app: Sphinx, config: Config):
     """Called when ``conf.py`` has been loaded."""
     global github_base_url, project_dir
     _check_html_context(config)
-    github_base_url = "https://github.com/{github_user}/{github_repo}/tree/{github_version}".format_map(
-        config.html_context
-    )
+    try:
+        github_base_url = "https://github.com/{github_user}/{github_repo}/tree/{github_version}".format_map(
+            config.html_context
+        )
+    except KeyError:
+        github_base_url = "{repository_url}/tree/{repository_branch}".format_map(
+            config.html_context
+        )
     project_dir = Path(config.project_dir)
 
 
 def _get_obj_module(qualname: str) -> tuple[Any, ModuleType]:
     """Get a module/class/attribute and its original module by qualname."""
     modname = qualname
     attr_path = []
@@ -106,52 +137,54 @@
         return start, start + len(lines) - 1
 
 
 def github_url(qualname: str) -> str:
     """Get the full GitHub URL for some object’s qualname.
 
     Args:
-    ----
         qualname: The full qualified name of a function, class, method or module
 
     Returns:
-    -------
         A GitHub URL derived from the :confval:`html_context`.
     """
     try:
         obj, module = _get_obj_module(qualname)
     except Exception:
         print(f"Error in github_url({qualname!r}):", file=sys.stderr)
         raise
-    try:
+    try:  # only works when installed in dev mode
         path = PurePosixPath(Path(module.__file__).resolve().relative_to(project_dir))
     except ValueError:
-        # trying to document something from another package
-        path = "/".join(module.__file__.split("/")[-2:])
+        # no dev mode or something from another package
+        path = PurePosixPath(*module.__file__.split("/")[-2:])
+        if (project_dir / "src").is_dir():
+            path = "src" / path
     start, end = _get_linenos(obj)
     fragment = f"#L{start}-L{end}" if start and end else ""
     return f"{github_base_url}/{path}{fragment}"
 
 
 def _check_html_context(config: Config):
     try:
-        html_context = config.html_context
+        html_context: dict[str, Any] = config.html_context
     except AttributeError:
         raise ValueError(
             f"Extension {__name__} needs “html_context” to be defined in conf.py"
         )
-    missing_values = {
-        "github_user",
-        "github_repo",
-        "github_version",
-    } - html_context.keys()
-    if missing_values:
-        mvs = ", ".join([f"html_context[{mv!r}]" for mv in missing_values])
+    options = [
+        {"github_user", "github_repo", "github_version"},
+        {"repository_url", "repository_branch"},
+    ]
+    missing_value_sets = [opt - html_context.keys() for opt in options]
+    if all(missing_value_sets):
+        mvs = " or ".join(
+            ", ".join(repr(mv) for mv in mvs) for mvs in missing_value_sets
+        )
         raise ValueError(
-            f"Extension {__name__} needs “{mvs}” to be defined in conf.py.\n"
+            f"Extension {__name__} needs html_context {mvs} to be defined in conf.py.\n"
             f"html_context = {html_context!r}"
         )
 
 
 @_setup_sig
 def setup(app: Sphinx) -> dict[str, Any]:
     """Register the :func:`github_url` :ref:`Jinja filter <jinja:filters>`."""
@@ -161,14 +194,20 @@
         proj_dir = proj_dir.parent
     elif not (proj_dir / "docs").is_dir():
         proj_dir = proj_dir.parent
 
     app.add_config_value("project_dir", proj_dir, "")
     app.connect("config-inited", _init_vars)
 
+    # if linkcode config not set
+    if "linkcode_resolve" not in app.config or app.config["linkcode_resolve"] is None:
+        from ._linkcode import linkcode_resolve
+
+        app.config["linkcode_resolve"] = linkcode_resolve
+
     # html_context doesn’t apply to autosummary templates ☹
     # and there’s no way to insert filters into those templates
     # so we have to modify the default filters
     DEFAULT_FILTERS["github_url"] = github_url
 
     return metadata
```

### Comparing `scanpydoc-0.7.9/src/scanpydoc/elegant_typehints/__init__.py` & `scanpydoc-0.8/src/scanpydoc/elegant_typehints/__init__.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.7.9/src/scanpydoc/elegant_typehints/autodoc_patch.py` & `scanpydoc-0.8/src/scanpydoc/elegant_typehints/autodoc_patch.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.7.9/src/scanpydoc/elegant_typehints/formatting.py` & `scanpydoc-0.8/src/scanpydoc/elegant_typehints/formatting.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,20 +81,18 @@
 def format_annotation(annotation: type[Any], config: Config) -> str | None:
     """Generate reStructuredText containing links to the types.
 
     Unlike :func:`sphinx_autodoc_typehints.format_annotation`,
     it tries to achieve a simpler style as seen in numeric packages like numpy.
 
     Args:
-    ----
         annotation: A type or class used as type annotation.
         config: Sphinx config containing ``sphinx-autodoc-typehints``’s options.
 
     Returns:
-    -------
         reStructuredText describing the type
     """
     curframe = inspect.currentframe()
     calframe = inspect.getouterframes(curframe, 2)
     if calframe[2].function in {"process_docstring", "_inject_signature"} or (
         calframe[2].function == "_inject_types_to_docstring"
         and calframe[3].function == "process_docstring"
```

### Comparing `scanpydoc-0.7.9/src/scanpydoc/elegant_typehints/return_tuple.py` & `scanpydoc-0.8/src/scanpydoc/elegant_typehints/return_tuple.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.7.9/src/scanpydoc/theme/__init__.py` & `scanpydoc-0.8/src/scanpydoc/theme/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""A widescreen extension for :doc:`sphinx_rtd_theme:index`.
+"""A widescreen extension for :doc:`sphinx_book_theme:index`.
 
 Add to ``conf.py``:
 
 .. code:: python
 
    html_theme = 'scanpydoc'
 
@@ -15,22 +15,22 @@
 .. confval:: accent_color
 
    :type: str
    :default: ``#f07e44``
 
    The CSS color used for the mobile header background and the project name text.
 
-See ``sphinx_rtd_theme``’s :doc:`sphinx_rtd_theme:configuring`, e.g.:
+See ``sphinx_book_theme``’s :doc:`sphinx_book_theme:reference`, e.g.:
 
 .. code:: python
 
    html_theme_options = dict(
-       logo_only=False,
-       accent_color='rebeccapurple',
-       display_version=False,
+       repository_url="https://github.com/theislab/scanpydoc",
+       repository_branch="main",
+       use_repository_button=True,
    )
 
 Docsearch options
 -----------------
 
 These two configuration values are required to use docsearch_:
```

### Comparing `scanpydoc-0.7.9/src/scanpydoc/theme/layout.html` & `scanpydoc-0.8/src/scanpydoc/theme/layout.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,46 @@
-{% extends "sphinx_rtd_theme/layout.html" %}
+{% extends "sphinx_book_theme/layout.html" %}
 
-<!-- Have to use htmltitle to include this earlier as our style -->
-{%- block htmltitle %} {{ super() }} {% if theme_docsearch_key and theme_docsearch_index
-%}
-<link
-    rel="stylesheet"
-    href="https://cdn.jsdelivr.net/npm/docsearch.js@{{ theme_docsearch_js_version }}/dist/cdn/docsearch.min.css"
-/>
-{% endif %} {%- endblock -%}
+{%- block css -%}
+    {{ super() }}
+    {% if theme_docsearch_key and theme_docsearch_index %}
+        <link
+            rel="stylesheet"
+            href="https://cdn.jsdelivr.net/npm/docsearch.js@{{ theme_docsearch_js_version }}/dist/cdn/docsearch.min.css"
+        />
+    {% endif %}
+{%- endblock -%}
 
 <!-- Styles that come last -->
-{%- block extrahead %} {{ super() }} {% if theme_accent_color %}
-<style>
-    :root { --accent-color: {{ theme_accent_color }} }
-</style>
-{% endif %} {% endblock %} {% set safe_version = version if version in ["latest",
-"stable"] else "latest" %} {% block scripts %} {{ super() }} {% if theme_docsearch_key
-and theme_docsearch_index %}
-<script src="https://cdn.jsdelivr.net/npm/docsearch.js@{{ theme_docsearch_js_version }}/dist/cdn/docsearch.min.js"></script>
-<script>
-    document.addEventListener('DOMContentLoaded', () => docsearch({
-      apiKey: '{{ theme_docsearch_key }}',
-      indexName: '{{ theme_docsearch_index }}',
-      inputSelector: '#rtd-search-form > input[name="q"]',
-      algoliaOptions: {
-        facetFilters: ['version:{{ theme_docsearch_doc_version or safe_version }}'],
-        hitsPerPage: 10,
-      },
-      debug: {{ theme_docsearch_debug }},
-    }))
-</script>
-{% endif %} {% endblock %}
+{%- block extrahead -%}
+    {{ super() }}
+    {% if theme_accent_color %}
+        <!-- prettier-ignore-start -->
+        <style>
+        :root { --accent-color: {{ theme_accent_color }} }
+        </style>
+        <!-- prettier-ignore-end -->
+    {% endif %}
+{% endblock %}
+
+{% set safe_version = version if version in ["latest", "stable"] else "latest" %}
+
+{% block scripts %}
+    {{ super() }}
+    {% if theme_docsearch_key and theme_docsearch_index %}
+    <script src="https://cdn.jsdelivr.net/npm/docsearch.js@{{ theme_docsearch_js_version }}/dist/cdn/docsearch.min.js"></script>
+    <!-- prettier-ignore-start -->
+    <script>
+        document.addEventListener('DOMContentLoaded', () => docsearch({
+            apiKey: '{{ theme_docsearch_key }}',
+            indexName: '{{ theme_docsearch_index }}',
+            inputSelector: '#rtd-search-form > input[name="q"]',
+            algoliaOptions: {
+            facetFilters: ['version:{{ theme_docsearch_doc_version or safe_version }}'],
+            hitsPerPage: 10,
+            },
+            debug: {{ theme_docsearch_debug }},
+        }))
+    </script>
+    <!-- prettier-ignore-end -->
+    {% endif %}
+{% endblock %}
```

#### html2text {}

```diff
@@ -1,8 +1,9 @@
-{% extends "sphinx_rtd_theme/layout.html" %}  {%- block htmltitle %} {{ super()
-}} {% if theme_docsearch_key and theme_docsearch_index %}
- {% endif %} {%- endblock -%}  {%- block extrahead %} {{ super() }} {% if
+{% extends "sphinx_book_theme/layout.html" %} {%- block css -%} {{ super() }}
+{% if theme_docsearch_key and theme_docsearch_index %}
+ {% endif %} {%- endblock -%}  {%- block extrahead -%} {{ super() }} {% if
 theme_accent_color %}
- {% endif %} {% endblock %} {% set safe_version = version if version in
+  {% endif %} {% endblock %} {% set safe_version = version if version in
 ["latest", "stable"] else "latest" %} {% block scripts %} {{ super() }} {% if
 theme_docsearch_key and theme_docsearch_index %}
- {% endif %} {% endblock %}
+
+  {% endif %} {% endblock %}
```

### Comparing `scanpydoc-0.7.9/tests/conftest.py` & `scanpydoc-0.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.7.9/tests/test_base.py` & `scanpydoc-0.8/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.7.9/tests/test_definition_list_typed_field.py` & `scanpydoc-0.8/tests/test_definition_list_typed_field.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.7.9/tests/test_elegant_typehints.py` & `scanpydoc-0.8/tests/test_elegant_typehints.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.7.9/tests/test_rtd_github_links.py` & `scanpydoc-0.8/tests/test_rtd_github_links.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,24 +9,22 @@
 
 HERE = Path(__file__).parent
 
 
 @pytest.fixture
 def env(monkeypatch: MonkeyPatch):
     monkeypatch.setattr("scanpydoc.rtd_github_links.github_base_url", ".")
-    monkeypatch.setattr("scanpydoc.rtd_github_links.project_dir", HERE)
+    monkeypatch.setattr("scanpydoc.rtd_github_links.project_dir", HERE.parent)
 
 
 def test_as_function(env):
-    assert github_url("scanpydoc.rtd_github_links") == "./scanpydoc/rtd_github_links.py"
+    pth = "./src/scanpydoc/rtd_github_links/__init__.py"
+    assert github_url("scanpydoc.rtd_github_links") == pth
     s, e = _get_linenos(github_url)
-    assert (
-        github_url("scanpydoc.rtd_github_links.github_url")
-        == f"./scanpydoc/rtd_github_links.py#L{s}-L{e}"
-    )
+    assert github_url("scanpydoc.rtd_github_links.github_url") == f"{pth}#L{s}-L{e}"
 
 
 def test_get_obj_module():
     import sphinx.application as sa
 
     obj, mod = _get_obj_module("scanpydoc.Sphinx")
     assert obj is sa.Sphinx
```

### Comparing `scanpydoc-0.7.9/LICENSE` & `scanpydoc-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.7.9/README.rst` & `scanpydoc-0.8/README.rst`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.7.9/pyproject.toml` & `scanpydoc-0.8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -26,19 +26,19 @@
     'pre-commit',
 ]
 test = [
     'pytest',
     'pytest-cov',
 ]
 doc = [
-    'scanpydoc[typehints]',
-    'sphinx-rtd-theme',
+    'scanpydoc[typehints,theme]',
+    'sphinx',
 ]
 typehints = ['sphinx-autodoc-typehints>=1.15.2']
-theme = ['sphinx-rtd-theme']
+theme = ['sphinx-book-theme>=1.0.1']
 
 [project.entry-points.'sphinx.html_themes']
 scanpydoc = 'scanpydoc.theme'
 
 [tool.ruff]
 select = [
     'E', 'W', # Pycodestyle
@@ -57,20 +57,25 @@
 known-first-party = ['scanpydoc']
 
 [tool.hatch.version]
 source = 'vcs'
 [tool.hatch.build.hooks.vcs]
 version-file = 'src/scanpydoc/_version.py'
 
+[tool.hatch.envs.docs]
+features = ['doc']
+[tool.hatch.envs.docs.scripts]
+build = 'sphinx-build -M html docs docs/_build'
+
 [[tool.hatch.envs.test.matrix]]
 python = ['3.8', '3.9', '3.10', '3.11']
 [tool.hatch.envs.test]
 features = ['test', 'typehints']
 [tool.hatch.envs.test.scripts]
-test = 'pytest -vv'
+run = 'pytest -vv {args}'
 
 [tool.pytest.ini_options]
 addopts = [
     '--import-mode=importlib',
     '-psphinx.testing.fixtures',
 ]
```

### Comparing `scanpydoc-0.7.9/PKG-INFO` & `scanpydoc-0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scanpydoc
-Version: 0.7.9
+Version: 0.8
 Summary: A series of Sphinx extensions to get maintainable numpydoc style documentation.
 Project-URL: Source, https://github.com/theislab/scanpydoc/
 Project-URL: Documentation, https://icb-scanpydoc.readthedocs-hosted.com/
 Author-email: Philipp Angerer <phil.angerer@gmail.com>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
 Classifier: Framework :: Sphinx :: Extension
@@ -13,21 +13,21 @@
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8.1
 Requires-Dist: sphinx>=3.0
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == 'dev'
 Provides-Extra: doc
-Requires-Dist: scanpydoc[typehints]; extra == 'doc'
-Requires-Dist: sphinx-rtd-theme; extra == 'doc'
+Requires-Dist: scanpydoc[theme,typehints]; extra == 'doc'
+Requires-Dist: sphinx; extra == 'doc'
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Provides-Extra: theme
-Requires-Dist: sphinx-rtd-theme; extra == 'theme'
+Requires-Dist: sphinx-book-theme>=1.0.1; extra == 'theme'
 Provides-Extra: typehints
 Requires-Dist: sphinx-autodoc-typehints>=1.15.2; extra == 'typehints'
 Description-Content-Type: text/x-rst
 
 scanpydoc |pypi| |docs| |tests| |checks| |cov|
 ==============================================
```

