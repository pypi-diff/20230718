# Comparing `tmp/cycode-0.2.6.dev8.tar.gz` & `tmp/cycode-0.2.6.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cycode-0.2.6.dev8.tar", max compression
+gzip compressed data, was "cycode-0.2.6.dev9.tar", max compression
```

## Comparing `cycode-0.2.6.dev8.tar` & `cycode-0.2.6.dev9.tar`

### file list

```diff
@@ -1,65 +1,66 @@
--rw-r--r--   0        0        0    32549 2023-07-05 14:26:43.321436 cycode-0.2.6.dev8/README.md
--rw-r--r--   0        0        0      114 2023-07-05 14:27:13.841938 cycode-0.2.6.dev8/cycode/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cli/auth/__init__.py
--rw-r--r--   0        0        0     2777 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cli/auth/auth_command.py
--rw-r--r--   0        0        0     4742 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cli/auth/auth_manager.py
--rw-r--r--   0        0        0     1560 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cli/ci_integrations.py
--rw-r--r--   0        0        0    53335 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cli/code_scanner.py
--rw-r--r--   0        0        0      466 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cli/config.py
--rw-r--r--   0        0        0      387 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cli/config.yaml
--rw-r--r--   0        0        0     5705 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cli/consts.py
--rw-r--r--   0        0        0        0 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cli/exceptions/__init__.py
--rw-r--r--   0        0        0     1717 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cli/exceptions/custom_exceptions.py
--rw-r--r--   0        0        0        0 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cli/helpers/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cli/helpers/maven/__init__.py
--rw-r--r--   0        0        0     2041 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cli/helpers/maven/base_restore_maven_dependencies.py
--rw-r--r--   0        0        0      975 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cli/helpers/maven/restore_gradle_dependencies.py
--rw-r--r--   0        0        0     2888 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cli/helpers/maven/restore_maven_dependencies.py
--rw-r--r--   0        0        0     5626 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cli/helpers/sca_code_scanner.py
--rw-r--r--   0        0        0     7940 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cli/main.py
--rw-r--r--   0        0        0     1554 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cli/models.py
--rw-r--r--   0        0        0       93 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cli/printers/__init__.py
--rw-r--r--   0        0        0      700 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cli/printers/base_printer.py
--rw-r--r--   0        0        0     1378 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cli/printers/base_table_printer.py
--rw-r--r--   0        0        0     1963 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cli/printers/console_printer.py
--rw-r--r--   0        0        0     1603 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cli/printers/json_printer.py
--rw-r--r--   0        0        0     5809 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cli/printers/sca_table_printer.py
--rw-r--r--   0        0        0     2266 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cli/printers/table.py
--rw-r--r--   0        0        0      477 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cli/printers/table_models.py
--rw-r--r--   0        0        0     5409 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cli/printers/table_printer.py
--rw-r--r--   0        0        0     9539 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cli/printers/text_printer.py
--rw-r--r--   0        0        0        0 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cli/user_settings/__init__.py
--rw-r--r--   0        0        0      533 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cli/user_settings/base_file_manager.py
--rw-r--r--   0        0        0     4485 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cli/user_settings/config_file_manager.py
--rw-r--r--   0        0        0     7054 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cli/user_settings/configuration_manager.py
--rw-r--r--   0        0        0     1862 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cli/user_settings/credentials_manager.py
--rw-r--r--   0        0        0     6548 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cli/user_settings/user_settings_commands.py
--rw-r--r--   0        0        0        0 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cli/utils/__init__.py
--rw-r--r--   0        0        0      154 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cli/utils/enum_utils.py
--rw-r--r--   0        0        0     2170 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cli/utils/path_utils.py
--rw-r--r--   0        0        0     7572 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cli/utils/progress_bar.py
--rw-r--r--   0        0        0     2751 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cli/utils/scan_batch.py
--rw-r--r--   0        0        0      334 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cli/utils/scan_utils.py
--rw-r--r--   0        0        0      970 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cli/utils/shell_executor.py
--rw-r--r--   0        0        0     2004 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cli/utils/string_utils.py
--rw-r--r--   0        0        0     2684 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cli/utils/task_timer.py
--rw-r--r--   0        0        0      816 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cli/utils/yaml_utils.py
--rw-r--r--   0        0        0      930 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cli/zip_file.py
--rw-r--r--   0        0        0       56 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cyclient/__init__.py
--rw-r--r--   0        0        0     1709 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cyclient/auth_client.py
--rw-r--r--   0        0        0     2543 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cyclient/config.py
--rw-r--r--   0        0        0      126 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cyclient/config.yaml
--rw-r--r--   0        0        0      120 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cyclient/config_dev.py
--rw-r--r--   0        0        0      220 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cyclient/cycode_client.py
--rw-r--r--   0        0        0     3757 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cyclient/cycode_client_base.py
--rw-r--r--   0        0        0      581 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cyclient/cycode_dev_based_client.py
--rw-r--r--   0        0        0     1788 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cyclient/cycode_token_based_client.py
--rw-r--r--   0        0        0     9412 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cyclient/models.py
--rw-r--r--   0        0        0     6400 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cyclient/scan_client.py
--rw-r--r--   0        0        0        0 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cyclient/scan_config/__init__.py
--rw-r--r--   0        0        0     1165 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cyclient/scan_config/scan_config_base.py
--rw-r--r--   0        0        0     1241 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cyclient/scan_config/scan_config_creator.py
--rw-r--r--   0        0        0      199 2023-07-05 14:26:43.325436 cycode-0.2.6.dev8/cycode/cyclient/utils.py
--rw-r--r--   0        0        0     3137 2023-07-05 14:27:13.841938 cycode-0.2.6.dev8/pyproject.toml
--rw-r--r--   0        0        0    34044 1970-01-01 00:00:00.000000 cycode-0.2.6.dev8/PKG-INFO
+-rw-r--r--   0        0        0    32549 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/README.md
+-rw-r--r--   0        0        0      760 2023-07-06 08:23:21.437194 cycode-0.2.6.dev9/cycode/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/auth/__init__.py
+-rw-r--r--   0        0        0     2777 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/auth/auth_command.py
+-rw-r--r--   0        0        0     4742 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/auth/auth_manager.py
+-rw-r--r--   0        0        0     1560 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/ci_integrations.py
+-rw-r--r--   0        0        0    53335 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/code_scanner.py
+-rw-r--r--   0        0        0      466 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/config.py
+-rw-r--r--   0        0        0      387 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/config.yaml
+-rw-r--r--   0        0        0     5705 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/consts.py
+-rw-r--r--   0        0        0        0 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/exceptions/__init__.py
+-rw-r--r--   0        0        0     1717 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/exceptions/custom_exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/helpers/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/helpers/maven/__init__.py
+-rw-r--r--   0        0        0     2041 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/helpers/maven/base_restore_maven_dependencies.py
+-rw-r--r--   0        0        0      975 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/helpers/maven/restore_gradle_dependencies.py
+-rw-r--r--   0        0        0     2888 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/helpers/maven/restore_maven_dependencies.py
+-rw-r--r--   0        0        0     5626 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/helpers/sca_code_scanner.py
+-rw-r--r--   0        0        0     7940 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/main.py
+-rw-r--r--   0        0        0     1554 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/models.py
+-rw-r--r--   0        0        0       93 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/printers/__init__.py
+-rw-r--r--   0        0        0      700 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/printers/base_printer.py
+-rw-r--r--   0        0        0     1378 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/printers/base_table_printer.py
+-rw-r--r--   0        0        0     1963 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/printers/console_printer.py
+-rw-r--r--   0        0        0     1603 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/printers/json_printer.py
+-rw-r--r--   0        0        0     5809 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/printers/sca_table_printer.py
+-rw-r--r--   0        0        0     2266 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/printers/table.py
+-rw-r--r--   0        0        0      477 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/printers/table_models.py
+-rw-r--r--   0        0        0     5409 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/printers/table_printer.py
+-rw-r--r--   0        0        0     9539 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/printers/text_printer.py
+-rw-r--r--   0        0        0        0 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/user_settings/__init__.py
+-rw-r--r--   0        0        0      533 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/user_settings/base_file_manager.py
+-rw-r--r--   0        0        0     4485 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/user_settings/config_file_manager.py
+-rw-r--r--   0        0        0     7054 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/user_settings/configuration_manager.py
+-rw-r--r--   0        0        0     1862 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/user_settings/credentials_manager.py
+-rw-r--r--   0        0        0     6548 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/user_settings/user_settings_commands.py
+-rw-r--r--   0        0        0        0 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/utils/__init__.py
+-rw-r--r--   0        0        0      154 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/utils/enum_utils.py
+-rw-r--r--   0        0        0     2170 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/utils/path_utils.py
+-rw-r--r--   0        0        0     7572 2023-07-06 08:22:35.484955 cycode-0.2.6.dev9/cycode/cli/utils/progress_bar.py
+-rw-r--r--   0        0        0     2751 2023-07-06 08:22:35.488955 cycode-0.2.6.dev9/cycode/cli/utils/scan_batch.py
+-rw-r--r--   0        0        0      334 2023-07-06 08:22:35.488955 cycode-0.2.6.dev9/cycode/cli/utils/scan_utils.py
+-rw-r--r--   0        0        0      970 2023-07-06 08:22:35.488955 cycode-0.2.6.dev9/cycode/cli/utils/shell_executor.py
+-rw-r--r--   0        0        0     2004 2023-07-06 08:22:35.488955 cycode-0.2.6.dev9/cycode/cli/utils/string_utils.py
+-rw-r--r--   0        0        0     2684 2023-07-06 08:22:35.488955 cycode-0.2.6.dev9/cycode/cli/utils/task_timer.py
+-rw-r--r--   0        0        0      816 2023-07-06 08:22:35.488955 cycode-0.2.6.dev9/cycode/cli/utils/yaml_utils.py
+-rw-r--r--   0        0        0      930 2023-07-06 08:22:35.488955 cycode-0.2.6.dev9/cycode/cli/zip_file.py
+-rw-r--r--   0        0        0       56 2023-07-06 08:22:35.488955 cycode-0.2.6.dev9/cycode/cyclient/__init__.py
+-rw-r--r--   0        0        0     1709 2023-07-06 08:22:35.488955 cycode-0.2.6.dev9/cycode/cyclient/auth_client.py
+-rw-r--r--   0        0        0     2543 2023-07-06 08:22:35.488955 cycode-0.2.6.dev9/cycode/cyclient/config.py
+-rw-r--r--   0        0        0      126 2023-07-06 08:22:35.488955 cycode-0.2.6.dev9/cycode/cyclient/config.yaml
+-rw-r--r--   0        0        0      120 2023-07-06 08:22:35.488955 cycode-0.2.6.dev9/cycode/cyclient/config_dev.py
+-rw-r--r--   0        0        0      220 2023-07-06 08:22:35.488955 cycode-0.2.6.dev9/cycode/cyclient/cycode_client.py
+-rw-r--r--   0        0        0     3757 2023-07-06 08:22:35.488955 cycode-0.2.6.dev9/cycode/cyclient/cycode_client_base.py
+-rw-r--r--   0        0        0      581 2023-07-06 08:22:35.488955 cycode-0.2.6.dev9/cycode/cyclient/cycode_dev_based_client.py
+-rw-r--r--   0        0        0     1788 2023-07-06 08:22:35.488955 cycode-0.2.6.dev9/cycode/cyclient/cycode_token_based_client.py
+-rw-r--r--   0        0        0     9412 2023-07-06 08:22:35.488955 cycode-0.2.6.dev9/cycode/cyclient/models.py
+-rw-r--r--   0        0        0     6400 2023-07-06 08:22:35.488955 cycode-0.2.6.dev9/cycode/cyclient/scan_client.py
+-rw-r--r--   0        0        0        0 2023-07-06 08:22:35.488955 cycode-0.2.6.dev9/cycode/cyclient/scan_config/__init__.py
+-rw-r--r--   0        0        0     1165 2023-07-06 08:22:35.488955 cycode-0.2.6.dev9/cycode/cyclient/scan_config/scan_config_base.py
+-rw-r--r--   0        0        0     1241 2023-07-06 08:22:35.488955 cycode-0.2.6.dev9/cycode/cyclient/scan_config/scan_config_creator.py
+-rw-r--r--   0        0        0      199 2023-07-06 08:22:35.488955 cycode-0.2.6.dev9/cycode/cyclient/utils.py
+-rw-r--r--   0        0        0       16 2023-07-06 08:22:35.488955 cycode-0.2.6.dev9/cycode/pre-commit-hook-version
+-rw-r--r--   0        0        0     3138 2023-07-06 08:23:21.433194 cycode-0.2.6.dev9/pyproject.toml
+-rw-r--r--   0        0        0    34044 1970-01-01 00:00:00.000000 cycode-0.2.6.dev9/PKG-INFO
```

### Comparing `cycode-0.2.6.dev8/README.md` & `cycode-0.2.6.dev9/README.md`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev8/cycode/cli/auth/auth_command.py` & `cycode-0.2.6.dev9/cycode/cli/auth/auth_command.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev8/cycode/cli/auth/auth_manager.py` & `cycode-0.2.6.dev9/cycode/cli/auth/auth_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev8/cycode/cli/ci_integrations.py` & `cycode-0.2.6.dev9/cycode/cli/ci_integrations.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev8/cycode/cli/code_scanner.py` & `cycode-0.2.6.dev9/cycode/cli/code_scanner.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev8/cycode/cli/consts.py` & `cycode-0.2.6.dev9/cycode/cli/consts.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev8/cycode/cli/exceptions/custom_exceptions.py` & `cycode-0.2.6.dev9/cycode/cli/exceptions/custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev8/cycode/cli/helpers/maven/base_restore_maven_dependencies.py` & `cycode-0.2.6.dev9/cycode/cli/helpers/maven/base_restore_maven_dependencies.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev8/cycode/cli/helpers/maven/restore_gradle_dependencies.py` & `cycode-0.2.6.dev9/cycode/cli/helpers/maven/restore_gradle_dependencies.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev8/cycode/cli/helpers/maven/restore_maven_dependencies.py` & `cycode-0.2.6.dev9/cycode/cli/helpers/maven/restore_maven_dependencies.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev8/cycode/cli/helpers/sca_code_scanner.py` & `cycode-0.2.6.dev9/cycode/cli/helpers/sca_code_scanner.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev8/cycode/cli/main.py` & `cycode-0.2.6.dev9/cycode/cli/main.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev8/cycode/cli/models.py` & `cycode-0.2.6.dev9/cycode/cli/models.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev8/cycode/cli/printers/base_printer.py` & `cycode-0.2.6.dev9/cycode/cli/printers/base_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev8/cycode/cli/printers/base_table_printer.py` & `cycode-0.2.6.dev9/cycode/cli/printers/base_table_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev8/cycode/cli/printers/console_printer.py` & `cycode-0.2.6.dev9/cycode/cli/printers/console_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev8/cycode/cli/printers/json_printer.py` & `cycode-0.2.6.dev9/cycode/cli/printers/json_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev8/cycode/cli/printers/sca_table_printer.py` & `cycode-0.2.6.dev9/cycode/cli/printers/sca_table_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev8/cycode/cli/printers/table.py` & `cycode-0.2.6.dev9/cycode/cli/printers/table.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev8/cycode/cli/printers/table_printer.py` & `cycode-0.2.6.dev9/cycode/cli/printers/table_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev8/cycode/cli/printers/text_printer.py` & `cycode-0.2.6.dev9/cycode/cli/printers/text_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev8/cycode/cli/user_settings/base_file_manager.py` & `cycode-0.2.6.dev9/cycode/cli/user_settings/base_file_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev8/cycode/cli/user_settings/config_file_manager.py` & `cycode-0.2.6.dev9/cycode/cli/user_settings/config_file_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev8/cycode/cli/user_settings/configuration_manager.py` & `cycode-0.2.6.dev9/cycode/cli/user_settings/configuration_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev8/cycode/cli/user_settings/credentials_manager.py` & `cycode-0.2.6.dev9/cycode/cli/user_settings/credentials_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev8/cycode/cli/user_settings/user_settings_commands.py` & `cycode-0.2.6.dev9/cycode/cli/user_settings/user_settings_commands.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev8/cycode/cli/utils/path_utils.py` & `cycode-0.2.6.dev9/cycode/cli/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev8/cycode/cli/utils/progress_bar.py` & `cycode-0.2.6.dev9/cycode/cli/utils/progress_bar.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev8/cycode/cli/utils/scan_batch.py` & `cycode-0.2.6.dev9/cycode/cli/utils/scan_batch.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev8/cycode/cli/utils/shell_executor.py` & `cycode-0.2.6.dev9/cycode/cli/utils/shell_executor.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev8/cycode/cli/utils/string_utils.py` & `cycode-0.2.6.dev9/cycode/cli/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev8/cycode/cli/utils/task_timer.py` & `cycode-0.2.6.dev9/cycode/cli/utils/task_timer.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev8/cycode/cli/utils/yaml_utils.py` & `cycode-0.2.6.dev9/cycode/cli/utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev8/cycode/cli/zip_file.py` & `cycode-0.2.6.dev9/cycode/cli/zip_file.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev8/cycode/cyclient/auth_client.py` & `cycode-0.2.6.dev9/cycode/cyclient/auth_client.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev8/cycode/cyclient/config.py` & `cycode-0.2.6.dev9/cycode/cyclient/config.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev8/cycode/cyclient/cycode_client_base.py` & `cycode-0.2.6.dev9/cycode/cyclient/cycode_client_base.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev8/cycode/cyclient/cycode_dev_based_client.py` & `cycode-0.2.6.dev9/cycode/cyclient/cycode_dev_based_client.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev8/cycode/cyclient/cycode_token_based_client.py` & `cycode-0.2.6.dev9/cycode/cyclient/cycode_token_based_client.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev8/cycode/cyclient/models.py` & `cycode-0.2.6.dev9/cycode/cyclient/models.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev8/cycode/cyclient/scan_client.py` & `cycode-0.2.6.dev9/cycode/cyclient/scan_client.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev8/cycode/cyclient/scan_config/scan_config_base.py` & `cycode-0.2.6.dev9/cycode/cyclient/scan_config/scan_config_base.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev8/cycode/cyclient/scan_config/scan_config_creator.py` & `cycode-0.2.6.dev9/cycode/cyclient/scan_config/scan_config_creator.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev8/pyproject.toml` & `cycode-0.2.6.dev9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cycode"
-version = "0.2.6.dev8" # DON'T TOUCH. Placeholder. Will be filled automatically on poetry build from Git Tag
+version = "0.2.6.dev9" # DON'T TOUCH. Placeholder. Will be filled automatically on poetry build from Git Tag
 description = "Perform secrets/iac scans for your sources using Cycode's engine"
 keywords=["secret-scan", "cycode", "devops", "token", "secret", "security", "cycode", "code"]
 authors = ["Cycode <support@cycode.com>"]
 license = "MIT"
 repository = "https://github.com/cycodehq-public/cycode-cli"
 readme = "README.md"
 classifiers = [
@@ -55,15 +55,15 @@
 
 [tool.pytest.ini_options]
 log_cli = true
 
 [tool.poetry-dynamic-versioning]
 # poetry self add "poetry-dynamic-versioning[plugin]"
 enable = false
-strict = true
+strict = false
 bump = true
 metadata = false
 vcs = "git"
 style = "pep440"
 
 [tool.black]
 line-length = 120
```

### Comparing `cycode-0.2.6.dev8/PKG-INFO` & `cycode-0.2.6.dev9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cycode
-Version: 0.2.6.dev8
+Version: 0.2.6.dev9
 Summary: Perform secrets/iac scans for your sources using Cycode's engine
 Home-page: https://github.com/cycodehq-public/cycode-cli
 License: MIT
 Keywords: secret-scan,cycode,devops,token,secret,security,cycode,code
 Author: Cycode
 Author-email: support@cycode.com
 Requires-Python: >=3.7,<3.12
```

