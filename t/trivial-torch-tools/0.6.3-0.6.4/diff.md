# Comparing `tmp/trivial_torch_tools-0.6.3.tar.gz` & `tmp/trivial_torch_tools-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trivial_torch_tools-0.6.3.tar", last modified: Thu May 25 21:29:15 2023, max compression
+gzip compressed data, was "trivial_torch_tools-0.6.4.tar", last modified: Tue Jul 18 14:47:50 2023, max compression
```

## Comparing `trivial_torch_tools-0.6.3.tar` & `trivial_torch_tools-0.6.4.tar`

### file list

```diff
@@ -1,394 +1,394 @@
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.239662 trivial_torch_tools-0.6.3/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     3039 2023-05-25 21:29:15.239469 trivial_torch_tools-0.6.3/PKG-INFO
--rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2023-05-25 21:29:15.239711 trivial_torch_tools-0.6.3/setup.cfg
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1453 2023-05-18 16:49:02.000000 trivial_torch_tools-0.6.3/setup.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.181678 trivial_torch_tools-0.6.3/trivial_torch_tools/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.182473 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6126 2023-05-18 16:57:30.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__init__.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.182747 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__pycache__/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     4319 2023-05-18 16:57:34.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.176768 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.184026 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     8884 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/.gitignore
--rw-r--r--   0 jeffhykin   (501) staff       (20)      424 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/.gitrepo
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1850 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/README.md
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.184876 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      156 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/pip
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.185723 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/project/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      461 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/project/clean
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1328 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/project/commands
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       39 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/project/local_install
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      477 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/project/publish
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      860 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/project/purge
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4038 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/shell
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     8865 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/start
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      416 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/subrepo
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.186051 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     8842 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/fornix_framework.md
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.188862 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/images/
--rw-r--r--   0 jeffhykin   (501) staff       (20)   706321 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/images/cd_tutorial.gif
--rw-r--r--   0 jeffhykin   (501) staff       (20)   141455 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/images/package_from_example.png
--rw-r--r--   0 jeffhykin   (501) staff       (20)    67463 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/images/package_name.png
--rw-r--r--   0 jeffhykin   (501) staff       (20)   234123 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/images/package_versions.png
--rw-r--r--   0 jeffhykin   (501) staff       (20)     4209 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/setup.md
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.189538 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/logs/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      315 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/logs/main.py.log
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.189963 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.190337 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/file_system_py/
--rw-r--r--   0 jeffhykin   (501) staff       (20)    12380 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/file_system_py/__init__.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.190575 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/file_system_py/__pycache__/
--rw-r--r--   0 jeffhykin   (501) staff       (20)    10922 2023-05-18 16:57:34.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/file_system_py/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1069 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/license.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1202 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/setup.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)    29546 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/poetry.lock
--rw-r--r--   0 jeffhykin   (501) staff       (20)      483 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/pyproject.toml
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.191132 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/run/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4637 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/run/tests
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4637 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/run/tests.ps1
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.191264 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.191559 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/.cache/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/.cache/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.192211 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_clean/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_clean/450_nix.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      464 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_clean/600_cache_folder.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_clean/801_python.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.192914 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_manual_start/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_manual_start/022_000_setup_pythonpath.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_manual_start/024_000_python_ignores.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_manual_start/081_000__ensure_all_commands_executable__.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.193425 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_purge/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_purge/580_mac_library_caches.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1949 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_purge/802_remove_venv.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.197583 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/000_009__add_path_injections__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1826 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/001_000__setup_zsh__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       75 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/001_010__setup_nix_path__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      190 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/001_010_enable_globbing.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/004_000_add_system_bin.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      368 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/005_000__setup_ld_path__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/010_000__ssl_fix__.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      565 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/019_000_setup_python_venv.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/021_000_ensure_pip_modules.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/022_000_setup_pythonpath.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/024_000_python_ignores.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/081_000__ensure_all_commands_executable__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      225 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/082_000_add_commands_to_path.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      154 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/090_000_run_project_commands.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     2043 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/091_000_commands_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       93 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/092_000_doit_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      252 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/092_000_resume_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)    22180 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/093_000_customize_ll_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)    13674 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/094_000_jeffs_git_shortcuts.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      120 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/095_000_customize_tree_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      186 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/099_050_finish_spaceship_setup_.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.199885 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      204 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/010_000_setting_up_env_message.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/049_000_link_keychain.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/051_000_copy_git_config.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1567 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_deno_store.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      772 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_nix_channel.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1071 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_tealdeer.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       92 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/089_000__sudo_injection__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       94 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/091_000__logger_injection__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      116 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/095_000_vim_injection.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/096_000_vscode_injection.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/097_000_atom_injection.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.176478 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.200045 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6087 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/#establish_extension.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.175318 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.175505 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.200860 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      555 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/add_execute_permission
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      650 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/copy
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2280 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/relative_link
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      348 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/remove
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      280 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/storage
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.201862 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1192 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/basic_init_example
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4392 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/create_wrapped_command
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/ensure_all_commands_executable
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1319 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/inject_into_path
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      795 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/merge_all_templates
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1553 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/trigger
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.202802 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       59 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/escape_grep_regex
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       91 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/escape_shell_argument
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/indent
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       58 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/remove_doublequotes
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1789 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/remove_spaces_from_names
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/unindent
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.203284 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     5930 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/#establish_extension.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.203557 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/commands/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2782 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/commands/ignore
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2254 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/commands/mixin
--rw-r--r--   0 jeffhykin   (501) staff       (20)      244 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/during_cleaning.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/during_start_prep.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.176206 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.203697 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/fsmonitor-watchman/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/fsmonitor-watchman/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.203869 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-merge/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-merge/.keep
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-merge/901_check_pip_modules
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.204088 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-update/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-update/.keep
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-update/901_check_pip_modules
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.204208 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-applypatch/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-applypatch/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.204390 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-commit/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-commit/.keep
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1447 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-commit/002_prevent_large_files.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.204644 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-merge-commit/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-merge-commit/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.204742 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-push/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-push/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.204834 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-receive/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-receive/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.204918 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/prepare-commit-msg/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/prepare-commit-msg/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.205014 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/update/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/update/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.207415 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1376 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/#establish_extension.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)   201623 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/cacert.pem
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.208906 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     7988 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/ensure_nix_installed
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2246 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/fix_ssl
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      742 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/lib_path_for
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      164 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/long_eval
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      746 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/package_path_for
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       62 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/raw_find
--rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/during_clean.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/during_start.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)    28669 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/installer_helper
--rw-r--r--   0 jeffhykin   (501) staff       (20)     8590 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/nix.toml
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.209073 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/nixpkgs/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      604 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/nixpkgs/salt.nix
--rw-r--r--   0 jeffhykin   (501) staff       (20)    13466 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/parse_dependencies.nix
--rw-r--r--   0 jeffhykin   (501) staff       (20)      228 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/settings.toml
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6031 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/shell.nix
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5862 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/uninstaller_helper
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.209684 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/os_mac/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      500 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/os_mac/#establish_extension.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/os_mac/during_purge.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/os_mac/during_start_prep.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.210148 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     2072 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/#establish_extension.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.211379 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/add_project_to_pythonpath
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/ensure_pip_modules
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/refresh_ignores
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      565 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/setup_venv
--rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/during_clean.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1949 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/during_purge.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6180 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/fornix_core
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.211830 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/home/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1471 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/home/.zshenv
--rw-r--r--   0 jeffhykin   (501) staff       (20)       76 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/home/.zshrc
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.212231 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/requirements/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6031 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/requirements/advanced_system_tools.nix
--rw-r--r--   0 jeffhykin   (501) staff       (20)     8590 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/requirements/system_tools.toml
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.212350 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/tests/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1044 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/tests/main.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.213207 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     8884 2023-05-25 21:27:34.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/.gitignore
--rw-r--r--   0 jeffhykin   (501) staff       (20)      416 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/.gitrepo
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1327 2023-05-25 21:27:34.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/README.md
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.213671 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      156 2023-05-25 21:27:34.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/pip
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.214277 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/project/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      461 2023-05-25 21:27:34.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/project/clean
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1328 2023-05-25 21:27:34.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/project/commands
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       39 2023-05-25 21:27:34.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/project/local_install
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      477 2023-05-25 21:27:34.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/project/publish
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      860 2023-05-25 21:27:34.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/project/purge
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4038 2023-05-25 21:27:34.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/shell
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     8865 2023-05-25 21:27:34.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/start
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      416 2023-05-25 21:27:34.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/subrepo
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.214522 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     8842 2023-05-25 21:27:34.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/fornix_framework.md
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.215901 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/images/
--rw-r--r--   0 jeffhykin   (501) staff       (20)   706321 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/images/cd_tutorial.gif
--rw-r--r--   0 jeffhykin   (501) staff       (20)   141455 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/images/package_from_example.png
--rw-r--r--   0 jeffhykin   (501) staff       (20)    67463 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/images/package_name.png
--rw-r--r--   0 jeffhykin   (501) staff       (20)   234123 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/images/package_versions.png
--rw-r--r--   0 jeffhykin   (501) staff       (20)     4209 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/setup.md
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.216588 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/.keep
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1069 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/license.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)     3216 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/setup.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.216718 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/super_hash/
--rw-r--r--   0 jeffhykin   (501) staff       (20)    12054 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/super_hash/__init__.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)    27813 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/poetry.lock
--rw-r--r--   0 jeffhykin   (501) staff       (20)      486 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/pyproject.toml
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.216843 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.216964 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/.cache/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/.cache/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.217446 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_clean/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_clean/450_nix.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      464 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_clean/600_cache_folder.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_clean/801_python.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.218227 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_manual_start/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_manual_start/022_000_setup_pythonpath.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_manual_start/024_000_python_ignores.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_manual_start/081_000__ensure_all_commands_executable__.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.218486 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_purge/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_purge/580_mac_library_caches.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1949 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_purge/802_remove_venv.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.220878 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/000_009__add_path_injections__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1826 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/001_000__setup_zsh__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       75 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/001_010__setup_nix_path__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      190 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/001_010_enable_globbing.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/004_000_add_system_bin.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      368 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/005_000__setup_ld_path__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/010_000__ssl_fix__.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      565 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/019_000_setup_python_venv.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/021_000_ensure_pip_modules.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/022_000_setup_pythonpath.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/024_000_python_ignores.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/081_000__ensure_all_commands_executable__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      225 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/082_000_add_commands_to_path.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      154 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/090_000_run_project_commands.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     2043 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/091_000_commands_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       93 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/092_000_doit_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      252 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/092_000_resume_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)    22180 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/093_000_customize_ll_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)    13674 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/094_000_jeffs_git_shortcuts.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      120 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/095_000_customize_tree_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      186 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/099_050_finish_spaceship_setup_.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.222031 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      204 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/010_000_setting_up_env_message.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/049_000_link_keychain.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/051_000_copy_git_config.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1567 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/060_010_link_deno_store.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      772 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/060_010_link_nix_channel.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1071 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/060_010_link_tealdeer.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       92 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/089_000__sudo_injection__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       94 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/091_000__logger_injection__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      116 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/095_000_vim_injection.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/096_000_vscode_injection.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/097_000_atom_injection.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.178762 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.222136 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6087 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/#establish_extension.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.177674 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.177831 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.222671 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      555 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/add_execute_permission
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      650 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/copy
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2280 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/relative_link
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      348 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/remove
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      280 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/storage
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.223325 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1192 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/basic_init_example
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4392 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/create_wrapped_command
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/ensure_all_commands_executable
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1319 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/inject_into_path
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      795 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/merge_all_templates
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1553 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/trigger
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.223962 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       59 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/escape_grep_regex
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       91 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/escape_shell_argument
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/indent
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       58 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/remove_doublequotes
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1789 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/remove_spaces_from_names
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/unindent
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.224279 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     5930 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/#establish_extension.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.224500 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/commands/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2782 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/commands/ignore
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2254 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/commands/mixin
--rw-r--r--   0 jeffhykin   (501) staff       (20)      244 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/during_cleaning.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/during_start_prep.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.178538 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.224611 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/fsmonitor-watchman/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/fsmonitor-watchman/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.224782 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-merge/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-merge/.keep
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-merge/901_check_pip_modules
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.224973 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-update/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-update/.keep
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-update/901_check_pip_modules
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.225081 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-applypatch/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-applypatch/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.225244 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-commit/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-commit/.keep
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1447 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-commit/002_prevent_large_files.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.225348 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-merge-commit/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-merge-commit/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.225425 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-push/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-push/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.225503 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-receive/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-receive/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.225587 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/prepare-commit-msg/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/prepare-commit-msg/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.225872 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/update/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/update/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.228059 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1376 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/#establish_extension.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)   201623 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/cacert.pem
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.231573 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     7988 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/ensure_nix_installed
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2246 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/fix_ssl
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      742 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/lib_path_for
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      164 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/long_eval
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      746 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/package_path_for
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       62 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/raw_find
--rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/during_clean.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/during_start.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)    28669 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/installer_helper
--rw-r--r--   0 jeffhykin   (501) staff       (20)     8590 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/nix.toml
--rw-r--r--   0 jeffhykin   (501) staff       (20)    13466 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/parse_dependencies.nix
--rw-r--r--   0 jeffhykin   (501) staff       (20)      228 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/settings.toml
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6031 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/shell.nix
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5862 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/uninstaller_helper
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.232227 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/os_mac/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      500 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/os_mac/#establish_extension.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/os_mac/during_purge.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/os_mac/during_start_prep.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.233959 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     2072 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/#establish_extension.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.234447 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/add_project_to_pythonpath
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/ensure_pip_modules
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/refresh_ignores
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      565 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/setup_venv
--rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/during_clean.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1949 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/during_purge.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6180 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/fornix_core
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.234671 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/home/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1471 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/home/.zshenv
--rw-r--r--   0 jeffhykin   (501) staff       (20)       76 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/home/.zshrc
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.234893 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/requirements/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6031 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/requirements/advanced_system_tools.nix
--rw-r--r--   0 jeffhykin   (501) staff       (20)     8590 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/requirements/system_tools.toml
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.235100 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/tests/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      321 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/tests/output.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)      644 2023-05-25 21:27:35.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/tests/test.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)       19 2023-05-18 17:17:03.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__init__.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.238428 trivial_torch_tools-0.6.3/trivial_torch_tools/__pycache__/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      191 2023-05-18 17:17:59.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 jeffhykin   (501) staff       (20)     3260 2023-05-18 17:18:00.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__pycache__/core.cpython-38.pyc
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6818 2023-05-18 17:18:00.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__pycache__/generics.cpython-38.pyc
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1865 2023-05-18 17:19:18.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__pycache__/image.cpython-38.pyc
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1549 2023-05-18 17:19:18.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__pycache__/main.cpython-38.pyc
--rw-r--r--   0 jeffhykin   (501) staff       (20)     2669 2023-05-18 17:18:00.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__pycache__/misc.cpython-38.pyc
--rw-r--r--   0 jeffhykin   (501) staff       (20)     8971 2023-05-18 17:18:00.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__pycache__/model.cpython-38.pyc
--rw-r--r--   0 jeffhykin   (501) staff       (20)     2112 2023-05-18 17:18:00.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/__pycache__/one_hots.cpython-38.pyc
--rw-r--r--   0 jeffhykin   (501) staff       (20)     4653 2023-05-18 16:41:54.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/core.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)     8874 2023-05-18 17:17:49.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/generics.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1328 2023-05-18 16:25:43.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/image.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)      897 2023-05-18 17:19:17.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/main.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)     2820 2023-05-18 17:17:53.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/misc.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)     8906 2023-05-18 16:42:07.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/model.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1746 2023-05-18 16:42:16.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/one_hots.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)      380 2023-05-18 16:48:39.000000 trivial_torch_tools-0.6.3/trivial_torch_tools/settings.json
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 21:29:15.182370 trivial_torch_tools-0.6.3/trivial_torch_tools.egg-info/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     3039 2023-05-25 21:29:14.000000 trivial_torch_tools-0.6.3/trivial_torch_tools.egg-info/PKG-INFO
--rw-r--r--   0 jeffhykin   (501) staff       (20)    30299 2023-05-25 21:29:15.000000 trivial_torch_tools-0.6.3/trivial_torch_tools.egg-info/SOURCES.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2023-05-25 21:29:14.000000 trivial_torch_tools-0.6.3/trivial_torch_tools.egg-info/dependency_links.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       19 2023-05-25 21:29:14.000000 trivial_torch_tools-0.6.3/trivial_torch_tools.egg-info/requires.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       20 2023-05-25 21:29:14.000000 trivial_torch_tools-0.6.3/trivial_torch_tools.egg-info/top_level.txt
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.886088 trivial_torch_tools-0.6.4/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     3039 2023-07-18 14:47:50.885935 trivial_torch_tools-0.6.4/PKG-INFO
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2023-07-18 14:47:50.886133 trivial_torch_tools-0.6.4/setup.cfg
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1453 2023-05-18 16:49:02.000000 trivial_torch_tools-0.6.4/setup.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.794659 trivial_torch_tools-0.6.4/trivial_torch_tools/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.795474 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6452 2023-07-18 14:43:50.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__init__.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.795771 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__pycache__/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     4319 2023-05-18 16:57:34.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.789449 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.797426 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8884 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/.gitignore
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      424 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/.gitrepo
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1850 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/README.md
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.798647 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      156 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/pip
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.800017 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/project/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      461 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/project/clean
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1328 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/project/commands
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       39 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/project/local_install
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      477 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/project/publish
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      860 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/project/purge
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4038 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/shell
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     8865 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/start
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      416 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/subrepo
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.800408 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8842 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/fornix_framework.md
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.803770 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/images/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   706321 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/images/cd_tutorial.gif
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   141455 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/images/package_from_example.png
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    67463 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/images/package_name.png
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   234123 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/images/package_versions.png
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     4209 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/setup.md
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.804444 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/logs/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      315 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/logs/main.py.log
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.804975 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.805188 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/file_system_py/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    12380 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/file_system_py/__init__.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.805386 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/file_system_py/__pycache__/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    10922 2023-05-18 16:57:34.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/file_system_py/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1069 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/license.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1202 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/setup.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    29546 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/poetry.lock
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      483 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/pyproject.toml
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.806091 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/run/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4637 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/run/tests
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4637 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/run/tests.ps1
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.806253 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.806568 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/.cache/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/.cache/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.807184 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_clean/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_clean/450_nix.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      464 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_clean/600_cache_folder.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_clean/801_python.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.807923 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_manual_start/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_manual_start/022_000_setup_pythonpath.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_manual_start/024_000_python_ignores.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_manual_start/081_000__ensure_all_commands_executable__.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.808391 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_purge/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_purge/580_mac_library_caches.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1949 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_purge/802_remove_venv.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.812605 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/000_009__add_path_injections__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1826 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/001_000__setup_zsh__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       75 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/001_010__setup_nix_path__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      190 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/001_010_enable_globbing.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/004_000_add_system_bin.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      368 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/005_000__setup_ld_path__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/010_000__ssl_fix__.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      565 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/019_000_setup_python_venv.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/021_000_ensure_pip_modules.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/022_000_setup_pythonpath.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/024_000_python_ignores.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/081_000__ensure_all_commands_executable__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      225 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/082_000_add_commands_to_path.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      154 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/090_000_run_project_commands.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     2043 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/091_000_commands_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       93 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/092_000_doit_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      252 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/092_000_resume_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    22180 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/093_000_customize_ll_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    13674 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/094_000_jeffs_git_shortcuts.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      120 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/095_000_customize_tree_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      186 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/099_050_finish_spaceship_setup_.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.815152 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      204 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/010_000_setting_up_env_message.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/049_000_link_keychain.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/051_000_copy_git_config.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1567 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_deno_store.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      772 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_nix_channel.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1071 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_tealdeer.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       92 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/089_000__sudo_injection__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       94 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/091_000__logger_injection__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      116 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/095_000_vim_injection.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/096_000_vscode_injection.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/097_000_atom_injection.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.789160 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.815347 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6087 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/#establish_extension.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.787438 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.787593 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.816460 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      555 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/add_execute_permission
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      650 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/copy
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2280 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/relative_link
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      348 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/remove
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      280 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/storage
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.817514 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1192 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/basic_init_example
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4392 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/create_wrapped_command
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/ensure_all_commands_executable
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1319 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/inject_into_path
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      795 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/merge_all_templates
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1553 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/trigger
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.818971 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       59 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/escape_grep_regex
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       91 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/escape_shell_argument
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/indent
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       58 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/remove_doublequotes
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1789 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/remove_spaces_from_names
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/unindent
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.819706 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     5930 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/#establish_extension.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.820032 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2782 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/commands/ignore
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2254 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/commands/mixin
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      244 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/during_cleaning.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/during_start_prep.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.788728 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.820509 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/fsmonitor-watchman/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/fsmonitor-watchman/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.820767 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-merge/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-merge/.keep
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-merge/901_check_pip_modules
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.824129 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-update/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-update/.keep
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-update/901_check_pip_modules
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.824399 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-applypatch/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-applypatch/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.824627 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-commit/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-commit/.keep
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1447 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-commit/002_prevent_large_files.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.826347 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-merge-commit/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-merge-commit/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.826486 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-push/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-push/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.826579 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-receive/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-receive/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.826665 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/prepare-commit-msg/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/prepare-commit-msg/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.826749 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/update/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/update/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.832984 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1376 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/#establish_extension.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   201623 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/cacert.pem
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.834775 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     7988 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/ensure_nix_installed
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2246 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/fix_ssl
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      742 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/lib_path_for
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      164 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/long_eval
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      746 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/package_path_for
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       62 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/raw_find
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/during_clean.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/during_start.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)    28669 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/installer_helper
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8590 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/nix.toml
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.835720 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/nixpkgs/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      604 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/nixpkgs/salt.nix
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    13466 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/parse_dependencies.nix
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      228 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/settings.toml
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6031 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/shell.nix
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5862 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/uninstaller_helper
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.836267 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/os_mac/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      500 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/os_mac/#establish_extension.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/os_mac/during_purge.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/os_mac/during_start_prep.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.838923 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     2072 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/#establish_extension.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.839460 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/add_project_to_pythonpath
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/ensure_pip_modules
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/refresh_ignores
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      565 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/setup_venv
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/during_clean.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1949 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/during_purge.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6180 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/fornix_core
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.840543 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/home/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1471 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/home/.zshenv
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       76 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/home/.zshrc
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.842331 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/requirements/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6031 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/requirements/advanced_system_tools.nix
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8590 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/requirements/system_tools.toml
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.842492 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/tests/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1044 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/tests/main.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.845095 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8884 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/.gitignore
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      420 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/.gitrepo
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1327 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/README.md
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.845987 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      156 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/pip
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.846881 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/project/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      461 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/project/clean
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1328 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/project/commands
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       39 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/project/local_install
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      477 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/project/publish
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      860 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/project/purge
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4038 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/shell
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     8865 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/start
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      416 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/subrepo
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.847534 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8842 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/fornix_framework.md
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.852004 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/images/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   706321 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/images/cd_tutorial.gif
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   141455 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/images/package_from_example.png
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    67463 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/images/package_name.png
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   234123 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/images/package_versions.png
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     4209 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/setup.md
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.853229 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/.keep
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1069 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/license.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     3216 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/setup.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.853412 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/super_hash/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    12071 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/super_hash/__init__.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    27813 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/poetry.lock
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      486 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/pyproject.toml
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.853600 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.855357 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/.cache/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/.cache/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.856006 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_clean/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_clean/450_nix.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      464 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_clean/600_cache_folder.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_clean/801_python.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.856813 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_manual_start/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_manual_start/022_000_setup_pythonpath.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_manual_start/024_000_python_ignores.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_manual_start/081_000__ensure_all_commands_executable__.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.857512 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_purge/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_purge/580_mac_library_caches.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1949 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_purge/802_remove_venv.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.863742 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/000_009__add_path_injections__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1826 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/001_000__setup_zsh__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       75 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/001_010__setup_nix_path__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      190 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/001_010_enable_globbing.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/004_000_add_system_bin.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      368 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/005_000__setup_ld_path__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/010_000__ssl_fix__.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      565 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/019_000_setup_python_venv.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/021_000_ensure_pip_modules.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/022_000_setup_pythonpath.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/024_000_python_ignores.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/081_000__ensure_all_commands_executable__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      225 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/082_000_add_commands_to_path.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      154 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/090_000_run_project_commands.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     2043 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/091_000_commands_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       93 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/092_000_doit_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      252 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/092_000_resume_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    22180 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/093_000_customize_ll_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    13674 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/094_000_jeffs_git_shortcuts.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      120 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/095_000_customize_tree_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      186 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/099_050_finish_spaceship_setup_.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.866018 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      204 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/010_000_setting_up_env_message.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/049_000_link_keychain.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/051_000_copy_git_config.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1567 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/060_010_link_deno_store.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      772 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/060_010_link_nix_channel.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1071 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/060_010_link_tealdeer.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       92 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/089_000__sudo_injection__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       94 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/091_000__logger_injection__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      116 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/095_000_vim_injection.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/096_000_vscode_injection.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/097_000_atom_injection.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.791520 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.866213 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6087 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/#establish_extension.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.790359 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.790523 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.867101 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      555 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/add_execute_permission
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      650 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/copy
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2280 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/relative_link
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      348 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/remove
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      280 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/storage
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.868362 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1192 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/basic_init_example
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4392 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/create_wrapped_command
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/ensure_all_commands_executable
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1319 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/inject_into_path
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      795 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/merge_all_templates
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1553 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/trigger
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.870161 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       59 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/escape_grep_regex
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       91 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/escape_shell_argument
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/indent
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       58 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/remove_doublequotes
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1789 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/remove_spaces_from_names
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/unindent
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.870725 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     5930 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/#establish_extension.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.871040 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2782 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/commands/ignore
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2254 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/commands/mixin
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      244 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/during_cleaning.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/during_start_prep.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.791277 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.871203 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/fsmonitor-watchman/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/fsmonitor-watchman/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.871397 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-merge/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-merge/.keep
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-merge/901_check_pip_modules
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.872157 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-update/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-update/.keep
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-update/901_check_pip_modules
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.872288 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-applypatch/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-applypatch/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.872804 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-commit/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-commit/.keep
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1447 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-commit/002_prevent_large_files.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.873003 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-merge-commit/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-merge-commit/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.873098 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-push/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-push/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.873187 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-receive/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-receive/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.873271 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/prepare-commit-msg/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/prepare-commit-msg/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.873355 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/update/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/update/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.876534 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1376 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/#establish_extension.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   201623 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/cacert.pem
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.878247 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     7988 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/ensure_nix_installed
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2246 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/fix_ssl
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      742 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/lib_path_for
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      164 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/long_eval
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      746 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/package_path_for
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       62 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/raw_find
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/during_clean.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/during_start.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)    28669 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/installer_helper
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8590 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/nix.toml
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    13466 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/parse_dependencies.nix
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      228 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/settings.toml
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6031 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/shell.nix
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5862 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/uninstaller_helper
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.878717 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/os_mac/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      500 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/os_mac/#establish_extension.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/os_mac/during_purge.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/os_mac/during_start_prep.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.879128 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     2072 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/#establish_extension.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.879763 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/add_project_to_pythonpath
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/ensure_pip_modules
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/refresh_ignores
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      565 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/setup_venv
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/during_clean.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1949 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/during_purge.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6180 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/fornix_core
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.880117 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/home/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1471 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/home/.zshenv
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       76 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/home/.zshrc
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.880714 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/requirements/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6031 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/requirements/advanced_system_tools.nix
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8590 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/requirements/system_tools.toml
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.881024 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/tests/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      321 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/tests/output.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      644 2023-05-28 15:35:15.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/tests/test.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       19 2023-05-18 17:17:03.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__init__.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.885649 trivial_torch_tools-0.6.4/trivial_torch_tools/__pycache__/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      191 2023-05-18 17:17:59.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     3260 2023-05-18 17:18:00.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__pycache__/core.cpython-38.pyc
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6818 2023-05-18 17:18:00.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__pycache__/generics.cpython-38.pyc
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1865 2023-05-18 17:19:18.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__pycache__/image.cpython-38.pyc
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1549 2023-05-18 17:19:18.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__pycache__/main.cpython-38.pyc
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     2669 2023-05-18 17:18:00.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__pycache__/misc.cpython-38.pyc
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8971 2023-05-18 17:18:00.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__pycache__/model.cpython-38.pyc
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     2112 2023-05-18 17:18:00.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/__pycache__/one_hots.cpython-38.pyc
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     4653 2023-05-18 16:41:54.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/core.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8874 2023-05-18 17:17:49.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/generics.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1328 2023-05-18 16:25:43.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/image.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      897 2023-05-18 17:19:17.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/main.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     2820 2023-05-18 17:17:53.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/misc.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8906 2023-05-18 16:42:07.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/model.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1746 2023-05-18 16:42:16.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/one_hots.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      380 2023-05-18 16:48:39.000000 trivial_torch_tools-0.6.4/trivial_torch_tools/settings.json
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-07-18 14:47:50.795369 trivial_torch_tools-0.6.4/trivial_torch_tools.egg-info/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     3039 2023-07-18 14:47:50.000000 trivial_torch_tools-0.6.4/trivial_torch_tools.egg-info/PKG-INFO
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    30299 2023-07-18 14:47:50.000000 trivial_torch_tools-0.6.4/trivial_torch_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2023-07-18 14:47:50.000000 trivial_torch_tools-0.6.4/trivial_torch_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       19 2023-07-18 14:47:50.000000 trivial_torch_tools-0.6.4/trivial_torch_tools.egg-info/requires.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       20 2023-07-18 14:47:50.000000 trivial_torch_tools-0.6.4/trivial_torch_tools.egg-info/top_level.txt
```

### Comparing `trivial_torch_tools-0.6.3/PKG-INFO` & `trivial_torch_tools-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trivial_torch_tools
-Version: 0.6.3
+Version: 0.6.4
 Summary: Decorators for reducing pytorch boilerplate
 Home-page: https://github.com/jeff-hykin/trivial-torch-tools.git
 Author: Jeff Hykin
 Author-email: jeff.hykin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `trivial_torch_tools-0.6.3/setup.py` & `trivial_torch_tools-0.6.4/setup.py`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__init__.py` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from pathlib import Path
 import os
 import shutil
 import sys
 import warnings # TODO: convert serveral prints to warnings
 from hashlib import md5 
 
+is_windows = os.name == 'nt'
 # 
 # helpers
 # 
 def consistent_hash(value):
     if isinstance(value, bytes):
         return md5(value).hexdigest()
     
@@ -149,30 +150,37 @@
     if not dependency_name.isidentifier():
         raise Exception(f"""dependency names must be an identifier ("blah".isidentifier() in python), but this one is not: {dependency_name}. This source of that name is in: {settings_path}""")
     
     target_path = join(this_folder, dependency_info["path"])
     relative_target_path = make_relative_path(to=target_path, coming_from=best_import_zone_match)
     # ensure the parent folder
     *path_parts, _, _ = path_pieces(join(relative_target_path, "_"))
-    eval_part = dependency_info.get("eval", dependency_name)
     unique_name = f"{dependency_name}_{random()}_{counter}".replace(".","")
     target_folder_for_import = join(this_folder, dependency_name)
-    if not Path(target_folder_for_import).is_symlink() or final_target_of(target_folder_for_import) != dependency_info["path"]:
-        # clear the way
+    
+    target_path_obj = Path(target_folder_for_import)
+    if is_windows:
+        if not target_path_obj.exists():
+            # windows has to copy the files because it can't symlink
+            if os.path.isdir(target_path):
+                shutil.copytree(target_path, target_folder_for_import)
+            else:
+                shutil.copy(target_path, target_folder_for_import)
+    elif not target_path_obj.is_symlink() or final_target_of(target_folder_for_import) != dependency_info["path"]:
+        # clear the way (encase something was in the way)
         remove(target_folder_for_import)
-        # symlink the folder
-        Path(target_folder_for_import).symlink_to(dependency_info["path"])
-
+        target_path_obj.symlink_to(dependency_info["path"])
+        
 # import the paths
 __all__ = []
 for dependency_name, dependency_info in dependency_mapping.items():
     # this will register it with python and convert it to a proper module with a unique path (important for pickling things)
     try:
         exec(f"""from .{dependency_name} import __file__ as _""")
         __all__.append(dependency_name)
     except ImportError as error:
-        if f"{error}" == "ImportError: cannot import name '__file__'":
+        if f"{error}" == "cannot import name '__file__'":
             # this means top level folder isn't a module or doesnt have a __init__.py
             # some modules simply are like this
             pass
         else:
             raise error
```

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__pycache__/__init__.cpython-38.pyc` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/.gitignore` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/.gitignore`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/README.md` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/README.md`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/project/commands` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/project/commands`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/project/purge` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/project/purge`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/shell` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/shell`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/start` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/start`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/fornix_framework.md` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/fornix_framework.md`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/images/cd_tutorial.gif` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/images/cd_tutorial.gif`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/images/package_from_example.png` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/images/package_from_example.png`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/images/package_name.png` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/images/package_name.png`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/images/package_versions.png` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/images/package_versions.png`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/setup.md` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/setup.md`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/file_system_py/__init__.py` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/file_system_py/__init__.py`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/file_system_py/__pycache__/__init__.cpython-38.pyc` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/file_system_py/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/license.txt` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/license.txt`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/setup.py` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/setup.py`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/poetry.lock` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/poetry.lock`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/run/tests` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/run/tests`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/run/tests.ps1` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/run/tests.ps1`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_manual_start/081_000__ensure_all_commands_executable__.sh` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_manual_start/081_000__ensure_all_commands_executable__.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_purge/802_remove_venv.sh` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_purge/802_remove_venv.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/001_000__setup_zsh__.sh` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/001_000__setup_zsh__.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/019_000_setup_python_venv.sh` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/019_000_setup_python_venv.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/021_000_ensure_pip_modules.sh` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/021_000_ensure_pip_modules.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/081_000__ensure_all_commands_executable__.sh` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/081_000__ensure_all_commands_executable__.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/091_000_commands_function.sh` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/091_000_commands_function.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/093_000_customize_ll_function.sh` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/093_000_customize_ll_function.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/094_000_jeffs_git_shortcuts.sh` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/094_000_jeffs_git_shortcuts.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_deno_store.sh` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_deno_store.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_nix_channel.sh` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_nix_channel.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_tealdeer.sh` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_tealdeer.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/#establish_extension.sh` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/#establish_extension.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/add_execute_permission` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/add_execute_permission`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/copy` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/copy`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/relative_link` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/relative_link`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/basic_init_example` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/basic_init_example`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/create_wrapped_command` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/create_wrapped_command`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/ensure_all_commands_executable` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/ensure_all_commands_executable`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/inject_into_path` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/inject_into_path`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/merge_all_templates` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/merge_all_templates`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/trigger` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/trigger`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/remove_spaces_from_names` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/remove_spaces_from_names`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/#establish_extension.sh` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/#establish_extension.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/commands/ignore` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/commands/ignore`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/commands/mixin` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/commands/mixin`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-merge/901_check_pip_modules` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-merge/901_check_pip_modules`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-update/901_check_pip_modules` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-update/901_check_pip_modules`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-commit/002_prevent_large_files.sh` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-commit/002_prevent_large_files.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/#establish_extension.sh` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/#establish_extension.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/cacert.pem` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/cacert.pem`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/ensure_nix_installed` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/ensure_nix_installed`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/fix_ssl` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/fix_ssl`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/lib_path_for` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/lib_path_for`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/package_path_for` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/package_path_for`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/installer_helper` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/installer_helper`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/nix.toml` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/nix.toml`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/nixpkgs/salt.nix` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/nixpkgs/salt.nix`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/parse_dependencies.nix` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/parse_dependencies.nix`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/shell.nix` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/shell.nix`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/uninstaller_helper` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/uninstaller_helper`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/#establish_extension.sh` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/#establish_extension.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/ensure_pip_modules` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/ensure_pip_modules`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/setup_venv` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/setup_venv`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/during_purge.sh` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/during_purge.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/fornix_core` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/fornix_core`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/home/.zshenv` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/home/.zshenv`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/requirements/advanced_system_tools.nix` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/requirements/advanced_system_tools.nix`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/requirements/system_tools.toml` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/requirements/system_tools.toml`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/file_system_py/tests/main.py` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/file_system_py/tests/main.py`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/.gitignore` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/.gitignore`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/README.md` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/README.md`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/project/commands` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/project/commands`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/project/purge` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/project/purge`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/shell` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/shell`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/start` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/start`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/fornix_framework.md` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/fornix_framework.md`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/images/cd_tutorial.gif` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/images/cd_tutorial.gif`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/images/package_from_example.png` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/images/package_from_example.png`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/images/package_name.png` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/images/package_name.png`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/images/package_versions.png` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/images/package_versions.png`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/setup.md` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/setup.md`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/license.txt` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/license.txt`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/setup.py` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/setup.py`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/super_hash/__init__.py` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/super_hash/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,15 @@
             if function_reference is None:
                 continue
             try:
                 instructions = dis.get_instructions(function_reference)
             except TypeError as error:
                 continue
             instruction_hashes.append(function_hashers.instructions_to_hash(instructions))
-            child_names = get_referenced_function_names(instructions)
+            child_names = function_hashers.get_referenced_function_names(instructions)
             for child_name in child_names:
                 if child_name not in closed_set:
                     frontier.add(child_name)
         hash_str = ' '.join(instruction_hashes).encode('utf-8')
         return consistent_hash(hash_str)
     
 try:
```

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/poetry.lock` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/poetry.lock`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_manual_start/081_000__ensure_all_commands_executable__.sh` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_manual_start/081_000__ensure_all_commands_executable__.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_purge/802_remove_venv.sh` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_purge/802_remove_venv.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/001_000__setup_zsh__.sh` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/001_000__setup_zsh__.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/019_000_setup_python_venv.sh` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/019_000_setup_python_venv.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/021_000_ensure_pip_modules.sh` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/021_000_ensure_pip_modules.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/081_000__ensure_all_commands_executable__.sh` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/081_000__ensure_all_commands_executable__.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/091_000_commands_function.sh` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/091_000_commands_function.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/093_000_customize_ll_function.sh` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/093_000_customize_ll_function.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/094_000_jeffs_git_shortcuts.sh` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/094_000_jeffs_git_shortcuts.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/060_010_link_deno_store.sh` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/060_010_link_deno_store.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/060_010_link_nix_channel.sh` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/060_010_link_nix_channel.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/060_010_link_tealdeer.sh` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/060_010_link_tealdeer.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/#establish_extension.sh` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/#establish_extension.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/add_execute_permission` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/add_execute_permission`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/copy` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/copy`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/relative_link` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/relative_link`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/basic_init_example` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/basic_init_example`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/create_wrapped_command` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/create_wrapped_command`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/ensure_all_commands_executable` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/ensure_all_commands_executable`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/inject_into_path` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/inject_into_path`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/merge_all_templates` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/merge_all_templates`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/trigger` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/trigger`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/remove_spaces_from_names` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/remove_spaces_from_names`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/#establish_extension.sh` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/#establish_extension.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/commands/ignore` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/commands/ignore`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/commands/mixin` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/commands/mixin`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-merge/901_check_pip_modules` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-merge/901_check_pip_modules`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-update/901_check_pip_modules` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-update/901_check_pip_modules`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-commit/002_prevent_large_files.sh` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-commit/002_prevent_large_files.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/#establish_extension.sh` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/#establish_extension.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/cacert.pem` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/cacert.pem`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/ensure_nix_installed` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/ensure_nix_installed`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/fix_ssl` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/fix_ssl`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/lib_path_for` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/lib_path_for`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/package_path_for` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/package_path_for`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/installer_helper` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/installer_helper`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/nix.toml` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/nix.toml`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/parse_dependencies.nix` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/parse_dependencies.nix`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/shell.nix` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/shell.nix`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/uninstaller_helper` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/uninstaller_helper`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/#establish_extension.sh` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/#establish_extension.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/ensure_pip_modules` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/ensure_pip_modules`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/setup_venv` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/setup_venv`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/during_purge.sh` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/during_purge.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/fornix_core` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/fornix_core`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/home/.zshenv` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/home/.zshenv`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/requirements/advanced_system_tools.nix` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/requirements/advanced_system_tools.nix`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/requirements/system_tools.toml` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/requirements/system_tools.toml`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__dependencies__/__sources__/super_hash/tests/test.py` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__dependencies__/__sources__/super_hash/tests/test.py`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__pycache__/core.cpython-38.pyc` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__pycache__/core.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__pycache__/generics.cpython-38.pyc` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__pycache__/generics.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__pycache__/image.cpython-38.pyc` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__pycache__/image.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__pycache__/main.cpython-38.pyc` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__pycache__/main.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__pycache__/misc.cpython-38.pyc` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__pycache__/misc.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__pycache__/model.cpython-38.pyc` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__pycache__/model.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/__pycache__/one_hots.cpython-38.pyc` & `trivial_torch_tools-0.6.4/trivial_torch_tools/__pycache__/one_hots.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/core.py` & `trivial_torch_tools-0.6.4/trivial_torch_tools/core.py`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/generics.py` & `trivial_torch_tools-0.6.4/trivial_torch_tools/generics.py`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/image.py` & `trivial_torch_tools-0.6.4/trivial_torch_tools/image.py`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/main.py` & `trivial_torch_tools-0.6.4/trivial_torch_tools/main.py`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/misc.py` & `trivial_torch_tools-0.6.4/trivial_torch_tools/misc.py`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/model.py` & `trivial_torch_tools-0.6.4/trivial_torch_tools/model.py`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools/one_hots.py` & `trivial_torch_tools-0.6.4/trivial_torch_tools/one_hots.py`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools.egg-info/PKG-INFO` & `trivial_torch_tools-0.6.4/trivial_torch_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trivial-torch-tools
-Version: 0.6.3
+Version: 0.6.4
 Summary: Decorators for reducing pytorch boilerplate
 Home-page: https://github.com/jeff-hykin/trivial-torch-tools.git
 Author: Jeff Hykin
 Author-email: jeff.hykin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `trivial_torch_tools-0.6.3/trivial_torch_tools.egg-info/SOURCES.txt` & `trivial_torch_tools-0.6.4/trivial_torch_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

