# Comparing `tmp/pytest_molecule_JC-2.0.0.post1.tar.gz` & `tmp/pytest_molecule_JC-2.0.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/fazi/others/pytest-molecule/dist/tmpxy263bvl/pytest_molecule_JC-2.0.0.post1.tar", last modified: Tue Jul 18 12:34:00 2023, max compression
+gzip compressed data, was "/home/fazi/others/pytest-molecule/dist/tmpwdkzcur_/pytest_molecule_JC-2.0.0.post2.tar", last modified: Tue Jul 18 13:25:04 2023, max compression
```

## Comparing `pytest_molecule_JC-2.0.0.post1.tar` & `pytest_molecule_JC-2.0.0.post2.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 12:34:00.000000 pytest_molecule_JC-2.0.0.post1/
-drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 12:34:00.000000 pytest_molecule_JC-2.0.0.post1/.github/
-drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 12:34:00.000000 pytest_molecule_JC-2.0.0.post1/.github/workflows/
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)      244 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post1/.github/workflows/ack.yml
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)      248 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post1/.github/workflows/push.yml
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     1182 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post1/.github/workflows/release.yml
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     2069 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post1/.github/workflows/tox.yml
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)       28 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post1/.github/CODEOWNERS
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)       64 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post1/.github/FUNDING.yml
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)      573 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post1/.github/dependabot.yml
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     1211 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post1/.github/labels.yml
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)       73 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post1/.github/release-drafter.yml
-drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 12:34:00.000000 pytest_molecule_JC-2.0.0.post1/src/
-drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 12:34:00.000000 pytest_molecule_JC-2.0.0.post1/src/pytest_molecule/
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)    11282 2023-07-18 12:06:55.000000 pytest_molecule_JC-2.0.0.post1/src/pytest_molecule/__init__.py
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post1/src/pytest_molecule/py.typed
-drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 12:34:00.000000 pytest_molecule_JC-2.0.0.post1/src/pytest_molecule_JC.egg-info/
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     5358 2023-07-18 12:34:00.000000 pytest_molecule_JC-2.0.0.post1/src/pytest_molecule_JC.egg-info/PKG-INFO
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     1782 2023-07-18 12:34:00.000000 pytest_molecule_JC-2.0.0.post1/src/pytest_molecule_JC.egg-info/SOURCES.txt
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)        1 2023-07-18 12:34:00.000000 pytest_molecule_JC-2.0.0.post1/src/pytest_molecule_JC.egg-info/dependency_links.txt
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)       39 2023-07-18 12:34:00.000000 pytest_molecule_JC-2.0.0.post1/src/pytest_molecule_JC.egg-info/entry_points.txt
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)        1 2023-07-18 12:34:00.000000 pytest_molecule_JC-2.0.0.post1/src/pytest_molecule_JC.egg-info/not-zip-safe
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)      156 2023-07-18 12:34:00.000000 pytest_molecule_JC-2.0.0.post1/src/pytest_molecule_JC.egg-info/requires.txt
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)       16 2023-07-18 12:34:00.000000 pytest_molecule_JC-2.0.0.post1/src/pytest_molecule_JC.egg-info/top_level.txt
-drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 12:34:00.000000 pytest_molecule_JC-2.0.0.post1/tests/
-drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 12:34:00.000000 pytest_molecule_JC-2.0.0.post1/tests/roles/
-drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 12:34:00.000000 pytest_molecule_JC-2.0.0.post1/tests/roles/base_config/
-drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 12:34:00.000000 pytest_molecule_JC-2.0.0.post1/tests/roles/base_config/molecule/
-drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 12:34:00.000000 pytest_molecule_JC-2.0.0.post1/tests/roles/base_config/molecule/s1/
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)      125 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post1/tests/roles/base_config/molecule/s1/converge.yml
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)       62 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post1/tests/roles/base_config/molecule/s1/molecule.yml
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)      211 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post1/tests/roles/base_config/molecule/s1/prepare.yml
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)       46 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post1/tests/roles/base_config/base.yml
-drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 12:34:00.000000 pytest_molecule_JC-2.0.0.post1/tests/roles/ensure-ansible/
-drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 12:34:00.000000 pytest_molecule_JC-2.0.0.post1/tests/roles/ensure-ansible/meta/
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)      467 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post1/tests/roles/ensure-ansible/meta/main.yml
-drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 12:34:00.000000 pytest_molecule_JC-2.0.0.post1/tests/roles/ensure-ansible/molecule/
-drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 12:34:00.000000 pytest_molecule_JC-2.0.0.post1/tests/roles/ensure-ansible/molecule/default/
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     1925 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post1/tests/roles/ensure-ansible/molecule/default/converge.yml
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     1744 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post1/tests/roles/ensure-ansible/molecule/default/molecule.yml
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)      263 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post1/tests/roles/ensure-ansible/molecule/Dockerfile.j2
-drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 12:34:00.000000 pytest_molecule_JC-2.0.0.post1/tests/roles/ensure-ansible/tasks/
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     1669 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post1/tests/roles/ensure-ansible/tasks/main.yml
-drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 12:34:00.000000 pytest_molecule_JC-2.0.0.post1/tests/roles/ensure-ansible/vars/
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)      213 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post1/tests/roles/ensure-ansible/vars/centos-7.yml
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)       50 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post1/tests/roles/ensure-ansible/vars/debian-10.yml
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)      213 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post1/tests/roles/ensure-ansible/vars/family-redhat.yml
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)      160 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post1/tests/roles/ensure-ansible/vars/redhat-8.yml
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)      137 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post1/tests/roles/ensure-ansible/vars/ubuntu.yml
-drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 12:34:00.000000 pytest_molecule_JC-2.0.0.post1/tests/roles/foo/
-drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 12:34:00.000000 pytest_molecule_JC-2.0.0.post1/tests/roles/foo/molecule/
-drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 12:34:00.000000 pytest_molecule_JC-2.0.0.post1/tests/roles/foo/molecule/default/
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)       84 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post1/tests/roles/foo/molecule/default/converge.yml
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)      147 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post1/tests/roles/foo/molecule/default/molecule.yml
-drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 12:34:00.000000 pytest_molecule_JC-2.0.0.post1/tests/roles/foo/molecule/disabled/
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)      149 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post1/tests/roles/foo/molecule/disabled/converge.yml
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)      167 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post1/tests/roles/foo/molecule/disabled/molecule.yml
-drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 12:34:00.000000 pytest_molecule_JC-2.0.0.post1/tests/roles/no_drivers/
-drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 12:34:00.000000 pytest_molecule_JC-2.0.0.post1/tests/roles/no_drivers/molecule/
-drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 12:34:00.000000 pytest_molecule_JC-2.0.0.post1/tests/roles/no_drivers/molecule/default/
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)       35 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post1/tests/roles/no_drivers/molecule/default/molecule.yml
-drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 12:34:00.000000 pytest_molecule_JC-2.0.0.post1/tests/roles/no_platforms/
-drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 12:34:00.000000 pytest_molecule_JC-2.0.0.post1/tests/roles/no_platforms/molecule/
-drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 12:34:00.000000 pytest_molecule_JC-2.0.0.post1/tests/roles/no_platforms/molecule/default/
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)       30 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post1/tests/roles/no_platforms/molecule/default/molecule.yml
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)       93 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post1/tests/conftest.py
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)       35 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post1/tests/hosts.ini
-drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 12:34:00.000000 pytest_molecule_JC-2.0.0.post1/tools/
--rwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)      122 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post1/tools/test-setup.sh
-drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 12:34:00.000000 pytest_molecule_JC-2.0.0.post1/zuul.d/
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)      806 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post1/zuul.d/layout.yaml
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)      248 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post1/.flake8
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     1222 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post1/.gitignore
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     2232 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post1/.pre-commit-config.yaml
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     1085 2023-07-18 12:06:55.000000 pytest_molecule_JC-2.0.0.post1/LICENSE
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)       97 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post1/MANIFEST.in
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     3814 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post1/README.rst
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)       80 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post1/ansible.cfg
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)      334 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post1/bindep.txt
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)       96 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post1/mypy.ini
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)      399 2023-07-18 12:33:38.000000 pytest_molecule_JC-2.0.0.post1/pyproject.toml
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)       37 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post1/pytest.ini
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     1906 2023-07-18 12:34:00.000000 pytest_molecule_JC-2.0.0.post1/setup.cfg
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)      241 2023-07-18 12:33:38.000000 pytest_molecule_JC-2.0.0.post1/setup.py
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     3176 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post1/tox.ini
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     5358 2023-07-18 12:34:00.000000 pytest_molecule_JC-2.0.0.post1/PKG-INFO
+drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 13:25:04.000000 pytest_molecule_JC-2.0.0.post2/
+drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 13:25:04.000000 pytest_molecule_JC-2.0.0.post2/.github/
+drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 13:25:04.000000 pytest_molecule_JC-2.0.0.post2/.github/workflows/
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)      244 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post2/.github/workflows/ack.yml
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)      248 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post2/.github/workflows/push.yml
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     1182 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post2/.github/workflows/release.yml
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     2069 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post2/.github/workflows/tox.yml
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)       28 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post2/.github/CODEOWNERS
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)       64 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post2/.github/FUNDING.yml
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)      573 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post2/.github/dependabot.yml
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     1211 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post2/.github/labels.yml
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)       73 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post2/.github/release-drafter.yml
+drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 13:25:04.000000 pytest_molecule_JC-2.0.0.post2/src/
+drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 13:25:04.000000 pytest_molecule_JC-2.0.0.post2/src/pytest_molecule/
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)    11418 2023-07-18 13:24:00.000000 pytest_molecule_JC-2.0.0.post2/src/pytest_molecule/__init__.py
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post2/src/pytest_molecule/py.typed
+drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 13:25:04.000000 pytest_molecule_JC-2.0.0.post2/src/pytest_molecule_JC.egg-info/
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     5358 2023-07-18 13:25:04.000000 pytest_molecule_JC-2.0.0.post2/src/pytest_molecule_JC.egg-info/PKG-INFO
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     1782 2023-07-18 13:25:04.000000 pytest_molecule_JC-2.0.0.post2/src/pytest_molecule_JC.egg-info/SOURCES.txt
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)        1 2023-07-18 13:25:04.000000 pytest_molecule_JC-2.0.0.post2/src/pytest_molecule_JC.egg-info/dependency_links.txt
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)       39 2023-07-18 13:25:04.000000 pytest_molecule_JC-2.0.0.post2/src/pytest_molecule_JC.egg-info/entry_points.txt
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)        1 2023-07-18 13:25:04.000000 pytest_molecule_JC-2.0.0.post2/src/pytest_molecule_JC.egg-info/not-zip-safe
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)      156 2023-07-18 13:25:04.000000 pytest_molecule_JC-2.0.0.post2/src/pytest_molecule_JC.egg-info/requires.txt
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)       16 2023-07-18 13:25:04.000000 pytest_molecule_JC-2.0.0.post2/src/pytest_molecule_JC.egg-info/top_level.txt
+drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 13:25:04.000000 pytest_molecule_JC-2.0.0.post2/tests/
+drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 13:25:04.000000 pytest_molecule_JC-2.0.0.post2/tests/roles/
+drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 13:25:04.000000 pytest_molecule_JC-2.0.0.post2/tests/roles/base_config/
+drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 13:25:04.000000 pytest_molecule_JC-2.0.0.post2/tests/roles/base_config/molecule/
+drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 13:25:04.000000 pytest_molecule_JC-2.0.0.post2/tests/roles/base_config/molecule/s1/
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)      125 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post2/tests/roles/base_config/molecule/s1/converge.yml
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)       62 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post2/tests/roles/base_config/molecule/s1/molecule.yml
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)      211 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post2/tests/roles/base_config/molecule/s1/prepare.yml
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)       46 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post2/tests/roles/base_config/base.yml
+drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 13:25:04.000000 pytest_molecule_JC-2.0.0.post2/tests/roles/ensure-ansible/
+drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 13:25:04.000000 pytest_molecule_JC-2.0.0.post2/tests/roles/ensure-ansible/meta/
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)      467 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post2/tests/roles/ensure-ansible/meta/main.yml
+drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 13:25:04.000000 pytest_molecule_JC-2.0.0.post2/tests/roles/ensure-ansible/molecule/
+drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 13:25:04.000000 pytest_molecule_JC-2.0.0.post2/tests/roles/ensure-ansible/molecule/default/
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     1925 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post2/tests/roles/ensure-ansible/molecule/default/converge.yml
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     1744 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post2/tests/roles/ensure-ansible/molecule/default/molecule.yml
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)      263 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post2/tests/roles/ensure-ansible/molecule/Dockerfile.j2
+drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 13:25:04.000000 pytest_molecule_JC-2.0.0.post2/tests/roles/ensure-ansible/tasks/
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     1669 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post2/tests/roles/ensure-ansible/tasks/main.yml
+drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 13:25:04.000000 pytest_molecule_JC-2.0.0.post2/tests/roles/ensure-ansible/vars/
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)      213 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post2/tests/roles/ensure-ansible/vars/centos-7.yml
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)       50 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post2/tests/roles/ensure-ansible/vars/debian-10.yml
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)      213 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post2/tests/roles/ensure-ansible/vars/family-redhat.yml
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)      160 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post2/tests/roles/ensure-ansible/vars/redhat-8.yml
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)      137 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post2/tests/roles/ensure-ansible/vars/ubuntu.yml
+drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 13:25:04.000000 pytest_molecule_JC-2.0.0.post2/tests/roles/foo/
+drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 13:25:04.000000 pytest_molecule_JC-2.0.0.post2/tests/roles/foo/molecule/
+drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 13:25:04.000000 pytest_molecule_JC-2.0.0.post2/tests/roles/foo/molecule/default/
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)       84 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post2/tests/roles/foo/molecule/default/converge.yml
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)      147 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post2/tests/roles/foo/molecule/default/molecule.yml
+drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 13:25:04.000000 pytest_molecule_JC-2.0.0.post2/tests/roles/foo/molecule/disabled/
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)      149 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post2/tests/roles/foo/molecule/disabled/converge.yml
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)      167 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post2/tests/roles/foo/molecule/disabled/molecule.yml
+drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 13:25:04.000000 pytest_molecule_JC-2.0.0.post2/tests/roles/no_drivers/
+drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 13:25:04.000000 pytest_molecule_JC-2.0.0.post2/tests/roles/no_drivers/molecule/
+drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 13:25:04.000000 pytest_molecule_JC-2.0.0.post2/tests/roles/no_drivers/molecule/default/
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)       35 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post2/tests/roles/no_drivers/molecule/default/molecule.yml
+drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 13:25:04.000000 pytest_molecule_JC-2.0.0.post2/tests/roles/no_platforms/
+drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 13:25:04.000000 pytest_molecule_JC-2.0.0.post2/tests/roles/no_platforms/molecule/
+drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 13:25:04.000000 pytest_molecule_JC-2.0.0.post2/tests/roles/no_platforms/molecule/default/
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)       30 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post2/tests/roles/no_platforms/molecule/default/molecule.yml
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)       93 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post2/tests/conftest.py
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)       35 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post2/tests/hosts.ini
+drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 13:25:04.000000 pytest_molecule_JC-2.0.0.post2/tools/
+-rwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)      122 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post2/tools/test-setup.sh
+drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-07-18 13:25:04.000000 pytest_molecule_JC-2.0.0.post2/zuul.d/
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)      806 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post2/zuul.d/layout.yaml
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)      248 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post2/.flake8
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     1222 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post2/.gitignore
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     2232 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post2/.pre-commit-config.yaml
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     1085 2023-07-18 13:24:00.000000 pytest_molecule_JC-2.0.0.post2/LICENSE
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)       97 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post2/MANIFEST.in
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     3814 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post2/README.rst
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)       80 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post2/ansible.cfg
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)      334 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post2/bindep.txt
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)       96 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post2/mypy.ini
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)      399 2023-07-18 13:24:00.000000 pytest_molecule_JC-2.0.0.post2/pyproject.toml
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)       37 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post2/pytest.ini
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     1906 2023-07-18 13:25:04.000000 pytest_molecule_JC-2.0.0.post2/setup.cfg
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)      241 2023-07-18 13:24:00.000000 pytest_molecule_JC-2.0.0.post2/setup.py
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     3176 2023-07-18 10:07:34.000000 pytest_molecule_JC-2.0.0.post2/tox.ini
+-rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     5358 2023-07-18 13:25:04.000000 pytest_molecule_JC-2.0.0.post2/PKG-INFO
```

### Comparing `pytest_molecule_JC-2.0.0.post1/.github/workflows/release.yml` & `pytest_molecule_JC-2.0.0.post2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pytest_molecule_JC-2.0.0.post1/.github/workflows/tox.yml` & `pytest_molecule_JC-2.0.0.post2/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `pytest_molecule_JC-2.0.0.post1/.github/dependabot.yml` & `pytest_molecule_JC-2.0.0.post2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `pytest_molecule_JC-2.0.0.post1/.github/labels.yml` & `pytest_molecule_JC-2.0.0.post2/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `pytest_molecule_JC-2.0.0.post1/src/pytest_molecule/__init__.py` & `pytest_molecule_JC-2.0.0.post2/src/pytest_molecule/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -277,15 +277,17 @@
                 pytest.fail("Error checking git diff. Error was:" + str(exc))
 
         cmd.extend((self.name, "-s", scenario))
         # We append the additional options to molecule call, allowing user to
         # control how molecule is called by pytest-molecule
         opts = os.environ.get("MOLECULE_OPTS")
         if opts:
-            cmd.extend(shlex.split(opts))
+            for opt in shlex.split(opts):
+                if not any(opt.startswith(x) for x in ["--include-scenarios", "--skip-scenarios"]):
+                    cmd.append(opt)
 
         print(f"running: {' '.join(quote(arg) for arg in cmd)} (from {cwd})")
         try:
             # Workaround for STDOUT/STDERR line ordering issue:
             # https://github.com/pytest-dev/pytest/issues/5449
 
             with subprocess.Popen(
```

### Comparing `pytest_molecule_JC-2.0.0.post1/src/pytest_molecule_JC.egg-info/PKG-INFO` & `pytest_molecule_JC-2.0.0.post2/src/pytest_molecule_JC.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-molecule-JC
-Version: 2.0.0.post1
+Version: 2.0.0.post2
 Summary: PyTest Molecule Plugin :: discover and run molecule tests
 Home-page: https://github.com/LegenJCdary/pytest-molecule
 Author: Jakub Wierzbowski
 Author-email: jakub.wierzbowski@aptiv.com
 Maintainer: Jakub Wierzbowski
 Maintainer-email: jakub.wierzbowski@aptiv.com
 License: MIT
```

### Comparing `pytest_molecule_JC-2.0.0.post1/src/pytest_molecule_JC.egg-info/SOURCES.txt` & `pytest_molecule_JC-2.0.0.post2/src/pytest_molecule_JC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest_molecule_JC-2.0.0.post1/tests/roles/ensure-ansible/molecule/default/converge.yml` & `pytest_molecule_JC-2.0.0.post2/tests/roles/ensure-ansible/molecule/default/converge.yml`

 * *Files identical despite different names*

### Comparing `pytest_molecule_JC-2.0.0.post1/tests/roles/ensure-ansible/molecule/default/molecule.yml` & `pytest_molecule_JC-2.0.0.post2/tests/roles/ensure-ansible/molecule/default/molecule.yml`

 * *Files identical despite different names*

### Comparing `pytest_molecule_JC-2.0.0.post1/tests/roles/ensure-ansible/tasks/main.yml` & `pytest_molecule_JC-2.0.0.post2/tests/roles/ensure-ansible/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `pytest_molecule_JC-2.0.0.post1/zuul.d/layout.yaml` & `pytest_molecule_JC-2.0.0.post2/zuul.d/layout.yaml`

 * *Files identical despite different names*

### Comparing `pytest_molecule_JC-2.0.0.post1/.gitignore` & `pytest_molecule_JC-2.0.0.post2/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest_molecule_JC-2.0.0.post1/.pre-commit-config.yaml` & `pytest_molecule_JC-2.0.0.post2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pytest_molecule_JC-2.0.0.post1/LICENSE` & `pytest_molecule_JC-2.0.0.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_molecule_JC-2.0.0.post1/README.rst` & `pytest_molecule_JC-2.0.0.post2/README.rst`

 * *Files identical despite different names*

### Comparing `pytest_molecule_JC-2.0.0.post1/setup.cfg` & `pytest_molecule_JC-2.0.0.post2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [aliases]
 dists = clean --all sdist bdist_wheel
 
 [metadata]
 name = pytest_molecule_JC
-version = 2.0.0-1
+version = 2.0.0-2
 url = https://github.com/LegenJCdary/pytest-molecule
 description = PyTest Molecule Plugin :: discover and run molecule tests
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Jakub Wierzbowski
 author_email = jakub.wierzbowski@aptiv.com
 maintainer = Jakub Wierzbowski
```

### Comparing `pytest_molecule_JC-2.0.0.post1/tox.ini` & `pytest_molecule_JC-2.0.0.post2/tox.ini`

 * *Files identical despite different names*

### Comparing `pytest_molecule_JC-2.0.0.post1/PKG-INFO` & `pytest_molecule_JC-2.0.0.post2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest_molecule_JC
-Version: 2.0.0.post1
+Version: 2.0.0.post2
 Summary: PyTest Molecule Plugin :: discover and run molecule tests
 Home-page: https://github.com/LegenJCdary/pytest-molecule
 Author: Jakub Wierzbowski
 Author-email: jakub.wierzbowski@aptiv.com
 Maintainer: Jakub Wierzbowski
 Maintainer-email: jakub.wierzbowski@aptiv.com
 License: MIT
```

