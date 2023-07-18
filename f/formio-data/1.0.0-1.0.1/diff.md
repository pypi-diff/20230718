# Comparing `tmp/formio-data-1.0.0.tar.gz` & `tmp/formio-data-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formio-data-1.0.0.tar", max compression
+gzip compressed data, was "formio-data-1.0.1.tar", max compression
```

## Comparing `formio-data-1.0.0.tar` & `formio-data-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1066 2022-06-23 06:15:09.395447 formio-data-1.0.0/LICENSE
--rw-r--r--   0        0        0     6454 2023-07-17 11:36:05.957057 formio-data-1.0.0/README.md
--rw-r--r--   0        0        0      171 2022-06-23 06:15:09.396448 formio-data-1.0.0/formiodata/__init__.py
--rw-r--r--   0        0        0     3516 2023-07-17 11:36:05.957057 formio-data-1.0.0/formiodata/builder.py
--rw-r--r--   0        0        0    37451 2023-07-17 11:36:05.958057 formio-data-1.0.0/formiodata/components.py
--rw-r--r--   0        0        0     4204 2023-01-13 07:53:22.436294 formio-data-1.0.0/formiodata/form.py
--rw-r--r--   0        0        0      979 2022-06-23 06:15:09.396448 formio-data-1.0.0/formiodata/utils.py
--rw-r--r--   0        0        0      541 2023-07-17 11:36:05.958057 formio-data-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     7572 2023-07-17 11:37:40.532253 formio-data-1.0.0/setup.py
--rw-r--r--   0        0        0     7230 2023-07-17 11:37:40.533293 formio-data-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-06-23 06:15:09.395447 formio-data-1.0.1/LICENSE
+-rw-r--r--   0        0        0     6700 2023-07-18 09:56:07.631728 formio-data-1.0.1/README.md
+-rw-r--r--   0        0        0      171 2022-06-23 06:15:09.396448 formio-data-1.0.1/formiodata/__init__.py
+-rw-r--r--   0        0        0     3568 2023-07-18 09:56:07.636728 formio-data-1.0.1/formiodata/builder.py
+-rw-r--r--   0        0        0    37451 2023-07-17 11:36:05.958057 formio-data-1.0.1/formiodata/components.py
+-rw-r--r--   0        0        0     4204 2023-01-13 07:53:22.436294 formio-data-1.0.1/formiodata/form.py
+-rw-r--r--   0        0        0      979 2022-06-23 06:15:09.396448 formio-data-1.0.1/formiodata/utils.py
+-rw-r--r--   0        0        0      541 2023-07-18 09:56:07.636728 formio-data-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     7834 2023-07-18 09:56:25.275981 formio-data-1.0.1/setup.py
+-rw-r--r--   0        0        0     7476 2023-07-18 09:56:25.277065 formio-data-1.0.1/PKG-INFO
```

### Comparing `formio-data-1.0.0/LICENSE` & `formio-data-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `formio-data-1.0.0/README.md` & `formio-data-1.0.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -150,24 +150,40 @@
 #################
 # components path
 #################
 
 # datagrid input
 >> datagridMeasurements = builder.components['datagridMeasurements']
 
->> [print(row.input_components['measurementDatetime'].builder_path_key) for row in datagridMeasurements.rows]
+# Component builder_path_key property
+>> [
+>>     print(row.input_components['measurementDatetime'].builder_path_key)
+>>     for row in datagridMeasurements.rows
+>> ]
 ['pageMeasurements', 'columnsExternal', 'datagridMeasurements', 'measurementDatetime']
 
->> [print(row.input_components['measurementDatetime'].builder_path_labels) for row in datagridMeasurements.rows]
+# Component builder_path_labels property
+>> [
+>>     print(row.input_components['measurementDatetime'].builder_path_labels)
+>>     for row in datagridMeasurements.rows
+>> ]
 ['Page Measurements', 'Columns External', 'Data Grid Measurements', 'Measurement Datetime']
 
->> [print(row.input_components['measurementDatetime'].builder_input_path_key) for row in datagridMeasurements.rows]
+# Component builder_input_path_key property
+>> [
+>>     print(row.input_components['measurementDatetime'].builder_input_path_key)
+>>     for row in datagridMeasurements.rows
+>> ]
 ['datagridMeasurements', 'measurementDatetime']
 
->> [print(row.input_components['measurementDatetime'].builder_input_path_labels) for row in datagridMeasurements.rows]
+# Component builder_input_path_labels property
+>> [
+>>     print(row.input_components['measurementDatetime'].builder_input_path_labels)
+>>     for row in datagridMeasurements.rows
+>> ]
 ['Data Grid Measurements', 'Measurement Datetime']
 
 #################################
 # components (layout, input etc.)
 #################################
 
 # columns
```

### Comparing `formio-data-1.0.0/formiodata/builder.py` & `formio-data-1.0.1/formiodata/builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 # Copyright Nova Code (http://www.novacode.nl)
 # See LICENSE file for full licensing details.
 
 import json
+import logging
 
 from collections import OrderedDict
 from copy import deepcopy
 
 from formiodata import components
 
+logger = logging.getLogger(__name__)
+
 
 class Builder:
 
     def __init__(self, schema_json, **kwargs):
         """
         @param schema_json
         @param lang
@@ -87,15 +90,14 @@
             msg = "Can't instantiate a (raw) component without a type.\n\n" \
                 "Component raw data\n" \
                 "==================\n" \
                 "%s\n"
             logging.warning(msg % component)
             return False
 
-
     @property
     def form(self):
         """
         Placeholder form dict, always empty.  Useful in contexts where the component owner's form
         is requested because there is a need for form data.
         """
         return {}
```

### Comparing `formio-data-1.0.0/formiodata/components.py` & `formio-data-1.0.1/formiodata/components.py`

 * *Files identical despite different names*

### Comparing `formio-data-1.0.0/formiodata/form.py` & `formio-data-1.0.1/formiodata/form.py`

 * *Files identical despite different names*

### Comparing `formio-data-1.0.0/formiodata/utils.py` & `formio-data-1.0.1/formiodata/utils.py`

 * *Files identical despite different names*

### Comparing `formio-data-1.0.0/pyproject.toml` & `formio-data-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "formio-data"
-version = "1.0.0"
+version = "1.0.1"
 homepage = "https://github.com/novacode-nl/python-formio-data"
 description = "formio.js JSON-data API"
 readme = "README.md"
 authors = ["Bob Leers <bob@novacode.nl>"]
 license = "MIT"
 packages = [ { include = "formiodata/**/*.py" } ]
 exclude = ["tests/*"]
```

### Comparing `formio-data-1.0.0/setup.py` & `formio-data-1.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 
 extras_require = \
 {':python_version <= "3.6"': ['python-dateutil>=2.8.2,<3.0.0'],
  'json_logic': ['json_logic_qubit>=0.9.1,<0.10.0']}
 
 setup_kwargs = {
     'name': 'formio-data',
-    'version': '1.0.0',
+    'version': '1.0.1',
     'description': 'formio.js JSON-data API',
-    'long_description': '# formio-data (Python)\n\nformio.js (JSON Form Builder) data API for Python.\n\nFor information about the formio.js project, see https://github.com/formio/formio.js\n\n## Introduction\n\n**python-formio-data** is a Python package, which loads and transforms\nformio.js **Builder JSON** and **Form JSON** into **usable Python objects**.  It\'s main\naim is to provide easy access to a Form its components/fields, also\ncaptured as **Python objects**, which makes this API very versatile and usable.\n\n**Notes about terms:**\n  - **Builder:** The Form Builder which is the design/blueprint of a Form.\n  - **Form:** A filled-in Form, aka Form submission.\n  - **Component:** Input (field) or layout component in the Form Builder and Form.\n\n## Features\n\n  - Compatible with Python 3.6 and later\n  - Constructor of the **Builder** and **Form** class, only requires\n    the JSON and an optional language code for translations.\n  - Get a Form object its Components as a usable object e.g. datetime, boolean, dict (for select component) etc.\n  - Open source (MIT License)\n\n## Installation\n\nThe source code is currently hosted on GitHub at:\nhttps://github.com/novacode-nl/python-formio-data\n\n### PyPI - Python Package Index\n\nBinary installers for the latest released version are available at the [Python\nPackage Index](https://pypi.python.org/pypi/formio-data)\n\n```sh\npip(3) install formio-data\n```\n\n#### Optional dependencies\n\nTo support conditional visibility using JSON logic, you can install\nthe `json-logic-qubit` package (the `json-logic` package it is forked\noff of is currently unmaintained).  It\'s also possible to install it\nvia the pip feature `json_logic` like so:\n\n```sh\npip(3) install -U formio-data[json_logic]\n```\n\n### Source Install with Poetry (recommended)\n\nConvenient for developers. Also useful for running the (unit)tests.\n\n```sh\ngit clone git@github.com:novacode-nl/python-formio-data.git\npoetry install\n```\n\n#### Optional dependencies\n\nWhen working in the project itself, use\n\n```sh\npoetry install -E json_logic\n```\n\n### Source Install with pip\n\nOptional dependencies need to be installed separately.\n\n```sh\npip(3) install -U -e python-formio-data\n```\n\n## Using direnv\n\nYou can use [nixpkgs](https://nixos.org/) to run a self-contained\nPython environment without any additional setup.  Once you\'ve\ninstalled nixpkgs, switch into the directory and type "nix-shell" to\nget a shell from which the correct Python with packages is available.\n\nIf you\'re using [direnv](https://direnv.net/), use `direnv allow`\nafter changing into the project directory and you\'re good to go.  Also\nconsider [nix-direnv](https://github.com/nix-community/nix-direnv) to\nspeed up the experience (it can re-use a cached local installation).\n\n## License\n[MIT](LICENSE)\n\n## Contributing\nAll contributions, bug reports, bug fixes, documentation improvements, enhancements and ideas are welcome.\n\n## Usage examples\n\nFor more examples of usage, see the unit-tests.\n\n``` python\n>> from formiodata import Builder, Form\n>>\n# builder_json is a formio.js Builder JSON document (text/string)\n# form_json is a formio.js Form JSON document (text/string)\n>>\n>> builder = Builder(builder_json)\n>> form = Form(builder, form_json)\n\n##################\n# input components\n##################\n\n# textfield label\n>> print(form.input_components[\'firstname\'].label)\n\'First Name\'\n\n# textfield value\n>> print(form.input_components[\'firstname\'].value)\n\'Bob\'\n\n# datetime label\n>> print(form.input_components[\'birthday\'].label)\n\'Birthday\'\n\n# datetime value\n>> print(form.input_components[\'birthday\'].value)\ndatetime.date(2009 10 16)\n\n# datagrid (rows property)\n>> print(form.input_components[\'datagridMeasurements\'].rows)\n[\n  {\'measurementDatetime\': <datetimeComponent>, \'measurementFahrenheit\': <numberComponent>}, \n  {\'measurementDatetime\': <datetimeComponent>, \'measurementFahrenheit\': <numberComponent>}\n]\n\n>> for row in form.input_components[\'datagridMeasurements\'].rows:\n>>    dtime = row[\'measurementDatetime\']\n>>    fahrenheit = row[\'measurementFahrenheit\']\n>>    print(%s: %s, %s: %s\' % (dt.label, dt.value, fahrenheit.label, fahrenheit.value))\n\nDatetime: datetime.datetime(2021, 5, 8, 11, 39, 0, 296487), Fahrenheit: 122\nDatetime: datetime.datetime(2021, 5, 8, 11, 41, 5, 919943), Fahrenheit: 131\n\n# alternative example, by getattr\n>> print(form.data.firstname.label)\n\'First Name\'\n\n>> print(form.data.firstname.value)\n\'Bob\'\n\n#################\n# components path\n#################\n\n# datagrid input\n>> datagridMeasurements = builder.components[\'datagridMeasurements\']\n\n>> [print(row.input_components[\'measurementDatetime\'].builder_path_key) for row in datagridMeasurements.rows]\n[\'pageMeasurements\', \'columnsExternal\', \'datagridMeasurements\', \'measurementDatetime\']\n\n>> [print(row.input_components[\'measurementDatetime\'].builder_path_labels) for row in datagridMeasurements.rows]\n[\'Page Measurements\', \'Columns External\', \'Data Grid Measurements\', \'Measurement Datetime\']\n\n>> [print(row.input_components[\'measurementDatetime\'].builder_input_path_key) for row in datagridMeasurements.rows]\n[\'datagridMeasurements\', \'measurementDatetime\']\n\n>> [print(row.input_components[\'measurementDatetime\'].builder_input_path_labels) for row in datagridMeasurements.rows]\n[\'Data Grid Measurements\', \'Measurement Datetime\']\n\n#################################\n# components (layout, input etc.)\n#################################\n\n# columns\n>> print(form.components[\'addressColumns\'])\n<columnsComponent>\n\n>> print(form.components[\'addressColumns\'].rows)\n[ \n  {\'firstName\': <textfieldComponent>, \'lastName: <textfieldComponent>}, \n  {\'email\': <emailComponent>, \'companyName: <textfieldComponent>}\n]\n```\n\n## Unit tests\n\n**Note:**\n\nInternet access is recommended for running the `filecStorageUrlComponentTestCase`, because this also tests the URL Storage (type).\\\nIf no internet access, this test won\'t fail and a WARNING shall be logged regarding a ConnectionError.\n\n### Run all unittests\n\nFrom toplevel directory:\n\n```\npoetry install -E json_logic  # if you haven\'t already\npoetry run python -m unittest\n```\n\n### Run component unittests\n\nAll Components, from toplevel directory:\n\n```\npoetry run python -m unittest tests/test_component_*.py\n```\n\nNested components (complexity), from toplevel directory:\n\n```\npoetry run python -m unittest tests/test_nested_components.py\n```\n\n### Run specific component unittest\n\n```\npoetry run python -m unittest tests.test_component_day.dayComponentTestCase.test_get_form_dayMonthYear\n```\n',
+    'long_description': '# formio-data (Python)\n\nformio.js (JSON Form Builder) data API for Python.\n\nFor information about the formio.js project, see https://github.com/formio/formio.js\n\n## Introduction\n\n**python-formio-data** is a Python package, which loads and transforms\nformio.js **Builder JSON** and **Form JSON** into **usable Python objects**.  It\'s main\naim is to provide easy access to a Form its components/fields, also\ncaptured as **Python objects**, which makes this API very versatile and usable.\n\n**Notes about terms:**\n  - **Builder:** The Form Builder which is the design/blueprint of a Form.\n  - **Form:** A filled-in Form, aka Form submission.\n  - **Component:** Input (field) or layout component in the Form Builder and Form.\n\n## Features\n\n  - Compatible with Python 3.6 and later\n  - Constructor of the **Builder** and **Form** class, only requires\n    the JSON and an optional language code for translations.\n  - Get a Form object its Components as a usable object e.g. datetime, boolean, dict (for select component) etc.\n  - Open source (MIT License)\n\n## Installation\n\nThe source code is currently hosted on GitHub at:\nhttps://github.com/novacode-nl/python-formio-data\n\n### PyPI - Python Package Index\n\nBinary installers for the latest released version are available at the [Python\nPackage Index](https://pypi.python.org/pypi/formio-data)\n\n```sh\npip(3) install formio-data\n```\n\n#### Optional dependencies\n\nTo support conditional visibility using JSON logic, you can install\nthe `json-logic-qubit` package (the `json-logic` package it is forked\noff of is currently unmaintained).  It\'s also possible to install it\nvia the pip feature `json_logic` like so:\n\n```sh\npip(3) install -U formio-data[json_logic]\n```\n\n### Source Install with Poetry (recommended)\n\nConvenient for developers. Also useful for running the (unit)tests.\n\n```sh\ngit clone git@github.com:novacode-nl/python-formio-data.git\npoetry install\n```\n\n#### Optional dependencies\n\nWhen working in the project itself, use\n\n```sh\npoetry install -E json_logic\n```\n\n### Source Install with pip\n\nOptional dependencies need to be installed separately.\n\n```sh\npip(3) install -U -e python-formio-data\n```\n\n## Using direnv\n\nYou can use [nixpkgs](https://nixos.org/) to run a self-contained\nPython environment without any additional setup.  Once you\'ve\ninstalled nixpkgs, switch into the directory and type "nix-shell" to\nget a shell from which the correct Python with packages is available.\n\nIf you\'re using [direnv](https://direnv.net/), use `direnv allow`\nafter changing into the project directory and you\'re good to go.  Also\nconsider [nix-direnv](https://github.com/nix-community/nix-direnv) to\nspeed up the experience (it can re-use a cached local installation).\n\n## License\n[MIT](LICENSE)\n\n## Contributing\nAll contributions, bug reports, bug fixes, documentation improvements, enhancements and ideas are welcome.\n\n## Usage examples\n\nFor more examples of usage, see the unit-tests.\n\n``` python\n>> from formiodata import Builder, Form\n>>\n# builder_json is a formio.js Builder JSON document (text/string)\n# form_json is a formio.js Form JSON document (text/string)\n>>\n>> builder = Builder(builder_json)\n>> form = Form(builder, form_json)\n\n##################\n# input components\n##################\n\n# textfield label\n>> print(form.input_components[\'firstname\'].label)\n\'First Name\'\n\n# textfield value\n>> print(form.input_components[\'firstname\'].value)\n\'Bob\'\n\n# datetime label\n>> print(form.input_components[\'birthday\'].label)\n\'Birthday\'\n\n# datetime value\n>> print(form.input_components[\'birthday\'].value)\ndatetime.date(2009 10 16)\n\n# datagrid (rows property)\n>> print(form.input_components[\'datagridMeasurements\'].rows)\n[\n  {\'measurementDatetime\': <datetimeComponent>, \'measurementFahrenheit\': <numberComponent>}, \n  {\'measurementDatetime\': <datetimeComponent>, \'measurementFahrenheit\': <numberComponent>}\n]\n\n>> for row in form.input_components[\'datagridMeasurements\'].rows:\n>>    dtime = row[\'measurementDatetime\']\n>>    fahrenheit = row[\'measurementFahrenheit\']\n>>    print(%s: %s, %s: %s\' % (dt.label, dt.value, fahrenheit.label, fahrenheit.value))\n\nDatetime: datetime.datetime(2021, 5, 8, 11, 39, 0, 296487), Fahrenheit: 122\nDatetime: datetime.datetime(2021, 5, 8, 11, 41, 5, 919943), Fahrenheit: 131\n\n# alternative example, by getattr\n>> print(form.data.firstname.label)\n\'First Name\'\n\n>> print(form.data.firstname.value)\n\'Bob\'\n\n#################\n# components path\n#################\n\n# datagrid input\n>> datagridMeasurements = builder.components[\'datagridMeasurements\']\n\n# Component builder_path_key property\n>> [\n>>     print(row.input_components[\'measurementDatetime\'].builder_path_key)\n>>     for row in datagridMeasurements.rows\n>> ]\n[\'pageMeasurements\', \'columnsExternal\', \'datagridMeasurements\', \'measurementDatetime\']\n\n# Component builder_path_labels property\n>> [\n>>     print(row.input_components[\'measurementDatetime\'].builder_path_labels)\n>>     for row in datagridMeasurements.rows\n>> ]\n[\'Page Measurements\', \'Columns External\', \'Data Grid Measurements\', \'Measurement Datetime\']\n\n# Component builder_input_path_key property\n>> [\n>>     print(row.input_components[\'measurementDatetime\'].builder_input_path_key)\n>>     for row in datagridMeasurements.rows\n>> ]\n[\'datagridMeasurements\', \'measurementDatetime\']\n\n# Component builder_input_path_labels property\n>> [\n>>     print(row.input_components[\'measurementDatetime\'].builder_input_path_labels)\n>>     for row in datagridMeasurements.rows\n>> ]\n[\'Data Grid Measurements\', \'Measurement Datetime\']\n\n#################################\n# components (layout, input etc.)\n#################################\n\n# columns\n>> print(form.components[\'addressColumns\'])\n<columnsComponent>\n\n>> print(form.components[\'addressColumns\'].rows)\n[ \n  {\'firstName\': <textfieldComponent>, \'lastName: <textfieldComponent>}, \n  {\'email\': <emailComponent>, \'companyName: <textfieldComponent>}\n]\n```\n\n## Unit tests\n\n**Note:**\n\nInternet access is recommended for running the `filecStorageUrlComponentTestCase`, because this also tests the URL Storage (type).\\\nIf no internet access, this test won\'t fail and a WARNING shall be logged regarding a ConnectionError.\n\n### Run all unittests\n\nFrom toplevel directory:\n\n```\npoetry install -E json_logic  # if you haven\'t already\npoetry run python -m unittest\n```\n\n### Run component unittests\n\nAll Components, from toplevel directory:\n\n```\npoetry run python -m unittest tests/test_component_*.py\n```\n\nNested components (complexity), from toplevel directory:\n\n```\npoetry run python -m unittest tests/test_nested_components.py\n```\n\n### Run specific component unittest\n\n```\npoetry run python -m unittest tests.test_component_day.dayComponentTestCase.test_get_form_dayMonthYear\n```\n',
     'author': 'Bob Leers',
     'author_email': 'bob@novacode.nl',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/novacode-nl/python-formio-data',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `formio-data-1.0.0/PKG-INFO` & `formio-data-1.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formio-data
-Version: 1.0.0
+Version: 1.0.1
 Summary: formio.js JSON-data API
 Home-page: https://github.com/novacode-nl/python-formio-data
 License: MIT
 Author: Bob Leers
 Author-email: bob@novacode.nl
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -171,24 +171,40 @@
 #################
 # components path
 #################
 
 # datagrid input
 >> datagridMeasurements = builder.components['datagridMeasurements']
 
->> [print(row.input_components['measurementDatetime'].builder_path_key) for row in datagridMeasurements.rows]
+# Component builder_path_key property
+>> [
+>>     print(row.input_components['measurementDatetime'].builder_path_key)
+>>     for row in datagridMeasurements.rows
+>> ]
 ['pageMeasurements', 'columnsExternal', 'datagridMeasurements', 'measurementDatetime']
 
->> [print(row.input_components['measurementDatetime'].builder_path_labels) for row in datagridMeasurements.rows]
+# Component builder_path_labels property
+>> [
+>>     print(row.input_components['measurementDatetime'].builder_path_labels)
+>>     for row in datagridMeasurements.rows
+>> ]
 ['Page Measurements', 'Columns External', 'Data Grid Measurements', 'Measurement Datetime']
 
->> [print(row.input_components['measurementDatetime'].builder_input_path_key) for row in datagridMeasurements.rows]
+# Component builder_input_path_key property
+>> [
+>>     print(row.input_components['measurementDatetime'].builder_input_path_key)
+>>     for row in datagridMeasurements.rows
+>> ]
 ['datagridMeasurements', 'measurementDatetime']
 
->> [print(row.input_components['measurementDatetime'].builder_input_path_labels) for row in datagridMeasurements.rows]
+# Component builder_input_path_labels property
+>> [
+>>     print(row.input_components['measurementDatetime'].builder_input_path_labels)
+>>     for row in datagridMeasurements.rows
+>> ]
 ['Data Grid Measurements', 'Measurement Datetime']
 
 #################################
 # components (layout, input etc.)
 #################################
 
 # columns
```

