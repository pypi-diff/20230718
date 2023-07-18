# Comparing `tmp/experiment-config-0.2.tar.gz` & `tmp/experiment-config-0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/experiment-config-0.2.tar", last modified: Sun Apr 16 22:31:55 2023, max compression
+gzip compressed data, was "experiment-config-0.21.tar", last modified: Tue Jul 18 01:39:52 2023, max compression
```

## Comparing `experiment-config-0.2.tar` & `experiment-config-0.21.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-16 22:31:55.000000 experiment-config-0.2/
--rw-r--r--   0 ahalev     (502) staff       (20)     1073 2023-01-29 22:38:50.000000 experiment-config-0.2/LICENSE.txt
--rw-r--r--   0 ahalev     (502) staff       (20)     8624 2023-04-16 22:31:55.000000 experiment-config-0.2/PKG-INFO
--rw-r--r--   0 ahalev     (502) staff       (20)     8185 2023-03-08 21:19:36.000000 experiment-config-0.2/README.md
--rw-r--r--   0 ahalev     (502) staff       (20)       38 2023-04-16 22:31:55.000000 experiment-config-0.2/setup.cfg
--rw-r--r--   0 ahalev     (502) staff       (20)      929 2023-04-16 22:31:35.000000 experiment-config-0.2/setup.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-16 22:31:55.000000 experiment-config-0.2/src/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-16 22:31:55.000000 experiment-config-0.2/src/experiment_config.egg-info/
--rw-r--r--   0 ahalev     (502) staff       (20)     8624 2023-04-16 22:31:55.000000 experiment-config-0.2/src/experiment_config.egg-info/PKG-INFO
--rw-r--r--   0 ahalev     (502) staff       (20)      411 2023-04-16 22:31:55.000000 experiment-config-0.2/src/experiment_config.egg-info/SOURCES.txt
--rw-r--r--   0 ahalev     (502) staff       (20)        1 2023-04-16 22:31:55.000000 experiment-config-0.2/src/experiment_config.egg-info/dependency_links.txt
--rw-r--r--   0 ahalev     (502) staff       (20)       28 2023-04-16 22:31:55.000000 experiment-config-0.2/src/experiment_config.egg-info/requires.txt
--rw-r--r--   0 ahalev     (502) staff       (20)        7 2023-04-16 22:31:55.000000 experiment-config-0.2/src/experiment_config.egg-info/top_level.txt
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-16 22:31:55.000000 experiment-config-0.2/src/expfig/
--rw-r--r--   0 ahalev     (502) staff       (20)      126 2023-03-08 21:19:36.000000 experiment-config-0.2/src/expfig/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)     8087 2023-04-16 22:26:51.000000 experiment-config-0.2/src/expfig/fig.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-16 22:31:55.000000 experiment-config-0.2/src/expfig/logging/
--rw-r--r--   0 ahalev     (502) staff       (20)       76 2023-03-08 21:19:36.000000 experiment-config-0.2/src/expfig/logging/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)     1281 2023-03-08 21:19:36.000000 experiment-config-0.2/src/expfig/logging/log_dir.py
--rw-r--r--   0 ahalev     (502) staff       (20)      381 2023-03-08 21:19:36.000000 experiment-config-0.2/src/expfig/logging/logger.py
--rw-r--r--   0 ahalev     (502) staff       (20)     6505 2023-04-08 23:03:36.000000 experiment-config-0.2/src/expfig/namespacify.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-07-18 01:39:52.501080 experiment-config-0.21/
+-rw-r--r--   0 ahalev     (502) staff       (20)     1073 2023-01-29 22:38:50.000000 experiment-config-0.21/LICENSE.txt
+-rw-r--r--   0 ahalev     (502) staff       (20)     9190 2023-07-18 01:39:52.500814 experiment-config-0.21/PKG-INFO
+-rw-r--r--   0 ahalev     (502) staff       (20)     8789 2023-05-31 22:41:55.000000 experiment-config-0.21/README.md
+-rw-r--r--   0 ahalev     (502) staff       (20)       38 2023-07-18 01:39:52.501133 experiment-config-0.21/setup.cfg
+-rw-r--r--   0 ahalev     (502) staff       (20)      930 2023-07-18 01:20:43.000000 experiment-config-0.21/setup.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-07-18 01:39:52.497728 experiment-config-0.21/src/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-07-18 01:39:52.498987 experiment-config-0.21/src/experiment_config.egg-info/
+-rw-r--r--   0 ahalev     (502) staff       (20)     9190 2023-07-18 01:39:52.000000 experiment-config-0.21/src/experiment_config.egg-info/PKG-INFO
+-rw-r--r--   0 ahalev     (502) staff       (20)      411 2023-07-18 01:39:52.000000 experiment-config-0.21/src/experiment_config.egg-info/SOURCES.txt
+-rw-r--r--   0 ahalev     (502) staff       (20)        1 2023-07-18 01:39:52.000000 experiment-config-0.21/src/experiment_config.egg-info/dependency_links.txt
+-rw-r--r--   0 ahalev     (502) staff       (20)       28 2023-07-18 01:39:52.000000 experiment-config-0.21/src/experiment_config.egg-info/requires.txt
+-rw-r--r--   0 ahalev     (502) staff       (20)        7 2023-07-18 01:39:52.000000 experiment-config-0.21/src/experiment_config.egg-info/top_level.txt
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-07-18 01:39:52.499678 experiment-config-0.21/src/expfig/
+-rw-r--r--   0 ahalev     (502) staff       (20)      138 2023-05-31 22:41:55.000000 experiment-config-0.21/src/expfig/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     8349 2023-07-18 01:16:28.000000 experiment-config-0.21/src/expfig/fig.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-07-18 01:39:52.500576 experiment-config-0.21/src/expfig/logging/
+-rw-r--r--   0 ahalev     (502) staff       (20)       76 2023-07-16 23:55:34.000000 experiment-config-0.21/src/expfig/logging/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     1905 2023-07-17 20:30:35.000000 experiment-config-0.21/src/expfig/logging/log_dir.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     1018 2023-07-16 23:55:34.000000 experiment-config-0.21/src/expfig/logging/logger.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     6919 2023-07-18 01:15:42.000000 experiment-config-0.21/src/expfig/namespacify.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `experiment-config-0.2/LICENSE.txt` & `experiment-config-0.21/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `experiment-config-0.2/PKG-INFO` & `experiment-config-0.21/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: experiment-config
-Version: 0.2
-Summary: A yaml-based configuration for reproducible python experiments.
-Home-page: UNKNOWN
-Maintainer: Avishai Halev
-Maintainer-email: avishaihalev@gmail.com
-License: MIT License
-Project-URL: Source Code, https://github.com/ahalev/experiment-config
-Platform: UNKNOWN
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE.txt
-
 ## Installation
 
 Install with pip:
 
 ```shell script
 pip install experiment-config
 ```
@@ -264,14 +249,26 @@
 
 3. Values within a config file passed at the command line. If multiple config files are passed and the 
    key is contained in more than one of said files, the value from the *last* file will be used.
 
 4. Values within your default config.
 
 
+## Variations between different methods of setting parameters
+
+### 1. Type casting
+Values passed at the command line are casted to the type of the default value as defined by the yaml-load of the default
+value. For example, a default config containing `value: 1` will result in the expectation that `value` is an `int`. 
+This is not true with values passed in python code or in separate config files. 
+
+There are two exceptions to this: 
+
+1. Values where the default value is `None` parse command line arguments to string.
+
+2. The string `null` passed at the command line results in the value `None`. 
+
+
 ## Additional Examples
 
 An example of using `expfig.Config` to set hyperparameters for a machine learning problem
 is available in `examples/knn`. This example demonstrates a simple class to run a classification problem using `scikit-learn`'s
 [`KNeighborsClassifier`](https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.KNeighborsClassifier.html).
-
-
```

### Comparing `experiment-config-0.2/README.md` & `experiment-config-0.21/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: experiment-config
+Version: 0.21
+Summary: A yaml-based configuration for reproducible python experiments.
+Maintainer: Avishai Halev
+Maintainer-email: avishaihalev@gmail.com
+License: MIT License
+Project-URL: Source Code, https://github.com/ahalev/experiment-config
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE.txt
+
 ## Installation
 
 Install with pip:
 
 ```shell script
 pip install experiment-config
 ```
@@ -249,12 +262,26 @@
 
 3. Values within a config file passed at the command line. If multiple config files are passed and the 
    key is contained in more than one of said files, the value from the *last* file will be used.
 
 4. Values within your default config.
 
 
+## Variations between different methods of setting parameters
+
+### 1. Type casting
+Values passed at the command line are casted to the type of the default value as defined by the yaml-load of the default
+value. For example, a default config containing `value: 1` will result in the expectation that `value` is an `int`. 
+This is not true with values passed in python code or in separate config files. 
+
+There are two exceptions to this: 
+
+1. Values where the default value is `None` parse command line arguments to string.
+
+2. The string `null` passed at the command line results in the value `None`. 
+
+
 ## Additional Examples
 
 An example of using `expfig.Config` to set hyperparameters for a machine learning problem
 is available in `examples/knn`. This example demonstrates a simple class to run a classification problem using `scikit-learn`'s
 [`KNeighborsClassifier`](https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.KNeighborsClassifier.html).
```

### Comparing `experiment-config-0.2/setup.py` & `experiment-config-0.21/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 from setuptools import setup, find_packages
 
 DESCRIPTION = 'A yaml-based configuration for reproducible python experiments.'
-VERSION = '0.2'
+VERSION = '0.21'
 MAINTAINER = 'Avishai Halev'
 MAINTAINER_EMAIL = 'avishaihalev@gmail.com'
 LICENSE = 'MIT License'
 PROJECT_URLS = {
     'Source Code': 'https://github.com/ahalev/experiment-config'
 }
 EXTRAS = {
```

### Comparing `experiment-config-0.2/src/experiment_config.egg-info/PKG-INFO` & `experiment-config-0.21/src/experiment_config.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: experiment-config
-Version: 0.2
+Version: 0.21
 Summary: A yaml-based configuration for reproducible python experiments.
-Home-page: UNKNOWN
 Maintainer: Avishai Halev
 Maintainer-email: avishaihalev@gmail.com
 License: MIT License
 Project-URL: Source Code, https://github.com/ahalev/experiment-config
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 ## Installation
 
@@ -264,14 +262,26 @@
 
 3. Values within a config file passed at the command line. If multiple config files are passed and the 
    key is contained in more than one of said files, the value from the *last* file will be used.
 
 4. Values within your default config.
 
 
+## Variations between different methods of setting parameters
+
+### 1. Type casting
+Values passed at the command line are casted to the type of the default value as defined by the yaml-load of the default
+value. For example, a default config containing `value: 1` will result in the expectation that `value` is an `int`. 
+This is not true with values passed in python code or in separate config files. 
+
+There are two exceptions to this: 
+
+1. Values where the default value is `None` parse command line arguments to string.
+
+2. The string `null` passed at the command line results in the value `None`. 
+
+
 ## Additional Examples
 
 An example of using `expfig.Config` to set hyperparameters for a machine learning problem
 is available in `examples/knn`. This example demonstrates a simple class to run a classification problem using `scikit-learn`'s
 [`KNeighborsClassifier`](https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.KNeighborsClassifier.html).
-
-
```

### Comparing `experiment-config-0.2/src/expfig/fig.py` & `experiment-config-0.21/src/expfig/fig.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,30 +14,29 @@
 from .logging import get_logger
 
 
 DEFAULT_CONFIG_PATH = os.path.join(os.getcwd(), 'default_config.yaml')
 
 
 class Config(Namespacify):
-    def __init__(self, config=None, keys_for_name=(), name_prefix='', default=DEFAULT_CONFIG_PATH):
-        self.default_config = DefaultConfig(self._parse_default(config, default)).with_name_from_keys(*keys_for_name, prefix=name_prefix)
+    def __init__(self, config=None, default=DEFAULT_CONFIG_PATH):
+        self.default_config = DefaultConfig(self._parse_default(config, default))
 
         self.logger = get_logger()
         self.verbosity = 0
 
         super().__init__(self._parse_config())
 
         self.update_with_configs(config)
-        # if config is not None:
-        #     self._update_with_config(config)
-
-        self.with_name_from_keys(*keys_for_name, prefix=name_prefix)
         self.verbose(self.verbosity)
 
     def _parse_default(self, config, default):
+        if pd.api.types.is_dict_like(default):
+            return default
+
         candidates = [Path(default), (Path(sys.argv[0]).parent / default)]
 
         if config is not None and isinstance(config, (str, Path)):
             candidates.extend([Path(config), (Path(sys.argv[0]).parent / config)])
 
         for candidate in candidates:
             if candidate.exists():
@@ -51,25 +50,23 @@
     def _parse_config(self):
         # First we parse any --config arguments and load those
         # Then we can override them with any other passed values.
         base_config = deepcopy(self.default_config)
         config_files, other_args = self._create_config_file_parser().parse_known_args()
 
         self.update_with_configs(config_files.config, base_config)
-        # for config_file in config_files.config:
-        #     self._update_with_config(config_file, updatee=base_config)
 
         parsed_args = self._create_parser(default=base_config).parse_known_args(other_args)
 
         if len(parsed_args[1]):
             bad_args = [x.replace("--", "") for x in parsed_args[1] if x.startswith("--")]
             valid_args = "\n\t\t".join(sorted(parsed_args[0].__dict__.keys()))
             warn(f'Unrecognized arguments {bad_args}.\n\tValid arguments:\n\t\t{valid_args}')
 
-        args_dict = parsed_args[0].__dict__
+        args_dict = {k: v if v != 'null' else None for k, v in parsed_args[0].__dict__.items()}
 
         args_dict = self._extract_verbosity(args_dict)
         restructured = restructure_arguments(args_dict)
 
         self._check_restructured(restructured, self.default_config)
         return restructured
 
@@ -148,28 +145,43 @@
                 args.update(self._get_arguments(key=new_key, d=v))
             else:
                 args[new_key] = self._collect_argument(v)
 
         return args
 
     def _collect_argument(self, default_val):
-        if not default_val and not isinstance(default_val, (float, int, bool)):
+        arg = {}
+
+        if pd.api.types.is_list_like(default_val):
+            arg['nargs'] = '+'
+            _type = self._get_list_like_type(default_val)
+
+        elif not default_val and not isinstance(default_val, (float, int, bool)):
             _type = str
         else:
             _type = type(default_val)
 
-        arg = {
-            'default': default_val,
-            'type': _type,
-        }
-        if hasattr(default_val, '__len__') and not isinstance(default_val, str):
-            arg["nargs"] = '+'
+        arg.update({'default': default_val, 'type': _type})
 
         return arg
 
+    def _get_list_like_type(self, list_like):
+        _types = pd.Series([type(x) for x in list_like])
+
+        try:
+            _type = _types.unique().item()
+        except ValueError:
+            _type = str
+
+            if len(_types):
+                warn('Collecting argument with non-unique types in default value.'
+                     'Collected values will be str.')
+
+        return _type
+
     def serialize_to_dir(self, log_dir, fname='config.yaml', use_existing_dir=False, with_default=False):
         log_dir = super().serialize_to_dir(log_dir, fname=fname, use_existing_dir=use_existing_dir)
 
         if with_default:
             path = Path(fname)
 
             def fname_func(kind): return (path.parent / f'{path.stem}_{kind}').with_suffix(path.suffix)
@@ -194,16 +206,19 @@
                 self.logger.info('Custom trainer config (difference from default):')
                 xor.pprint(indent=1, log_func=self.logger.info)
             else:
                 self.logger.info('No difference from default.')
 
 
 class DefaultConfig(Namespacify):
-    def __init__(self, file_path):
-        super().__init__(_config_from_yaml(file_path))
+    def __init__(self, default):
+        if not pd.api.types.is_dict_like(default):
+            default = _config_from_yaml(default)
+
+        super().__init__(default)
 
 
 def _config_from_yaml(file_path):
     contents = Path(file_path).expanduser().open('r')
     loaded_contents = yaml.safe_load(contents)
 
     if not isinstance(loaded_contents, dict):
```

### Comparing `experiment-config-0.2/src/expfig/namespacify.py` & `experiment-config-0.21/src/expfig/namespacify.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,69 +1,36 @@
+import pandas as pd
 import yaml
 
 from collections import UserDict
 from logging import getLogger
 
 from .logging import make_sequential_log_dir
 
 yaml.SafeDumper.add_multi_representer(UserDict, yaml.SafeDumper.represent_dict)
 logger = getLogger(__name__)
 
 
 class Namespacify(UserDict):
-    def __init__(self, in_dict, name=''):
-        self.name = name
-
+    def __init__(self, in_dict):
         in_dict = in_dict.copy()
-
         for key in in_dict.keys():
-            if key == 'name':
-                raise NameError(f"Cannot use key 'name'.")
             if isinstance(in_dict[key], dict):
-                in_dict[key] = Namespacify(in_dict[key], name=key)
+                in_dict[key] = Namespacify(in_dict[key])
 
         super().__init__(in_dict)
 
-    def with_name_from_keys(self, *keys, prefix='', suffix='', uppercase=True):
-        if not keys:
-            obj = ''
-        else:
-            obj = self
-            for j, key in enumerate(keys):
-                try:
-                    obj = obj[key]
-                except (KeyError, TypeError):
-                    raise KeyError(f'Nested value {"->".join(keys[:j])} does not exist.')
-
-            if isinstance(obj, (dict, UserDict)):
-                raise KeyError(f'Nested value {"->".join(keys)} is dict-like, should be str, int, etc.')
-
-            if uppercase:
-                obj = obj.upper()
-
-        self.name = f'{prefix}{obj}{suffix}'
-
-        return self
-
     def update(self, *args, **kwargs):
         return nested_dict_update(self, *args, nest_namespacify=True, **kwargs)
 
     def pprint(self, indent=0, log_func=None, _recur=False):
         log_block = ''
-        name = self.name if self.name else 'config'
-
-        log_block += "{}{}:".format(' ' * indent, name)
-
-        indent += 4
-
         for k, v in self.items():
-            if k == "name":
-                continue
             if isinstance(v, Namespacify):
-                log_block += f'\n{v.pprint(indent, _recur=True)}'
+                log_block += f'\n{v.pprint(indent+4, _recur=True)}'
             else:
                 log_block+= f'\n{" " * indent}{k}: {v}'
 
         if not _recur:
             if log_func is None:
                 print(log_block)
             else:
@@ -71,29 +38,56 @@
 
         return log_block
 
     def to_dict(self):
         return {k: v.to_dict() if isinstance(v, Namespacify) else (v.copy() if hasattr(v, 'copy') else v)
                 for k, v in self.items()}
 
+    def to_series(self):
+        series = pd.json_normalize(self.to_dict()).squeeze()
+        series.index = pd.MultiIndex.from_tuples([x.split('.') for x in series.index])
+        return series
+
     def intersection(self, other):
         intersection = {}
 
         for k, v in self.items():
             if k in other:
                 if other[k] == v:
                     intersection[k] = v
                 elif isinstance(v, Namespacify) and isinstance(other[k], Namespacify):
                     subint = v.intersection(other[k])
                     if subint:
                         intersection[k] = subint
 
-        return Namespacify(intersection, name=self.name if self.name == other.name else '')
+        return Namespacify(intersection)
 
     def symmetric_difference(self, other):
+        """
+        Get all values that differ in ``self`` or ``other``.
+
+        Returns the value in ``self`` if it exists and differs from ``other``. Otherwise returns the value in ``other``.
+
+        If ``self['a'] = 1`` and ``other['a'] = 2``, ``self.symmetric_difference(other)['a'] = 1``.
+        If ``self['a'] = 1`` and ``'a' not in other``, `self.symmetric_difference(other)['a'] = 1``.
+        If ``'a' not in self`` and ``other['a'] = 2``, `self.symmetric_difference(other)['a'] = 2``.
+
+
+        Parameters
+        ----------
+        other : dict-like
+            Object to compare against
+
+        Returns
+        -------
+        difference : :class:`.Namespacify`
+            Difference between ``self`` and ``other``.
+
+        """
+
         diff = {}
 
         keys = {*self.keys(), *other.keys()}
         for k in keys:
             if k not in self:
                 diff[k] = other[k]
                 continue
@@ -104,28 +98,45 @@
 
             elif self[k] != other[k]:
                 if isinstance(self[k], Namespacify):
                     diff[k] = self[k].__xor__(other[k])
                 else:
                     diff[k] = self[k]
 
-        return Namespacify(diff, name=self.name)
+        return Namespacify(diff)
 
     def difference(self, other):
+        """
+        Get all values that are in ``self`` that are NOT (or are different) in ``other``.
+
+        If ``self['a'] = 1`` and ``other['a'] = 2``, ``self.difference(other)['a'] = 1``.
+        If ``a not in self`` and ``other['a'] = 2``, ``self.difference(other)['a']`` returns a ``KeyError``.
+
+        Parameters
+        ----------
+        other : dict-like
+            Object to compare against
+
+        Returns
+        -------
+        difference : :class:`.Namespacify`
+            Difference between ``self`` and ``other``.
+
+        """
         diff = {}
         for k, v in self.items():
             if k not in other:
                 diff[k] = v
             elif v != other[k]:
                 if isinstance(v, Namespacify):
                     diff[k] = v.difference(other[k])
                 else:
                     diff[k] = v
 
-        return Namespacify(diff, name=self.name)
+        return Namespacify(diff)
 
     def serialize(self, stream=None):
         return yaml.safe_dump(self, stream=stream)
 
     def serialize_to_dir(self, log_dir, fname='namespacify.yaml', use_existing_dir=False):
         log_dir = make_sequential_log_dir(log_dir, use_existing_dir=use_existing_dir)
         log_file = f'{log_dir}/{fname}'
@@ -185,15 +196,15 @@
     def __and__(self, other):
         return self.intersection(other)
 
     def __sub__(self, other):
         return self.difference(other)
 
     def __deepcopy__(self, memo=None):
-        return Namespacify(self.to_dict(), self.name)
+        return Namespacify(self.to_dict())
 
 
 def nested_dict_update(nested_dict, *args, nest_namespacify=False, **kwargs):
     if args:
         if len(args) != 1 or not isinstance(args[0], (dict, UserDict)):
             raise TypeError('Invalid arguments')
         elif kwargs:
@@ -206,12 +217,12 @@
     for k, v in d.items():
         if isinstance(v, (dict, UserDict)):
             if k in nested_dict:
                 nested_dict_update(
                     nested_dict[k], v, nest_namespacify=(nest_namespacify or isinstance(nested_dict[k], Namespacify))
                 )
             else:
-                nested_dict[k] = Namespacify(v, name=k) if nest_namespacify else v
+                nested_dict[k] = Namespacify(v) if nest_namespacify else v
         else:
             nested_dict[k] = v
 
     return nested_dict
```

