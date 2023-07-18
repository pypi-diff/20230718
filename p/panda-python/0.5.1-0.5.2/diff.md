# Comparing `tmp/panda-python-0.5.1.tar.gz` & `tmp/panda-python-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panda-python-0.5.1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "panda-python-0.5.2.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `panda-python-0.5.1.tar` & `panda-python-0.5.2.tar`

### file list

```diff
@@ -1,73 +1,75 @@
--rw-r--r--   0        0        0     3097 2022-11-09 12:37:21.000000 panda-python-0.5.1/.github/workflows/build.yml
--rw-r--r--   0        0        0       18 2022-11-09 12:37:21.000000 panda-python-0.5.1/.gitignore
--rw-r--r--   0        0        0    19334 2022-11-09 12:37:21.000000 panda-python-0.5.1/.pylintrc
--rw-r--r--   0        0        0      168 2022-11-09 12:37:21.000000 panda-python-0.5.1/.readthedocs.yml
--rw-r--r--   0        0        0      482 2022-11-09 12:37:21.000000 panda-python-0.5.1/.vscode/c_cpp_properties.json
--rwxr-xr-x   0        0        0      481 2022-11-09 12:37:21.000000 panda-python-0.5.1/.vscode/generate_docs_api.sh
--rw-r--r--   0        0        0     2124 2022-11-09 12:37:21.000000 panda-python-0.5.1/.vscode/settings.json
--rw-r--r--   0        0        0      794 2022-11-09 12:37:21.000000 panda-python-0.5.1/.vscode/tasks.json
--rw-r--r--   0        0        0     1591 2022-11-09 12:37:21.000000 panda-python-0.5.1/CMakeLists.txt
--rw-r--r--   0        0        0    11357 2022-11-09 12:37:21.000000 panda-python-0.5.1/LICENSE
--rw-r--r--   0        0        0      881 2022-11-09 12:37:21.000000 panda-python-0.5.1/README.md
--rwxr-xr-x   0        0        0     1214 2022-11-09 12:37:21.000000 panda-python-0.5.1/bin/before_install.sh
--rwxr-xr-x   0        0        0     1376 2022-11-09 12:37:21.000000 panda-python-0.5.1/bin/build_all.sh
--rw-r--r--   0        0        0      634 2022-11-09 12:37:21.000000 panda-python-0.5.1/docs/Makefile
--rw-r--r--   0        0        0     1376 2022-11-09 12:37:21.000000 panda-python-0.5.1/docs/conf.py
--rw-r--r--   0        0        0      451 2022-11-09 12:37:21.000000 panda-python-0.5.1/docs/index.rst
--rw-r--r--   0        0        0      800 2022-11-09 12:37:21.000000 panda-python-0.5.1/docs/make.bat
--rw-r--r--   0        0        0      126 2022-11-09 12:37:21.000000 panda-python-0.5.1/docs/panda_py.cli.rst
--rw-r--r--   0        0        0      144 2022-11-09 12:37:21.000000 panda-python-0.5.1/docs/panda_py.constants.rst
--rw-r--r--   0        0        0      150 2022-11-09 12:37:21.000000 panda-python-0.5.1/docs/panda_py.controllers.rst
--rw-r--r--   0        0        0      144 2022-11-09 12:37:21.000000 panda-python-0.5.1/docs/panda_py.libfranka.rst
--rw-r--r--   0        0        0      135 2022-11-09 12:37:21.000000 panda-python-0.5.1/docs/panda_py.motion.rst
--rw-r--r--   0        0        0      273 2022-11-09 12:37:21.000000 panda-python-0.5.1/docs/panda_py.rst
--rw-r--r--   0        0        0       37 2022-11-09 12:37:21.000000 panda-python-0.5.1/docs/requirements.txt
--rw-r--r--   0        0        0      633 2022-11-09 12:37:21.000000 panda-python-0.5.1/examples/cartesian_impedance.py
--rw-r--r--   0        0        0     2531 2022-11-09 12:37:21.000000 panda-python-0.5.1/examples/communication_test.py
--rw-r--r--   0        0        0     2340 2022-11-09 12:37:21.000000 panda-python-0.5.1/examples/mmc.py
--rw-r--r--   0        0        0     5154 2022-11-09 12:37:21.000000 panda-python-0.5.1/examples/notebooks/benchmark.ipynb
--rw-r--r--   0        0        0    31180 2022-11-09 12:37:21.000000 panda-python-0.5.1/examples/notebooks/motion.ipynb
--rw-r--r--   0        0        0    38752 2022-11-09 12:37:21.000000 panda-python-0.5.1/examples/notebooks/paper.ipynb
--rw-r--r--   0        0        0     2076 2022-11-09 12:37:21.000000 panda-python-0.5.1/include/constants.h
--rw-r--r--   0        0        0     1136 2022-11-09 12:37:21.000000 panda-python-0.5.1/include/controllers/applied_force.h
--rw-r--r--   0        0        0     1091 2022-11-09 12:37:21.000000 panda-python-0.5.1/include/controllers/applied_torque.h
--rw-r--r--   0        0        0     2063 2022-11-09 12:37:21.000000 panda-python-0.5.1/include/controllers/cartesian_impedance.h
--rw-r--r--   0        0        0      673 2022-11-09 12:37:21.000000 panda-python-0.5.1/include/controllers/controller.h
--rw-r--r--   0        0        0     1683 2022-11-09 12:37:21.000000 panda-python-0.5.1/include/controllers/force.h
--rw-r--r--   0        0        0     1019 2022-11-09 12:37:21.000000 panda-python-0.5.1/include/controllers/integrated_velocity.h
--rw-r--r--   0        0        0     1337 2022-11-09 12:37:21.000000 panda-python-0.5.1/include/controllers/joint_limits/virtual_wall.h
--rw-r--r--   0        0        0     1381 2022-11-09 12:37:21.000000 panda-python-0.5.1/include/controllers/joint_limits/virtual_wall_controller.h
--rw-r--r--   0        0        0     1335 2022-11-09 12:37:21.000000 panda-python-0.5.1/include/controllers/joint_position.h
--rw-r--r--   0        0        0      778 2022-11-09 12:37:21.000000 panda-python-0.5.1/include/controllers/trajectory.h
--rw-r--r--   0        0        0    16534 2022-11-09 12:37:21.000000 panda-python-0.5.1/include/kinematics/fk.h
--rw-r--r--   0        0        0    14073 2022-11-09 12:37:21.000000 panda-python-0.5.1/include/kinematics/ik.h
--rw-r--r--   0        0        0     3949 2022-11-09 12:37:21.000000 panda-python-0.5.1/include/motion/generators.h
--rw-r--r--   0        0        0     3473 2022-11-09 12:37:21.000000 panda-python-0.5.1/include/motion/time_optimal/path.h
--rw-r--r--   0        0        0     5278 2022-11-09 12:37:21.000000 panda-python-0.5.1/include/motion/time_optimal/trajectory.h
--rw-r--r--   0        0        0     5819 2022-11-09 12:37:21.000000 panda-python-0.5.1/include/panda.h
--rw-r--r--   0        0        0     3864 2022-11-09 12:37:21.000000 panda-python-0.5.1/include/utils.h
--rw-r--r--   0        0        0    51837 2022-11-09 12:37:21.000000 panda-python-0.5.1/logo.jpg
--rw-r--r--   0        0        0     1672 2022-11-09 12:37:21.000000 panda-python-0.5.1/pyproject.toml
--rw-r--r--   0        0        0    21367 2022-11-09 12:37:21.000000 panda-python-0.5.1/src/_core.cpp
--rw-r--r--   0        0        0     2284 2022-11-09 12:37:21.000000 panda-python-0.5.1/src/controllers/applied_force.cpp
--rw-r--r--   0        0        0     2080 2022-11-09 12:37:21.000000 panda-python-0.5.1/src/controllers/applied_torque.cpp
--rw-r--r--   0        0        0     6444 2022-11-09 12:37:21.000000 panda-python-0.5.1/src/controllers/cartesian_impedance.cpp
--rw-r--r--   0        0        0     4628 2022-11-09 12:37:21.000000 panda-python-0.5.1/src/controllers/force.cpp
--rw-r--r--   0        0        0     2287 2022-11-09 12:37:21.000000 panda-python-0.5.1/src/controllers/integrated_velocity.cpp
--rw-r--r--   0        0        0     5337 2022-11-09 12:37:21.000000 panda-python-0.5.1/src/controllers/joint_limits/virtual_wall.cpp
--rw-r--r--   0        0        0     3069 2022-11-09 12:37:21.000000 panda-python-0.5.1/src/controllers/joint_position.cpp
--rw-r--r--   0        0        0     1240 2022-11-09 12:37:21.000000 panda-python-0.5.1/src/controllers/trajectory.cpp
--rw-r--r--   0        0        0    25036 2022-11-09 12:37:21.000000 panda-python-0.5.1/src/libfranka.cpp
--rw-r--r--   0        0        0     6824 2022-11-09 12:37:21.000000 panda-python-0.5.1/src/motion/generators.cpp
--rw-r--r--   0        0        0     9987 2022-11-09 12:37:21.000000 panda-python-0.5.1/src/motion/time_optimal/path.cpp
--rw-r--r--   0        0        0    23965 2022-11-09 12:37:21.000000 panda-python-0.5.1/src/motion/time_optimal/trajectory.cpp
--rw-r--r--   0        0        0    14329 2022-11-09 12:37:21.000000 panda-python-0.5.1/src/panda.cpp
--rw-r--r--   0        0        0    10245 2022-11-09 12:37:21.000000 panda-python-0.5.1/src/panda_py/__init__.py
--rw-r--r--   0        0        0     5211 2022-11-09 12:37:21.000000 panda-python-0.5.1/src/panda_py/__init__.pyi
--rw-r--r--   0        0        0    17071 2022-11-09 12:37:21.000000 panda-python-0.5.1/src/panda_py/_core/__init__.pyi
--rw-r--r--   0        0        0     2611 2022-11-09 12:37:21.000000 panda-python-0.5.1/src/panda_py/cli.py
--rw-r--r--   0        0        0      595 2022-11-09 12:37:21.000000 panda-python-0.5.1/src/panda_py/constants.py
--rw-r--r--   0        0        0      582 2022-11-09 12:37:21.000000 panda-python-0.5.1/src/panda_py/controllers.py
--rw-r--r--   0        0        0    34215 2022-11-09 12:37:21.000000 panda-python-0.5.1/src/panda_py/libfranka/__init__.pyi
--rw-r--r--   0        0        0      293 2022-11-09 12:37:21.000000 panda-python-0.5.1/src/panda_py/motion.py
--rw-r--r--   0        0        0    14908 2022-11-09 12:37:21.000000 panda-python-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      760 2022-11-09 12:37:21.000000 panda-python-0.5.2/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     3129 2022-11-09 12:37:21.000000 panda-python-0.5.2/.github/workflows/release.yml
+-rw-r--r--   0        0        0      293 2022-11-09 12:37:21.000000 panda-python-0.5.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0      392 2022-11-09 12:37:21.000000 panda-python-0.5.2/.github/workflows/test_all.yml
+-rw-r--r--   0        0        0       18 2022-11-09 12:37:21.000000 panda-python-0.5.2/.gitignore
+-rw-r--r--   0        0        0    19334 2022-11-09 12:37:21.000000 panda-python-0.5.2/.pylintrc
+-rw-r--r--   0        0        0      482 2022-11-09 12:37:21.000000 panda-python-0.5.2/.vscode/c_cpp_properties.json
+-rwxr-xr-x   0        0        0      481 2022-11-09 12:37:21.000000 panda-python-0.5.2/.vscode/generate_docs_api.sh
+-rw-r--r--   0        0        0     2124 2022-11-09 12:37:21.000000 panda-python-0.5.2/.vscode/settings.json
+-rw-r--r--   0        0        0      794 2022-11-09 12:37:21.000000 panda-python-0.5.2/.vscode/tasks.json
+-rw-r--r--   0        0        0     1591 2022-11-09 12:37:21.000000 panda-python-0.5.2/CMakeLists.txt
+-rw-r--r--   0        0        0    11357 2022-11-09 12:37:21.000000 panda-python-0.5.2/LICENSE
+-rw-r--r--   0        0        0     2512 2022-11-09 12:37:21.000000 panda-python-0.5.2/README.md
+-rwxr-xr-x   0        0        0     1214 2022-11-09 12:37:21.000000 panda-python-0.5.2/bin/before_install_centos.sh
+-rwxr-xr-x   0        0        0      591 2022-11-09 12:37:21.000000 panda-python-0.5.2/bin/before_install_ubuntu.sh
+-rwxr-xr-x   0        0        0     1376 2022-11-09 12:37:21.000000 panda-python-0.5.2/bin/build_all.sh
+-rw-r--r--   0        0        0      634 2022-11-09 12:37:21.000000 panda-python-0.5.2/docs/Makefile
+-rw-r--r--   0        0        0     1376 2022-11-09 12:37:21.000000 panda-python-0.5.2/docs/conf.py
+-rw-r--r--   0        0        0      451 2022-11-09 12:37:21.000000 panda-python-0.5.2/docs/index.rst
+-rw-r--r--   0        0        0      800 2022-11-09 12:37:21.000000 panda-python-0.5.2/docs/make.bat
+-rw-r--r--   0        0        0      126 2022-11-09 12:37:21.000000 panda-python-0.5.2/docs/panda_py.cli.rst
+-rw-r--r--   0        0        0      144 2022-11-09 12:37:21.000000 panda-python-0.5.2/docs/panda_py.constants.rst
+-rw-r--r--   0        0        0      150 2022-11-09 12:37:21.000000 panda-python-0.5.2/docs/panda_py.controllers.rst
+-rw-r--r--   0        0        0      144 2022-11-09 12:37:21.000000 panda-python-0.5.2/docs/panda_py.libfranka.rst
+-rw-r--r--   0        0        0      135 2022-11-09 12:37:21.000000 panda-python-0.5.2/docs/panda_py.motion.rst
+-rw-r--r--   0        0        0      273 2022-11-09 12:37:21.000000 panda-python-0.5.2/docs/panda_py.rst
+-rw-r--r--   0        0        0      633 2022-11-09 12:37:21.000000 panda-python-0.5.2/examples/cartesian_impedance.py
+-rw-r--r--   0        0        0     2531 2022-11-09 12:37:21.000000 panda-python-0.5.2/examples/communication_test.py
+-rw-r--r--   0        0        0     2340 2022-11-09 12:37:21.000000 panda-python-0.5.2/examples/mmc.py
+-rw-r--r--   0        0        0     5154 2022-11-09 12:37:21.000000 panda-python-0.5.2/examples/notebooks/benchmark.ipynb
+-rw-r--r--   0        0        0    31180 2022-11-09 12:37:21.000000 panda-python-0.5.2/examples/notebooks/motion.ipynb
+-rw-r--r--   0        0        0    38752 2022-11-09 12:37:21.000000 panda-python-0.5.2/examples/notebooks/paper.ipynb
+-rw-r--r--   0        0        0     2076 2022-11-09 12:37:21.000000 panda-python-0.5.2/include/constants.h
+-rw-r--r--   0        0        0     1136 2022-11-09 12:37:21.000000 panda-python-0.5.2/include/controllers/applied_force.h
+-rw-r--r--   0        0        0     1091 2022-11-09 12:37:21.000000 panda-python-0.5.2/include/controllers/applied_torque.h
+-rw-r--r--   0        0        0     2063 2022-11-09 12:37:21.000000 panda-python-0.5.2/include/controllers/cartesian_impedance.h
+-rw-r--r--   0        0        0      673 2022-11-09 12:37:21.000000 panda-python-0.5.2/include/controllers/controller.h
+-rw-r--r--   0        0        0     1683 2022-11-09 12:37:21.000000 panda-python-0.5.2/include/controllers/force.h
+-rw-r--r--   0        0        0     1019 2022-11-09 12:37:21.000000 panda-python-0.5.2/include/controllers/integrated_velocity.h
+-rw-r--r--   0        0        0     1337 2022-11-09 12:37:21.000000 panda-python-0.5.2/include/controllers/joint_limits/virtual_wall.h
+-rw-r--r--   0        0        0     1381 2022-11-09 12:37:21.000000 panda-python-0.5.2/include/controllers/joint_limits/virtual_wall_controller.h
+-rw-r--r--   0        0        0     1335 2022-11-09 12:37:21.000000 panda-python-0.5.2/include/controllers/joint_position.h
+-rw-r--r--   0        0        0      778 2022-11-09 12:37:21.000000 panda-python-0.5.2/include/controllers/trajectory.h
+-rw-r--r--   0        0        0    16534 2022-11-09 12:37:21.000000 panda-python-0.5.2/include/kinematics/fk.h
+-rw-r--r--   0        0        0    14073 2022-11-09 12:37:21.000000 panda-python-0.5.2/include/kinematics/ik.h
+-rw-r--r--   0        0        0     3949 2022-11-09 12:37:21.000000 panda-python-0.5.2/include/motion/generators.h
+-rw-r--r--   0        0        0     3473 2022-11-09 12:37:21.000000 panda-python-0.5.2/include/motion/time_optimal/path.h
+-rw-r--r--   0        0        0     5278 2022-11-09 12:37:21.000000 panda-python-0.5.2/include/motion/time_optimal/trajectory.h
+-rw-r--r--   0        0        0     5819 2022-11-09 12:37:21.000000 panda-python-0.5.2/include/panda.h
+-rw-r--r--   0        0        0     3864 2022-11-09 12:37:21.000000 panda-python-0.5.2/include/utils.h
+-rw-r--r--   0        0        0    51837 2022-11-09 12:37:21.000000 panda-python-0.5.2/logo.jpg
+-rw-r--r--   0        0        0     1742 2022-11-09 12:37:21.000000 panda-python-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0    21367 2022-11-09 12:37:21.000000 panda-python-0.5.2/src/_core.cpp
+-rw-r--r--   0        0        0     2284 2022-11-09 12:37:21.000000 panda-python-0.5.2/src/controllers/applied_force.cpp
+-rw-r--r--   0        0        0     2080 2022-11-09 12:37:21.000000 panda-python-0.5.2/src/controllers/applied_torque.cpp
+-rw-r--r--   0        0        0     6444 2022-11-09 12:37:21.000000 panda-python-0.5.2/src/controllers/cartesian_impedance.cpp
+-rw-r--r--   0        0        0     4628 2022-11-09 12:37:21.000000 panda-python-0.5.2/src/controllers/force.cpp
+-rw-r--r--   0        0        0     2287 2022-11-09 12:37:21.000000 panda-python-0.5.2/src/controllers/integrated_velocity.cpp
+-rw-r--r--   0        0        0     5337 2022-11-09 12:37:21.000000 panda-python-0.5.2/src/controllers/joint_limits/virtual_wall.cpp
+-rw-r--r--   0        0        0     3069 2022-11-09 12:37:21.000000 panda-python-0.5.2/src/controllers/joint_position.cpp
+-rw-r--r--   0        0        0     1240 2022-11-09 12:37:21.000000 panda-python-0.5.2/src/controllers/trajectory.cpp
+-rw-r--r--   0        0        0    25036 2022-11-09 12:37:21.000000 panda-python-0.5.2/src/libfranka.cpp
+-rw-r--r--   0        0        0     6824 2022-11-09 12:37:21.000000 panda-python-0.5.2/src/motion/generators.cpp
+-rw-r--r--   0        0        0     9987 2022-11-09 12:37:21.000000 panda-python-0.5.2/src/motion/time_optimal/path.cpp
+-rw-r--r--   0        0        0    23965 2022-11-09 12:37:21.000000 panda-python-0.5.2/src/motion/time_optimal/trajectory.cpp
+-rw-r--r--   0        0        0    14329 2022-11-09 12:37:21.000000 panda-python-0.5.2/src/panda.cpp
+-rw-r--r--   0        0        0    10248 2022-11-09 12:37:21.000000 panda-python-0.5.2/src/panda_py/__init__.py
+-rw-r--r--   0        0        0     5211 2022-11-09 12:37:21.000000 panda-python-0.5.2/src/panda_py/__init__.pyi
+-rw-r--r--   0        0        0    17230 2022-11-09 12:37:21.000000 panda-python-0.5.2/src/panda_py/_core/__init__.pyi
+-rw-r--r--   0        0        0     2611 2022-11-09 12:37:21.000000 panda-python-0.5.2/src/panda_py/cli.py
+-rw-r--r--   0        0        0      595 2022-11-09 12:37:21.000000 panda-python-0.5.2/src/panda_py/constants.py
+-rw-r--r--   0        0        0      582 2022-11-09 12:37:21.000000 panda-python-0.5.2/src/panda_py/controllers.py
+-rw-r--r--   0        0        0    34215 2022-11-09 12:37:21.000000 panda-python-0.5.2/src/panda_py/libfranka/__init__.pyi
+-rw-r--r--   0        0        0      293 2022-11-09 12:37:21.000000 panda-python-0.5.2/src/panda_py/motion.py
+-rw-r--r--   0        0        0    16687 2022-11-09 12:37:21.000000 panda-python-0.5.2/PKG-INFO
```

### Comparing `panda-python-0.5.1/.github/workflows/build.yml` & `panda-python-0.5.2/.github/workflows/release.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,28 @@
-name: build
+name: Build and deploy all variants
 
 on:
-  push:
-    branches: [main]
-  pull_request:
-    branches: [main]
   release:
     types: [published]
 
 env:
-  VERSION: 0.5.1
+  VERSION: 0.5.2
 
 permissions: write-all
 
 jobs:
   build_wheels:
-    name: Build wheels on ubuntu-latest
+    name: Build all wheels with cibuildwheel
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v3
       - name: Install cibuildwheel
         run: python -m pip install cibuildwheel==2.12.0
-      - name: Build wheels
+      - name: Build all wheels
         run: ./bin/build_all.sh
       - uses: actions/upload-artifact@v3
         with:
           path: ./dist/*.whl
           name: dist
       - uses: actions/upload-artifact@v3
         with:
@@ -42,19 +38,32 @@
       - name: Build sdist
         run: pipx run build --sdist
       - uses: actions/upload-artifact@v3
         with:
           path: dist/*.tar.gz
           name: dist
 
-  upload:
-    name: "Upload wheels"
+  upload_pypi:
+    name: "Upload wheels to pypi"
+    needs: [build_wheels, build_sdist]
+    runs-on: ubuntu-latest
+    steps:
+      - uses: actions/download-artifact@v3
+        with:
+          name: dist
+          path: dist
+      - uses: pypa/gh-action-pypi-publish@v1.5.0
+        with:
+          user: __token__
+          password: ${{ secrets.PYPI_API_TOKEN }}
+
+  upload_assets:
+    name: "Upload release assets"
     needs: [build_wheels, build_sdist]
     runs-on: ubuntu-latest
-    if: github.event_name == 'release' && github.event.action == 'published'
     steps:
       - uses: actions/download-artifact@v3
         with:
           name: archive
           path: archive
       - uses: actions/upload-release-asset@v1
         with:
@@ -84,15 +93,7 @@
         with:
           upload_url: ${{ github.event.release.upload_url }}
           asset_path: ./archive/panda_py_${{ env.VERSION }}_libfranka_0.10.0.zip
           asset_name: panda_py_${{ env.VERSION }}_libfranka_0.10.0.zip
           asset_content_type: application/zip
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
-      - uses: actions/download-artifact@v3
-        with:
-          name: dist
-          path: dist
-      - uses: pypa/gh-action-pypi-publish@v1.5.0
-        with:
-          user: __token__
-          password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `panda-python-0.5.1/.pylintrc` & `panda-python-0.5.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/.vscode/settings.json` & `panda-python-0.5.2/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/.vscode/tasks.json` & `panda-python-0.5.2/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/CMakeLists.txt` & `panda-python-0.5.2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/LICENSE` & `panda-python-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/bin/before_install.sh` & `panda-python-0.5.2/bin/before_install_centos.sh`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/bin/build_all.sh` & `panda-python-0.5.2/bin/build_all.sh`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/docs/Makefile` & `panda-python-0.5.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/docs/conf.py` & `panda-python-0.5.2/docs/conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'panda-py'
 copyright = '2023, Jean Elsner'
 author = 'Jean Elsner'
-release = '0.5.1'
+release = '0.5.2'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     'sphinx.ext.autodoc',
     'sphinx.ext.napoleon',
```

### Comparing `panda-python-0.5.1/docs/make.bat` & `panda-python-0.5.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/examples/cartesian_impedance.py` & `panda-python-0.5.2/examples/cartesian_impedance.py`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/examples/communication_test.py` & `panda-python-0.5.2/examples/communication_test.py`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/examples/mmc.py` & `panda-python-0.5.2/examples/mmc.py`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/examples/notebooks/benchmark.ipynb` & `panda-python-0.5.2/examples/notebooks/benchmark.ipynb`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/examples/notebooks/motion.ipynb` & `panda-python-0.5.2/examples/notebooks/motion.ipynb`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/examples/notebooks/paper.ipynb` & `panda-python-0.5.2/examples/notebooks/paper.ipynb`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/include/constants.h` & `panda-python-0.5.2/include/constants.h`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/include/controllers/applied_force.h` & `panda-python-0.5.2/include/controllers/applied_force.h`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/include/controllers/applied_torque.h` & `panda-python-0.5.2/include/controllers/applied_torque.h`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/include/controllers/cartesian_impedance.h` & `panda-python-0.5.2/include/controllers/cartesian_impedance.h`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/include/controllers/controller.h` & `panda-python-0.5.2/include/controllers/controller.h`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/include/controllers/force.h` & `panda-python-0.5.2/include/controllers/force.h`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/include/controllers/integrated_velocity.h` & `panda-python-0.5.2/include/controllers/integrated_velocity.h`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/include/controllers/joint_limits/virtual_wall.h` & `panda-python-0.5.2/include/controllers/joint_limits/virtual_wall.h`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/include/controllers/joint_limits/virtual_wall_controller.h` & `panda-python-0.5.2/include/controllers/joint_limits/virtual_wall_controller.h`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/include/controllers/joint_position.h` & `panda-python-0.5.2/include/controllers/joint_position.h`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/include/controllers/trajectory.h` & `panda-python-0.5.2/include/controllers/trajectory.h`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/include/kinematics/fk.h` & `panda-python-0.5.2/include/kinematics/fk.h`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/include/kinematics/ik.h` & `panda-python-0.5.2/include/kinematics/ik.h`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/include/motion/generators.h` & `panda-python-0.5.2/include/motion/generators.h`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/include/motion/time_optimal/path.h` & `panda-python-0.5.2/include/motion/time_optimal/path.h`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/include/motion/time_optimal/trajectory.h` & `panda-python-0.5.2/include/motion/time_optimal/trajectory.h`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/include/panda.h` & `panda-python-0.5.2/include/panda.h`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/include/utils.h` & `panda-python-0.5.2/include/utils.h`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/logo.jpg` & `panda-python-0.5.2/logo.jpg`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/pyproject.toml` & `panda-python-0.5.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "scikit_build_core.build"
 
 [project]
 name = "panda-python"
 description = "Python bindings for the Panda"
 requires-python = ">=3.7"
 dependencies = ["websockets>=11.0", "requests", "numpy"]
-version = "0.5.1"
+version = "0.5.2"
 authors = [
     { name = "Jean Elsner", email = "jean.elsner@tum.de" },
 ]
 license = {file = "LICENSE"}
 readme = "README.md"
 keywords = ["python", "real-time", "control", "robot", "franka", "emika"]
 classifiers = [
@@ -30,28 +30,33 @@
 examples = [
     "roboticstoolbox-python",
     "matplotlib",
     "spatialmath",
     "ansitable",
     "qpsolvers",
 ]
+docs = [
+    "furo",
+    "sphinx-reredirects",
+    "sphinx",
+]
 
 [project.scripts]
 panda-lock = "panda_py.cli:lock"
 panda-unlock = "panda_py.cli:unlock"
 panda-reboot = "panda_py.cli:reboot"
 
 [tool.cibuildwheel]
 manylinux-x86_64-image = "manylinux2014"
 build = [ "cp37-*", "cp38-*", "cp39-*", "cp310-*", "cp311-*",]
 skip = [ "pp*", "*musllinux*",]
 environment = "LIBFRANKA_VER=0.9.2"
 
 [tool.cibuildwheel.linux]
-before-all = [ "./bin/before_install.sh",]
+before-all = [ "./bin/before_install_centos.sh",]
 archs = [ "x86_64",]
 
 [tool.scikit-build.cmake]
 build-type = "Release"
 
 [tool.scikit-build.wheel]
 packages = ["src/panda_py"]
```

### Comparing `panda-python-0.5.1/src/_core.cpp` & `panda-python-0.5.2/src/_core.cpp`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/src/controllers/applied_force.cpp` & `panda-python-0.5.2/src/controllers/applied_force.cpp`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/src/controllers/applied_torque.cpp` & `panda-python-0.5.2/src/controllers/applied_torque.cpp`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/src/controllers/cartesian_impedance.cpp` & `panda-python-0.5.2/src/controllers/cartesian_impedance.cpp`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/src/controllers/force.cpp` & `panda-python-0.5.2/src/controllers/force.cpp`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/src/controllers/integrated_velocity.cpp` & `panda-python-0.5.2/src/controllers/integrated_velocity.cpp`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/src/controllers/joint_limits/virtual_wall.cpp` & `panda-python-0.5.2/src/controllers/joint_limits/virtual_wall.cpp`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/src/controllers/joint_position.cpp` & `panda-python-0.5.2/src/controllers/joint_position.cpp`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/src/controllers/trajectory.cpp` & `panda-python-0.5.2/src/controllers/trajectory.cpp`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/src/libfranka.cpp` & `panda-python-0.5.2/src/libfranka.cpp`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/src/motion/generators.cpp` & `panda-python-0.5.2/src/motion/generators.cpp`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/src/motion/time_optimal/path.cpp` & `panda-python-0.5.2/src/motion/time_optimal/path.cpp`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/src/motion/time_optimal/trajectory.cpp` & `panda-python-0.5.2/src/motion/time_optimal/trajectory.cpp`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/src/panda.cpp` & `panda-python-0.5.2/src/panda.cpp`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/src/panda_py/__init__.py` & `panda-python-0.5.2/src/panda_py/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Introduction
 ------------
 
 panda-py is a Python library for the Franka Emika Robot System
-that allows you to program and control the robot in Python.
+that allows you to program and control the robot in real-time.
 
 
 """
 
 import base64
 import configparser
 import dataclasses
```

### Comparing `panda-python-0.5.1/src/panda_py/__init__.pyi` & `panda-python-0.5.2/src/panda_py/__init__.pyi`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/src/panda_py/_core/__init__.pyi` & `panda-python-0.5.2/src/panda_py/_core/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -189,14 +189,19 @@
     def start_controller(self, controller: TorqueController) -> None: ...
     def stop_controller(self) -> None: ...
     @property
     def name(self) -> str:
         """
         :type: str
         """
+    @property
+    def q(self) -> numpy.ndarray[numpy.float64, _Shape[7, 1]]:
+        """
+        :type: numpy.ndarray[numpy.float64, _Shape[7, 1]]
+        """
     pass
 class PandaContext():
     def __enter__(self) -> PandaContext: ...
     def __exit__(self, arg0: object, arg1: object, arg2: object) -> bool: ...
     def ok(self) -> bool: ...
     @property
     def num_ticks(self) -> int:
```

### Comparing `panda-python-0.5.1/src/panda_py/cli.py` & `panda-python-0.5.2/src/panda_py/cli.py`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/src/panda_py/constants.py` & `panda-python-0.5.2/src/panda_py/constants.py`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/src/panda_py/controllers.py` & `panda-python-0.5.2/src/panda_py/controllers.py`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/src/panda_py/libfranka/__init__.pyi` & `panda-python-0.5.2/src/panda_py/libfranka/__init__.pyi`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.1/PKG-INFO` & `panda-python-0.5.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panda-python
-Version: 0.5.1
+Version: 0.5.2
 Summary: Python bindings for the Panda
 Keywords: python real-time control robot franka emika
 Author-Email: Jean Elsner <jean.elsner@tum.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -219,25 +219,66 @@
 Requires-Dist: requests
 Requires-Dist: numpy
 Requires-Dist: roboticstoolbox-python; extra == "examples"
 Requires-Dist: matplotlib; extra == "examples"
 Requires-Dist: spatialmath; extra == "examples"
 Requires-Dist: ansitable; extra == "examples"
 Requires-Dist: qpsolvers; extra == "examples"
+Requires-Dist: furo; extra == "docs"
+Requires-Dist: sphinx-reredirects; extra == "docs"
+Requires-Dist: sphinx; extra == "docs"
 Provides-Extra: examples
+Provides-Extra: docs
 Description-Content-Type: text/markdown
 
 # panda-py
+
+> **Info**
+>
+> Please consider this a work in progress. Documentation, continuous integration pipeline and a companion paper are currently being prepared.
+
 ![logo](https://github.com/JeanElsner/panda-py/blob/main/logo.jpg?raw=true)
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/JeanElsner/panda-py/build.yml)](https://github.com/JeanElsner/panda-py/actions/workflows/build.yml)
 [![GitHub](https://img.shields.io/github/license/JeanElsner/panda-py)](https://www.apache.org/licenses/LICENSE-2.0)
 [![PyPI](https://img.shields.io/pypi/v/panda-python)](https://pypi.org/project/panda-python/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/panda-python)
+[![Documentation](https://shields.io/badge/-Documentation-informational)](https://jeanelsner.github.io/panda-py/)
 
 Finally, Python bindings for the Panda. These will increase your productivity by 1000%, guaranteed[^1]!
 
-> **Info**
->
-> Please consider this a work in progress. Documentation, continuous integration pipeline and a companion paper are currently being prepared.
+## Getting started
+
+
+
+## Install
+
+```
+pip install panda-python
+```
+
+This will install panda-py and all its requirements. The pip version ships with libfranka 0.9.2, the newest version for the Franka Emika Robot. Please refer to the section below if you use an older system version or the more recent Franka Research 3 robot. 
+
+## libfranka Version
+
+There are currently two robot models available from Franka Emika: the Franka Emika Robot (FER, formerly known as Panda) and the Franka Research 3 (FR3). Depending on the installed firmware, the FER supports version <=0.9 while the FR3 requires version >=0.10. For details, refer to [this](https://frankaemika.github.io/docs/compatibility.html) compatibility matrix. If you need a libfranka version different from the default 0.9.2, download the respective zip archive from the [release page](https://github.com/JeanElsner/panda-py/releases). Extract the archive and install the wheel for your Python version with pip, e.g., run
+```
+pip install panda_python-*libfranka.0.7.1-cp310*.whl
+```
+to install the binary wheel for libfranka 0.7.1 and Python 3.10.
+
+# Citation
+
+If you use panda-py in published research, please consider citing the [companion paper](https://arxiv.org/abs/2307.07633).
+
+```
+@misc{elsner2023taming,
+      title={Taming the Panda with Python: A Powerful Duo for Seamless Robotics Programming and Integration}, 
+      author={Jean Elsner},
+      year={2023},
+      eprint={2307.07633},
+      archivePrefix={arXiv},
+      primaryClass={cs.RO}
+}
+```
 
 [^1]: Not actually guaranteed. Based on a sample size of one.
```

