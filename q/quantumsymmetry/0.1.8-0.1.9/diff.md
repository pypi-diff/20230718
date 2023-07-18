# Comparing `tmp/quantumsymmetry-0.1.8.tar.gz` & `tmp/quantumsymmetry-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantumsymmetry-0.1.8.tar", max compression
+gzip compressed data, was "quantumsymmetry-0.1.9.tar", max compression
```

## Comparing `quantumsymmetry-0.1.8.tar` & `quantumsymmetry-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rwxr-xr-x   0        0        0    35095 2022-03-11 16:25:53.167876 quantumsymmetry-0.1.8/LICENSE
--rw-r--r--   0        0        0      694 2022-03-11 16:25:53.178472 quantumsymmetry-0.1.8/README.md
--rw-r--r--   0        0        0     1078 2022-03-13 14:28:04.492070 quantumsymmetry-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       37 2022-03-11 18:05:39.765293 quantumsymmetry-0.1.8/src/quantumsymmetry/__init__.py
--rw-r--r--   0        0        0    40821 2022-03-13 14:27:43.881345 quantumsymmetry-0.1.8/src/quantumsymmetry/core.py
--rw-r--r--   0        0        0     1437 2022-03-13 14:28:58.701066 quantumsymmetry-0.1.8/setup.py
--rw-r--r--   0        0        0     1366 2022-03-13 14:28:58.701357 quantumsymmetry-0.1.8/PKG-INFO
+-rwxr-xr-x   0        0        0    35095 2022-03-11 16:25:53.167876 quantumsymmetry-0.1.9/LICENSE
+-rw-r--r--   0        0        0      694 2022-03-11 16:25:53.178472 quantumsymmetry-0.1.9/README.md
+-rw-r--r--   0        0        0     1078 2022-03-13 14:35:08.074806 quantumsymmetry-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       37 2022-03-11 18:05:39.765293 quantumsymmetry-0.1.9/src/quantumsymmetry/__init__.py
+-rw-r--r--   0        0        0    40875 2022-03-13 14:35:10.530222 quantumsymmetry-0.1.9/src/quantumsymmetry/core.py
+-rw-r--r--   0        0        0     1437 2022-03-13 14:35:18.101537 quantumsymmetry-0.1.9/setup.py
+-rw-r--r--   0        0        0     1366 2022-03-13 14:35:18.101838 quantumsymmetry-0.1.9/PKG-INFO
```

### Comparing `quantumsymmetry-0.1.8/LICENSE` & `quantumsymmetry-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `quantumsymmetry-0.1.8/README.md` & `quantumsymmetry-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `quantumsymmetry-0.1.8/pyproject.toml` & `quantumsymmetry-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quantumsymmetry"
-version = "0.1.8"
+version = "0.1.9"
 description = "Quantum computing research package"
 authors = ["Dario Picozzi"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `quantumsymmetry-0.1.8/src/quantumsymmetry/core.py` & `quantumsymmetry-0.1.9/src/quantumsymmetry/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -712,17 +712,20 @@
     mol.atom = atom
     mol.symmetry = True
     mol.basis = basis
     mol.charge = charge
     mol.spin = spin
     mol.verbose = 0
     mol.build()
-    if mol.groupname == 'Dooh' or mol.groupname == 'Coov' or mol.groupname == 'SO3':
+    if mol.groupname == 'Dooh' or mol.groupname == 'SO3':
         mol.symmetry = 'D2h'
         mol.build()
+    if mol.groupname == 'Coov':
+        mol.symmetry = 'C2v'
+        mol.build()
     mf = scf.RHF(mol)
     mf.kernel()
     label_orb_symm = symm.label_orb_symm(mol, mol.irrep_name, mol.symm_orb, mf.mo_coeff)
     character_table, conj_labels, irrep_labels, conj_descriptions = get_character_table(mol.groupname)
     molecule_name = get_molecule_name(mol)
     symmetry_generator_labels, symmetry_generators_strings, target_qubits, symmetry_generators, signs, descriptions = find_symmetry_generators(mol, mf, irrep)
     tableau, tableau_signs = make_clifford_tableau(symmetry_generators, signs, target_qubits)
```

### Comparing `quantumsymmetry-0.1.8/setup.py` & `quantumsymmetry-0.1.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['ipython', 'numpy', 'openfermion', 'pyscf', 'qiskit', 'tabulate']
 
 setup_kwargs = {
     'name': 'quantumsymmetry',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Quantum computing research package',
     'long_description': '# quantumsymmetry\n\nQuantum computing research package\n\n## Installation\n\n```bash\n$ pip install quantumsymmetry\n```\n\n## Usage\n\n- TODO\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.\n\n## License\n\n`quantumsymmetry` was created by Dario Picozzi. It is licensed under the terms of the GNU General Public License v3.0 license.\n\n## Credits\n\n`quantumsymmetry` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n',
     'author': 'Dario Picozzi',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `quantumsymmetry-0.1.8/PKG-INFO` & `quantumsymmetry-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantumsymmetry
-Version: 0.1.8
+Version: 0.1.9
 Summary: Quantum computing research package
 License: GNU General Public License v3.0
 Author: Dario Picozzi
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

