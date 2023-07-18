# Comparing `tmp/vantage6-3.9.0rc4.tar.gz` & `tmp/vantage6-4.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-3.9.0rc4.tar", last modified: Wed May 24 09:34:09 2023, max compression
+gzip compressed data, was "vantage6-4.0.0a2.tar", last modified: Tue Jul 18 13:32:08 2023, max compression
```

## Comparing `vantage6-3.9.0rc4.tar` & `vantage6-4.0.0a2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:09.521727 vantage6-3.9.0rc4/
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-05-24 09:34:09.521727 vantage6-3.9.0rc4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 09:34:09.521727 vantage6-3.9.0rc4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-24 09:33:56.000000 vantage6-3.9.0rc4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:09.517727 vantage6-3.9.0rc4/tests_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 09:33:56.000000 vantage6-3.9.0rc4/tests_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-24 09:33:56.000000 vantage6-3.9.0rc4/tests_cli/test_example.py
--rw-r--r--   0 runner    (1001) docker     (123)    14861 2023-05-24 09:33:56.000000 vantage6-3.9.0rc4/tests_cli/test_node_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-05-24 09:33:56.000000 vantage6-3.9.0rc4/tests_cli/test_server_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-05-24 09:33:56.000000 vantage6-3.9.0rc4/tests_cli/test_wizard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:09.517727 vantage6-3.9.0rc4/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:09.521727 vantage6-3.9.0rc4/vantage6/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 09:33:56.000000 vantage6-3.9.0rc4/vantage6/cli/__build__
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-24 09:33:56.000000 vantage6-3.9.0rc4/vantage6/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-24 09:33:56.000000 vantage6-3.9.0rc4/vantage6/cli/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-05-24 09:33:56.000000 vantage6-3.9.0rc4/vantage6/cli/configuration_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    10459 2023-05-24 09:33:56.000000 vantage6-3.9.0rc4/vantage6/cli/configuration_wizard.py
--rw-r--r--   0 runner    (1001) docker     (123)    14510 2023-05-24 09:33:56.000000 vantage6-3.9.0rc4/vantage6/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-24 09:33:56.000000 vantage6-3.9.0rc4/vantage6/cli/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)    37859 2023-05-24 09:33:56.000000 vantage6-3.9.0rc4/vantage6/cli/node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:09.521727 vantage6-3.9.0rc4/vantage6/cli/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-24 09:33:56.000000 vantage6-3.9.0rc4/vantage6/cli/rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-24 09:33:56.000000 vantage6-3.9.0rc4/vantage6/cli/rabbitmq/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-05-24 09:33:56.000000 vantage6-3.9.0rc4/vantage6/cli/rabbitmq/queue_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-24 09:33:56.000000 vantage6-3.9.0rc4/vantage6/cli/rabbitmq/rabbitmq.config
--rw-r--r--   0 runner    (1001) docker     (123)    29887 2023-05-24 09:33:56.000000 vantage6-3.9.0rc4/vantage6/cli/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-24 09:33:56.000000 vantage6-3.9.0rc4/vantage6/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:09.517727 vantage6-3.9.0rc4/vantage6.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-05-24 09:34:09.000000 vantage6-3.9.0rc4/vantage6.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-24 09:34:09.000000 vantage6-3.9.0rc4/vantage6.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 09:34:09.000000 vantage6-3.9.0rc4/vantage6.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-24 09:34:09.000000 vantage6-3.9.0rc4/vantage6.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-24 09:34:09.000000 vantage6-3.9.0rc4/vantage6.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-24 09:34:09.000000 vantage6-3.9.0rc4/vantage6.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:32:08.560677 vantage6-4.0.0a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-07-18 13:32:08.560677 vantage6-4.0.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 13:32:08.560677 vantage6-4.0.0a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-18 13:31:55.000000 vantage6-4.0.0a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:32:08.556677 vantage6-4.0.0a2/tests_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:31:55.000000 vantage6-4.0.0a2/tests_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-18 13:31:55.000000 vantage6-4.0.0a2/tests_cli/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14574 2023-07-18 13:31:55.000000 vantage6-4.0.0a2/tests_cli/test_node_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-07-18 13:31:55.000000 vantage6-4.0.0a2/tests_cli/test_server_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-07-18 13:31:55.000000 vantage6-4.0.0a2/tests_cli/test_wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:32:08.556677 vantage6-4.0.0a2/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:32:08.560677 vantage6-4.0.0a2/vantage6/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 13:31:55.000000 vantage6-4.0.0a2/vantage6/cli/__build__
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-18 13:31:55.000000 vantage6-4.0.0a2/vantage6/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-18 13:31:55.000000 vantage6-4.0.0a2/vantage6/cli/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-18 13:31:55.000000 vantage6-4.0.0a2/vantage6/cli/configuration_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11327 2023-07-18 13:31:55.000000 vantage6-4.0.0a2/vantage6/cli/configuration_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13262 2023-07-18 13:31:55.000000 vantage6-4.0.0a2/vantage6/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-18 13:31:55.000000 vantage6-4.0.0a2/vantage6/cli/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33998 2023-07-18 13:31:55.000000 vantage6-4.0.0a2/vantage6/cli/node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:32:08.560677 vantage6-4.0.0a2/vantage6/cli/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-18 13:31:55.000000 vantage6-4.0.0a2/vantage6/cli/rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-18 13:31:55.000000 vantage6-4.0.0a2/vantage6/cli/rabbitmq/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-07-18 13:31:55.000000 vantage6-4.0.0a2/vantage6/cli/rabbitmq/queue_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-18 13:31:55.000000 vantage6-4.0.0a2/vantage6/cli/rabbitmq/rabbitmq.config
+-rw-r--r--   0 runner    (1001) docker     (123)    28331 2023-07-18 13:31:55.000000 vantage6-4.0.0a2/vantage6/cli/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-18 13:31:55.000000 vantage6-4.0.0a2/vantage6/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:32:08.556677 vantage6-4.0.0a2/vantage6.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-07-18 13:32:08.000000 vantage6-4.0.0a2/vantage6.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-18 13:32:08.000000 vantage6-4.0.0a2/vantage6.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 13:32:08.000000 vantage6-4.0.0a2/vantage6.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-18 13:32:08.000000 vantage6-4.0.0a2/vantage6.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-18 13:32:08.000000 vantage6-4.0.0a2/vantage6.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-18 13:32:08.000000 vantage6-4.0.0a2/vantage6.egg-info/top_level.txt
```

### Comparing `vantage6-3.9.0rc4/PKG-INFO` & `vantage6-4.0.0a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6
-Version: 3.9.0rc4
+Version: 4.0.0a2
 Summary: vantage6 command line interface
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,11 +1,10 @@
-Metadata-Version: 2.1 Name: vantage6 Version: 3.9.0rc4 Summary: vantage6
-command line interface Home-page: https://github.com/vantage6/vantage6
-Requires-Python: >=3.6 Description-Content-Type: text/markdown Provides-Extra:
-dev
+Metadata-Version: 2.1 Name: vantage6 Version: 4.0.0a2 Summary: vantage6 command
+line interface Home-page: https://github.com/vantage6/vantage6 Requires-Python:
+>=3.6 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml) [![PyPI vantage6](https://badge.fury.io/py/vantage6.svg)](https://
 badge.fury.io/py/vantage6) [![Unittests](https://github.com/vantage6/vantage6/
```

### Comparing `vantage6-3.9.0rc4/setup.py` & `vantage6-4.0.0a2/setup.py`

 * *Files identical despite different names*

### Comparing `vantage6-3.9.0rc4/tests_cli/test_node_cli.py` & `vantage6-4.0.0a2/tests_cli/test_node_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         # docker deamon returns a list of running node-containers
         container1 = MagicMock()
         container1.name = f"{APPNAME}-iknl-user"
         containers.list.return_value = [container1]
 
         # returns a list of configurations and failed inports
         def side_effect(system_folders):
-            config = MagicMock(available_environments=["Application"])
+            config = MagicMock()
             config.name = "iknl"
             if not system_folders:
                 return [[config], []]
             else:
                 return [[config], []]
 
         available_configurations.side_effect = side_effect
@@ -74,34 +74,33 @@
 
         # validate exit code
         self.assertEqual(result.exit_code, 0)
 
         # check printed lines
         self.assertEqual(
             result.output,
-            "\nName                     Environments                    Status          System/User\n"
-            "-------------------------------------------------------------------------------------\n"
-            "iknl                     ['Application']                 Offline          System \n"
-            "iknl                     ['Application']                 Online           User   \n"
-            "-------------------------------------------------------------------------------------\n"
+            "\nName                     Status          System/User\n"
+            "-----------------------------------------------------\n"
+            "iknl                     Offline         System \n"
+            "iknl                     Online          User   \n"
+            "-----------------------------------------------------\n"
         )
 
     @patch("vantage6.cli.node.configuration_wizard")
     @patch("vantage6.cli.node.check_config_writeable")
     @patch("vantage6.cli.node.NodeContext")
     def test_new_config(self, context, permissions, wizard):
         """No error produced when creating new configuration."""
         context.config_exists.return_value = False
         permissions.return_value = True
         wizard.return_value = "/some/file/path"
 
         runner = CliRunner()
         result = runner.invoke(cli_node_new_configuration, [
             "--name", "some-name",
-            "--environment", "application"
         ])
 
         # check that info message is produced
         self.assertEqual(result.output[:7], "[info ]")
 
         # check OK exit code
         self.assertEqual(result.exit_code, 0)
@@ -109,15 +108,14 @@
     @patch("vantage6.cli.node.configuration_wizard")
     def test_new_config_replace_whitespace_in_name(self, _):
         """Whitespaces are replaced in the name."""
 
         runner = CliRunner()
         result = runner.invoke(cli_node_new_configuration, [
             "--name", "some name",
-            "--environment", "application"
         ])
 
         self.assertEqual(
             result.output[:60],
             "[info ] - Replaced spaces from configuration name: some-name"
         )
 
@@ -126,15 +124,14 @@
         """No duplicate configurations are allowed."""
 
         context.config_exists.return_value = True
 
         runner = CliRunner()
         result = runner.invoke(cli_node_new_configuration, [
             "--name", "some-name",
-            "--environment", "application"
         ])
 
         # check that error is produced
         self.assertEqual(result.output[:7], "[error]")
 
         # check non-zero exit code
         self.assertEqual(result.exit_code, 1)
@@ -146,15 +143,14 @@
 
         context.config_exists.return_value = False
         permissions.return_value = False
 
         runner = CliRunner()
         result = runner.invoke(cli_node_new_configuration, [
             "--name", "some-name",
-            "--environment", "application"
         ])
 
         # check that error is produced
         self.assertEqual(result.output[:7], "[error]")
 
         # check non-zero exit code
         self.assertEqual(result.exit_code, 1)
@@ -168,15 +164,15 @@
         context.return_value = MagicMock(
             config_file="/file.yaml",
             log_file="/log.log",
             data_dir="/dir"
         )
         context.return_value.databases.items.return_value = \
             [["label", "/file.db"]]
-        select_config.return_value = ["iknl", "application"]
+        select_config.return_value = "iknl"
 
         runner = CliRunner()
         result = runner.invoke(cli_node_files, [])
 
         # we check that no warnings have been produced
         self.assertEqual(result.output[:7], "[info ]")
 
@@ -212,15 +208,19 @@
         volumes.create.return_value = volume
         context.config_exists.return_value = True
 
         ctx = MagicMock(
             data_dir=Path("data"),
             log_dir=Path("logs"),
             config_dir=Path("configs"),
-            databases={"default": "data.csv"}
+            databases=[{
+                "label": "some-label",
+                "uri": "data.csv",
+                "type": "csv"
+            }]
         )
         ctx.get_data_file.return_value = "data.csv"
         ctx.name = 'some-name'
         context.return_value = ctx
 
         runner = CliRunner()
 
@@ -388,15 +388,15 @@
             _print_log_worker(stream)
         output = temp_stdout.getvalue().strip()
         self.assertEqual(output, "Hello!")
 
     @patch("vantage6.cli.node.info")
     @patch("vantage6.cli.node.debug")
     @patch("vantage6.cli.node.error")
-    @patch("vantage6.cli.node.Client")
+    @patch("vantage6.cli.node.UserClient")
     @patch("vantage6.cli.node.q")
     def test_client(self, q, client, error, debug, info):
 
         ctx = MagicMock(
             config={
                 "server_url": "localhost",
                 "port": 5000,
```

### Comparing `vantage6-3.9.0rc4/tests_cli/test_server_cli.py` & `vantage6-4.0.0a2/tests_cli/test_server_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     @patch("vantage6.cli.server.check_docker_running", return_value=True)
     def test_configuration_list(self, docker_check, containers, context):
         """Configuration list without errors."""
         container1 = MagicMock()
         container1.name = f"{APPNAME}-iknl-system"
         containers.list.return_value = [container1]
 
-        config = MagicMock(available_environments=["application"])
+        config = MagicMock()
         config.name = "iknl"
         context.available_configurations.return_value = ([config], [])
 
         runner = CliRunner()
         result = runner.invoke(cli_server_configuration_list)
 
         self.assertEqual(result.exit_code, 0)
```

### Comparing `vantage6-3.9.0rc4/tests_cli/test_wizard.py` & `vantage6-4.0.0a2/tests_cli/test_wizard.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,15 +30,22 @@
         return result
 
     def test_node_wizard(self):
         """An error is printed when docker is not running"""
 
         with patch(f"{module_path}.q") as q:
             q.prompt.side_effect = self.prompts
-            q.confirm.return_value.ask.side_effect = [True, False, True, True]
+            q.confirm.return_value.ask.side_effect = [
+                True,  # add a database
+                False,  # don't enable two-factor authentication
+                True,  # add VPN server
+                False,  # don't abort if no server connection is made to pull
+                        # collaboration settings
+                True  # Enable encryption
+            ]
             dirs = MagicMock(data="/")
             config = node_configuration_questionaire(dirs, "iknl")
 
         keys = ["api_key", "server_url", "port", "api_path", "task_dir",
                 "databases", "logging", "encryption", "vpn_subnet"]
         for key in keys:
             self.assertIn(key, config)
@@ -65,30 +72,28 @@
     @patch(f"{module_path}.NodeContext")
     def test_configuration_wizard_interface(self, context, node_m, server_m,
                                             server_q, node_q):
         context.instance_folders.return_value = {
             "config": "/some/path/"
         }
 
-        file_ = configuration_wizard("node", "vtg6", "application", False)
+        file_ = configuration_wizard("node", "vtg6", False)
         self.assertEqual(Path("/some/path/vtg6.yaml"), file_)
 
-        file_ = configuration_wizard("server", "vtg6", "application", True)
+        file_ = configuration_wizard("server", "vtg6", True)
         self.assertEqual(Path("/some/path/vtg6.yaml"), file_)
 
     @patch(f"{module_path}.NodeContext")
     @patch(f"{module_path}.ServerContext")
     def test_select_configuration(self, server_c, node_c):
 
         config = MagicMock()
         config.name = "vtg6"
-        config.available_environments = ["application"]
 
         server_c.available_configurations.return_value = [[config], []]
         node_c.available_configurations.return_value = [[config], []]
 
         with patch(f"{module_path}.q") as q:
-            q.select.return_value.ask.return_value = ["vtg6", "application"]
-            name, env = select_configuration_questionaire("node", True)
+            q.select.return_value.ask.return_value = "vtg6"
+            name = select_configuration_questionaire("node", True)
 
         self.assertEqual(name, "vtg6")
-        self.assertEqual(env, "application")
```

### Comparing `vantage6-3.9.0rc4/vantage6/cli/_version.py` & `vantage6-4.0.0a2/vantage6/cli/_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(here, '__build__')) as fp:
     __build__ = json.load(fp)
 
 # Module version
-version_info = (3, 9, 0, 'candidate', __build__, 0)
+version_info = (4, 0, 0, 'alpha', __build__, 0)
 
 # Module version stage suffix map
 _specifier_ = {'alpha': 'a', 'beta': 'b', 'candidate': 'rc', 'final': ''}
 version = f'{version_info[0]}.{version_info[1]}.{version_info[2]}'
 pre_release = '' if version_info[3] == 'final' else \
   '.'+_specifier_[version_info[3]]+str(version_info[4])
 post_release = '' if not version_info[5] else f'.post{version_info[5]}'
```

### Comparing `vantage6-3.9.0rc4/vantage6/cli/configuration_manager.py` & `vantage6-4.0.0a2/vantage6/cli/configuration_manager.py`

 * *Files identical despite different names*

### Comparing `vantage6-3.9.0rc4/vantage6/cli/configuration_wizard.py` & `vantage6-4.0.0a2/vantage6/cli/configuration_wizard.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import questionary as q
 import uuid
 
 from pathlib import Path
 
 from vantage6.common.globals import DATABASE_TYPES
+from vantage6.common.client.node_client import NodeClient
+from vantage6.common import error, warning
 from vantage6.cli.context import NodeContext, ServerContext
 from vantage6.cli.configuration_manager import (
     NodeConfigurationManager,
     ServerConfigurationManager
 )
 
 
@@ -110,15 +112,36 @@
             {"name": "requests", "level": "warning"},
             {"name": "engineio.client", "level": "warning"},
             {"name": "docker.utils.config", "level": "warning"},
             {"name": "docker.auth", "level": "warning"},
         ]
     }
 
-    encryption = q.confirm("Enable encryption?", default=True).ask()
+    # Check if we can login to the server to retrieve collaboration settings
+    client = NodeClient(config['server_url'], config['port'],
+                        config['api_path'])
+    try:
+        client.authenticate(config['api_key'])
+    except Exception as e:
+        error(f"Could not authenticate with server: {e}")
+        error("Please check (1) your API key and (2) if your server is online")
+        warning("If you continue, you should provide your collaboration "
+                "settings manually.")
+        if q.confirm("Do you want to abort?", default=True).ask():
+            exit(0)
+
+    if client.whoami is not None:
+        encryption = client.is_encrypted_collaboration()
+        # TODO when we build collaboration policies, update this to provide
+        # the node admin with a list of all policies, and whether or not
+        # to accept them
+        q.confirm(f"Encryption is {'enabled' if encryption else 'disabled'}"
+                  f" for this collaboration. Accept?", default=True).ask()
+    else:
+        encryption = q.confirm("Enable encryption?", default=True).ask()
 
     private_key = "" if not encryption else \
         q.text("Path to private key file:").ask()
 
     config["encryption"] = {
         "enabled": encryption == "true",
         "private_key": private_key
@@ -257,27 +280,25 @@
             {"name": "requests_oauthlib.oauth2_session", "level": "warning"},
         ]
     }
 
     return config
 
 
-def configuration_wizard(type_: str, instance_name: str, environment: str,
+def configuration_wizard(type_: str, instance_name: str,
                          system_folders: bool) -> Path:
     """
     Create a configuration file for a node or server instance.
 
     Parameters
     ----------
     type_ : str
         Type of the instance. Either "node" or "server"
     instance_name : str
         Name of the instance
-    environment : str
-        Name of the environment
     system_folders : bool
         Whether to use the system folders or not
 
     Returns
     -------
     Path
         Path to the configuration file
@@ -299,53 +320,48 @@
     config_file = Path(dirs.get("config")) / (instance_name + ".yaml")
 
     if Path(config_file).exists():
         config_manager = conf_manager.from_file(config_file)
     else:
         config_manager = conf_manager(instance_name)
 
-    config_manager.put(environment, config)
+    config_manager.put(config)
     config_manager.save(config_file)
 
     return config_file
 
 
-def select_configuration_questionaire(
-        type_: str, system_folders: bool) -> tuple[str, str]:
+def select_configuration_questionaire(type_: str, system_folders: bool) -> str:
     """
     Ask which configuration the user wants to use. It shows only configurations
     that are in the default folder.
 
     Parameters
     ----------
     type_ : str
         Type of the instance. Either "node" or "server"
     system_folders : bool
         Whether to use the system folders or not
 
     Returns
     -------
-    tuple[str, str]
-        Name of the configuration and the environment
+    str
+        Name of the configuration
     """
     context = NodeContext if type_ == "node" else ServerContext
-    configs, f = context.available_configurations(system_folders)
+    configs, _ = context.available_configurations(system_folders)
 
     # each collection (file) can contain multiple configs. (e.g. test,
     # dev)
     choices = []
     for config_collection in configs:
-
-        envs = config_collection.available_environments
-        for env in envs:
-            choices.append(q.Choice(
-                title=f"{config_collection.name:25} {env}",
-                value=(config_collection.name, env)))
+        choices.append(q.Choice(
+            title=f"{config_collection.name:25}",
+            value=config_collection.name
+        ))
 
     if not choices:
         raise Exception("No configurations could be found!")
 
     # pop the question
-    name, env = q.select("Select the configuration you want to use:",
-                         choices=choices).ask()
-
-    return name, env
+    return q.select("Select the configuration you want to use:",
+                    choices=choices).ask()
```

### Comparing `vantage6-3.9.0rc4/vantage6/cli/context.py` & `vantage6-4.0.0a2/vantage6/cli/context.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,44 +29,40 @@
 
 from sqlalchemy.engine.url import make_url
 
 from vantage6.common.context import AppContext
 from vantage6.common.globals import APPNAME
 from vantage6.cli.configuration_manager import (NodeConfigurationManager,
                                                 ServerConfigurationManager)
-from vantage6.cli.globals import (DEFAULT_NODE_ENVIRONMENT as N_ENV,
-                                  DEFAULT_NODE_SYSTEM_FOLDERS as N_FOL,
-                                  DEFAULT_SERVER_ENVIRONMENT as S_ENV,
-                                  DEFAULT_SERVER_SYSTEM_FOLDERS as S_FOL)
+from vantage6.cli.globals import (
+    DEFAULT_NODE_SYSTEM_FOLDERS as N_FOL,
+    DEFAULT_SERVER_SYSTEM_FOLDERS as S_FOL
+)
 from vantage6.cli._version import __version__
 
 
 class ServerContext(AppContext):
     """
     Server context
 
     Parameters
     ----------
     instance_name : str
         Name of the configuration instance, corresponds to the filename
         of the configuration file.
-    environment : str, optional
-        DTAP environment to load from the configuration file, by default
-        S_ENV
     system_folders : bool, optional
         System wide or user configuration, by default S_FOL
     """
 
     # The server configuration manager is aware of the structure of the server
     # configuration file and makes sure only valid configuration can be loaded.
     INST_CONFIG_MANAGER = ServerConfigurationManager
 
-    def __init__(self, instance_name: str, environment: str = S_ENV,
-                 system_folders: bool = S_FOL):
-        super().__init__("server", instance_name, environment=environment,
+    def __init__(self, instance_name: str, system_folders: bool = S_FOL):
+        super().__init__("server", instance_name,
                          system_folders=system_folders)
         self.log.info(f"vantage6 version '{__version__}'")
 
     def get_database_uri(self) -> str:
         """
         Obtain the database uri from the environment or the configuration. The
         `VANTAGE6_DB_URI` environment variable is used by the Docker container,
@@ -105,67 +101,59 @@
         str
             Server's docker container name
         """
         return f"{APPNAME}-{self.name}-{self.scope}-server"
 
     @classmethod
     def from_external_config_file(
-            cls, path: str, environment: str = S_ENV,
-            system_folders: bool = S_FOL) -> ServerContext:
+            cls, path: str, system_folders: bool = S_FOL) -> ServerContext:
         """
         Create a server context from an external configuration file. External
         means that the configuration file is not located in the default folders
         but its location is specified by the user.
 
         Parameters
         ----------
         path : str
             Path of the configuration file
-        environment : str, optional
-            DTAP environment to be loaded, by default S_ENV
         system_folders : bool, optional
             System wide or user configuration, by default S_FOL
 
         Returns
         -------
         ServerContext
             Server context object
         """
-        cls = super().from_external_config_file(
-            path, "server", environment, system_folders
-        )
+        cls = super().from_external_config_file(path, "server", system_folders)
         # if we are running a server in a docker container, the name is taken
         # from the name of the config file (which is usually a default). Get
         # the config name from environment if it is given.
         cls.name = os.environ.get("VANTAGE6_CONFIG_NAME") or cls.name
         return cls
 
     @classmethod
-    def config_exists(cls, instance_name: str, environment: str = S_ENV,
+    def config_exists(cls, instance_name: str,
                       system_folders: bool = S_FOL) -> bool:
         """
         Check if a configuration file exists.
 
         Parameters
         ----------
         instance_name : str
             Name of the configuration instance, corresponds to the filename
             of the configuration file.
-        environment : str, optional
-            DTAP environment that needs to be present, by default S_ENV
         system_folders : bool, optional
             System wide or user configuration, by default S_FOL
 
         Returns
         -------
         bool
             Whether the configuration file exists or not
         """
         return super().config_exists("server", instance_name,
-                                     environment=environment,
                                      system_folders=system_folders)
 
     @classmethod
     def available_configurations(cls, system_folders: bool = S_FOL) \
             -> tuple[list, list]:
         """
         Find all available server configurations in the default folders.
@@ -192,84 +180,75 @@
     dockerized service.
 
     Parameters
     ----------
     instance_name : str
         Name of the configuration instance, corresponds to the filename
         of the configuration file.
-    environment : str, optional
-        DTAP environment to be loaded, by default N_ENV
     system_folders : bool, optional
         _description_, by default N_FOL
     config_file : str, optional
         _description_, by default None
     """
 
     # The server configuration manager is aware of the structure of the server
     # configuration file and makes sure only valid configuration can be loaded.
     INST_CONFIG_MANAGER = NodeConfigurationManager
 
     # Flag to indicate if the node is running in a docker container or directly
     # on the host machine.
     running_in_docker = False
 
-    def __init__(self, instance_name: str, environment: str = N_ENV,
-                 system_folders: bool = N_FOL, config_file: str = None):
-        super().__init__("node", instance_name, environment, system_folders,
-                         config_file)
+    def __init__(self, instance_name: str, system_folders: bool = N_FOL,
+                 config_file: str = None):
+        super().__init__("node", instance_name, system_folders, config_file)
         self.log.info(f"vantage6 version '{__version__}'")
 
     @classmethod
-    def from_external_config_file(cls, path: str, environment: str = N_ENV,
+    def from_external_config_file(cls, path: str,
                                   system_folders: bool = N_FOL) -> NodeContext:
         """
         Create a node context from an external configuration file. External
         means that the configuration file is not located in the default folders
         but its location is specified by the user.
 
         Parameters
         ----------
         path : str
             Path of the configuration file
-        environment : str, optional
-            DTAP environment to be loaded, by default N_ENV
         system_folders : bool, optional
             System wide or user configuration, by default N_FOL
 
         Returns
         -------
         NodeContext
             Node context object
         """
-        return super().from_external_config_file(path, "node", environment,
-                                                 system_folders)
+        return super().from_external_config_file(path, "node", system_folders)
 
     @classmethod
-    def config_exists(cls, instance_name: str, environment: str = N_ENV,
+    def config_exists(cls, instance_name: str,
                       system_folders: bool = N_FOL) -> bool:
         """
         Check if a configuration file exists.
 
         Parameters
         ----------
         instance_name : str
             Name of the configuration instance, corresponds to the filename
             of the configuration file.
-        environment : str, optional
-            DTAP environment that needs to be present, by default N_ENV
         system_folders : bool, optional
             System wide or user configuration, by default N_FOL
 
         Returns
         -------
         bool
             Whether the configuration file exists or not
         """
         return super().config_exists("node", instance_name,
-                                     environment=environment,
                                      system_folders=system_folders)
 
     @classmethod
     def available_configurations(cls, system_folders: bool = N_FOL) \
             -> tuple[list, list]:
         """
         Find all available server configurations in the default folders.
@@ -402,31 +381,31 @@
             f"{self.docker_container_name}-squid-vol"
         )
 
     @property
     def proxy_log_file(self):
         return self.log_file_name(type_="proxy_server")
 
-    def docker_temporary_volume_name(self, run_id: int) -> str:
+    def docker_temporary_volume_name(self, job_id: int) -> str:
         """
         Docker volume in which temporary data is stored. Temporary data is
         linked to a specific run. Multiple algorithm containers can have the
         same run id, and therefore the share same temporary volume.
 
         Parameters
         ----------
-        run_id : int
+        job_id : int
             run id provided by the server
 
         Returns
         -------
         str
             Docker volume name
         """
-        return f"{APPNAME}-{self.name}-{self.scope}-{run_id}-tmpvol"
+        return f"{APPNAME}-{self.name}-{self.scope}-{job_id}-tmpvol"
 
     def get_database_uri(self, label: str = "default") -> str:
         """
         Obtain the database URI for a specific database.
 
         Parameters
         ----------
```

### Comparing `vantage6-3.9.0rc4/vantage6/cli/globals.py` & `vantage6-4.0.0a2/vantage6/cli/globals.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,24 +5,19 @@
 from vantage6.common.globals import APPNAME
 
 #
 #   SERVER SETTINGS
 #
 DEFAULT_SERVER_SYSTEM_FOLDERS = True
 
-DEFAULT_SERVER_ENVIRONMENT = "prod"
-
 #
 #   NODE SETTINGS
 #
 DEFAULT_NODE_SYSTEM_FOLDERS = False
 
-DEFAULT_NODE_ENVIRONMENT = "application"
-
-
 #
 #   INSTALLATION SETTINGS
 #
 PACKAGE_FOLDER = Path(__file__).parent.parent.parent
 
 # FIXME BvB 22-06-28 think this is also defined in the node globals, and this
 # one appears not to be used
```

### Comparing `vantage6-3.9.0rc4/vantage6/cli/node.py` & `vantage6-4.0.0a2/vantage6/cli/node.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,19 +40,18 @@
 from vantage6.common.globals import VPN_CONFIG_FILE
 from vantage6.common.docker.addons import (
   pull_if_newer,
   remove_container_if_exists,
   check_docker_running
 )
 from vantage6.common.encryption import RSACryptor
-from vantage6.client import Client
+from vantage6.client import UserClient
 
 from vantage6.cli.context import NodeContext
 from vantage6.cli.globals import (
-    DEFAULT_NODE_ENVIRONMENT as N_ENV,
     DEFAULT_NODE_SYSTEM_FOLDERS as N_FOL
 )
 from vantage6.cli.configuration_wizard import (
     configuration_wizard,
     select_configuration_questionaire,
     NodeConfigurationManager
 )
@@ -80,15 +79,14 @@
     client = docker.from_env()
     check_docker_running()
 
     running_node_names = _find_running_node_names(client)
 
     header = \
         "\nName"+(21*" ") + \
-        "Environments"+(20*" ") + \
         "Status"+(10*" ") + \
         "System/User"
 
     click.echo(header)
     click.echo("-"*len(header))
 
     running = Fore.GREEN + "Online" + Style.RESET_ALL
@@ -98,59 +96,52 @@
     configs, f1 = NodeContext.available_configurations(
         system_folders=True)
     for config in configs:
         status = running if f"{APPNAME}-{config.name}-system" in \
             running_node_names else stopped
         click.echo(
             f"{config.name:25}"
-            f"{str(config.available_environments):32}"
-            f"{status:25} System "
+            f"{status:25}System "
         )
 
     # user folders
     configs, f2 = NodeContext.available_configurations(
         system_folders=False)
     for config in configs:
         status = running if f"{APPNAME}-{config.name}-user" in \
             running_node_names else stopped
         click.echo(
             f"{config.name:25}"
-            f"{str(config.available_environments):32}"
-            f"{status:25} User   "
+            f"{status:25}User   "
         )
 
-    click.echo("-"*85)
+    click.echo("-"*53)
     if len(f1)+len(f2):
         warning(
              f"{Fore.RED}Failed imports: {len(f1)+len(f2)}{Style.RESET_ALL}")
 
 
 #
 #   new
 #
 @cli_node.command(name="new")
 @click.option("-n", "--name", default=None)
-@click.option('-e', '--environment', default="",
-              help='configuration environment to use')
 @click.option('--system', 'system_folders', flag_value=True)
 @click.option('--user', 'system_folders', flag_value=False, default=N_FOL)
-def cli_node_new_configuration(name: str, environment: str,
-                               system_folders: bool) -> None:
+def cli_node_new_configuration(name: str, system_folders: bool) -> None:
     """
     Create a new configuration file.
 
     Checks if the configuration already exists. If this is not the case
     a questionnaire is invoked to create a new configuration file.
 
     Parameters
     ----------
     name : str
         Name of the configuration file.
-    environment : str
-        DTAP environment to use.
     system_folders : bool
         Store this configuration in the system folders or in the user folders.
     """
     # select configuration name if none supplied
     if not name:
         name = q.text("Please enter a configuration-name:").ask()
 
@@ -159,121 +150,98 @@
     if name != name_new:
         info(f"Replaced spaces from configuration name: {name_new}")
         name = name_new
 
     # check if config name is allowed docker name
     check_config_name_allowed(name)
 
-    if not environment:
-        environment = q.select(
-            "Please select the environment you want to configure:",
-            ["application", "prod", "acc", "test", "dev"]
-        ).ask()
-
     # check that this config does not exist
-    if NodeContext.config_exists(name, environment, system_folders):
-        error(
-            f"Configuration {name} and environment"
-            f"{environment} already exists!"
-        )
+    if NodeContext.config_exists(name, system_folders):
+        error(f"Configuration {name} already exists!")
         exit(1)
 
     # Check that we can write in this folder
     if not check_config_writeable(system_folders):
         error("Cannot write configuration file. Exiting...")
         exit(1)
 
     # create config in ctx location
     flag = "--system" if system_folders else ""
-    cfg_file = configuration_wizard("node", name, environment, system_folders)
+    cfg_file = configuration_wizard("node", name, system_folders)
     info(f"New configuration created: {Fore.GREEN}{cfg_file}{Style.RESET_ALL}")
     info(f"You can start the node by running "
          f"{Fore.GREEN}vnode start {flag}{Style.RESET_ALL}")
 
 
 #
 #   files
 #
 @cli_node.command(name="files")
 @click.option("-n", "--name", default=None, help="configuration name")
-@click.option('-e', '--environment', default=N_ENV,
-              help='configuration environment to use')
 @click.option('--system', 'system_folders', flag_value=True)
 @click.option('--user', 'system_folders', flag_value=False, default=N_FOL)
-def cli_node_files(name: str, environment: str, system_folders: bool) -> None:
+def cli_node_files(name: str, system_folders: bool) -> None:
     """
     Prints location important files.
 
     If the specified configuration cannot be found, it exits. Otherwise
     it returns the absolute path to the output.
 
     Parameters
     ----------
     name : str
         Name of the configuration file.
-    environment : str
-        DTAP environment to use.
     system_folders : bool
         Is this configuration stored in the system or in the user folders.
     """
-    name, environment = _select_node(name, environment, system_folders)
+    name = _select_node(name, system_folders)
 
     # create node context
-    ctx = NodeContext(name, environment=environment,
-                      system_folders=system_folders)
+    ctx = NodeContext(name, system_folders=system_folders)
 
     # return path of the configuration
     info(f"Configuration file = {ctx.config_file}")
     info(f"Log file           = {ctx.log_file}")
     info(f"data folders       = {ctx.data_dir}")
     info("Database labels and files")
-    # TODO in v4+, this will always be a list so remove next few lines
-    if isinstance(ctx.databases, dict):
-        for label, path in ctx.databases.items():
-            info(f" - {label:15} = {path}")
-    else:
-        for db in ctx.databases:
-            info(f" - {db['label']:15} = {db['uri']} (type: {db['type']})")
+    for db in ctx.databases:
+        info(f" - {db['label']:15} = {db['uri']} (type: {db['type']})")
 
 
 #
 #   start
 #
 @cli_node.command(name='start')
 @click.option("-n", "--name", default=None, help="configuration name")
 @click.option("-c", "--config", default=None,
               help='absolute path to configuration-file; overrides NAME')
-@click.option('-e', '--environment', default=N_ENV,
-              help='configuration environment to use')
 @click.option('--system', 'system_folders', flag_value=True)
 @click.option('--user', 'system_folders', flag_value=False, default=N_FOL)
 @click.option('-i', '--image', default=None, help="Node Docker image to use")
 @click.option('--keep/--auto-remove', default=False,
               help="Keep image after finishing")
 @click.option('--force-db-mount', is_flag=True,
               help="Skip the check of the existence of the DB (always try to "
                    "mount)")
 @click.option('--attach/--detach', default=False,
               help="Attach node logs to the console after start")
 @click.option('--mount-src', default='',
               help="mount vantage6-master package source")
-def cli_node_start(name: str, config: str, environment: str,
-                   system_folders: bool, image: str, keep: bool,
-                   mount_src: str, attach: bool, force_db_mount: bool) -> None:
+def cli_node_start(name: str, config: str, system_folders: bool, image: str,
+                   keep: bool, mount_src: str, attach: bool,
+                   force_db_mount: bool) -> None:
     """
     Start the node instance inside a Docker container.
 
     Parameters
     ----------
     name : str
         Name of the configuration file.
     config : str
         Absolute path to configuration-file; overrides NAME
-    environment : str
-        DTAP environment to use.
     system_folders : bool
         Is this configuration stored in the system or in the user folders.
     image : str
         Node Docker image to use.
     keep : bool
         Keep container when finished or in the event of a crash. This is useful
         for debugging.
@@ -283,42 +251,41 @@
     attach : bool
         Attach node logs to the console after start.
     force_db_mount : bool
         Skip the check of the existence of the DB (always try to mount).
     """
     info("Starting node...")
     info("Finding Docker daemon")
+    print("alhoa")
     docker_client = docker.from_env()
     check_docker_running()
 
     NodeContext.LOGGING_ENABLED = False
     if config:
         name = Path(config).stem
-        ctx = NodeContext(name, environment, system_folders, config)
+        ctx = NodeContext(name, system_folders, config)
 
     else:
         # in case no name is supplied, ask the user to select one
         if not name:
-            name, environment = select_configuration_questionaire(
-                "node", system_folders)
+            name = select_configuration_questionaire("node", system_folders)
 
         # check that config exists, if not a questionaire will be invoked
-        if not NodeContext.config_exists(name, environment, system_folders):
-            warning(f"Configuration {Fore.RED}{name}{Style.RESET_ALL} "
-                    f"using environment {Fore.RED}{environment}"
-                    f"{Style.RESET_ALL} does not exist. ")
+        if not NodeContext.config_exists(name, system_folders):
+            warning(f"Configuration {Fore.RED}{name}{Style.RESET_ALL} does not"
+                    " exist.")
 
             if q.confirm("Create this configuration now?").ask():
-                configuration_wizard("node", name, environment, system_folders)
+                configuration_wizard("node", name, system_folders)
 
             else:
                 error("Config file couldn't be loaded")
                 sys.exit(0)
 
-        ctx = NodeContext(name, environment, system_folders)
+        ctx = NodeContext(name, system_folders)
 
     # check if config name is allowed docker name, else exit
     check_config_name_allowed(ctx.name)
 
     # check that this node is not already running
     running_nodes = docker_client.containers.list(
         filters={"label": f"{APPNAME}-type=node"}
@@ -335,22 +302,14 @@
     ctx.data_dir.mkdir(parents=True, exist_ok=True)
     ctx.log_dir.mkdir(parents=True, exist_ok=True)
 
     # Determine image-name. First we check if the option --image has been used.
     # Then we check if the image has been specified in the config file, and
     # finally we use the default settings from the package.
     if not image:
-
-        # FIXME: remove me in version 4+, as this is to support older
-        # configuration files. So the outer `image` key is no longer supported
-        if ctx.config.get('image'):
-            warning('Using the `image` option in the config file is to be '
-                    'removed in version 4+.')
-            image = ctx.config.get('image')
-
         custom_images: dict = ctx.config.get('images')
         if custom_images:
             image = custom_images.get("node")
         if not image:
             image = f"{DEFAULT_DOCKER_REGISTRY}/{DEFAULT_NODE_IMAGE}"
 
     info(f"Pulling latest node image '{image}'")
@@ -430,36 +389,23 @@
 
         # we remove the .tmp in the container, this is because the file is
         # mounted in a volume mount point. Somehow the file is than empty in
         # the volume but not for the node instance. By removing the .tmp we
         # make sure that the file is not empty in the volume.
         mounts.append((f"/mnt/ssh/{hostname}.pem.tmp", str(key_path)))
 
-    # Be careful not to use 'environment' as it would override the function
-    # argument ;-).
     env = {
         "DATA_VOLUME_NAME": data_volume.name,
         "VPN_VOLUME_NAME": vpn_volume.name,
         "PRIVATE_KEY": "/mnt/private_key.pem"
     }
 
     # only mount the DB if it is a file
     info("Setting up databases")
-
-    # Check wether the new or old database configuration is used
-    # TODO: remove this in version v4+
-    old_format = isinstance(ctx.databases, dict)
-    if old_format:
-        db_labels = ctx.databases.keys()
-        warning('Using the old database configuration format. Please update.')
-        debug('You are using the db config old format, algorithms using the '
-              'auto wrapper will not work!')
-    else:
-        db_labels = [db['label'] for db in ctx.databases]
-
+    db_labels = [db['label'] for db in ctx.databases]
     for label in db_labels:
 
         db_config = get_database_config(ctx.databases, label)
         uri = db_config['uri']
         db_type = db_config['type']
 
         info(f"  Processing {Fore.GREEN}{db_type}{Style.RESET_ALL} database "
@@ -480,31 +426,23 @@
             env[f'{label_capitals}_DATABASE_URI'] = uri
         else:
             debug('  - file-based database added')
             suffix = Path(uri).suffix
             env[f'{label_capitals}_DATABASE_URI'] = f'{label}{suffix}'
             mounts.append((f'/mnt/{label}{suffix}', str(uri)))
 
-        # FIXME legacy to support < 2.1.3 can be removed from 3+
-        # FIXME this is still required in v3+ but should be removed in v4
-        if label == 'default':
-            env['DATABASE_URI'] = '/mnt/default.csv'
-
     system_folders_option = "--system" if system_folders else "--user"
-    cmd = f'vnode-local start -c /mnt/config/{name}.yaml -n {name} -e '\
-          f'{environment} --dockerized {system_folders_option}'
+    cmd = f'vnode-local start -c /mnt/config/{name}.yaml -n {name} '\
+          f' --dockerized {system_folders_option}'
 
     info("Running Docker container")
     volumes = []
     for mount in mounts:
         volumes.append(f'{mount[1]}:{mount[0]}')
 
-    # debug(f"  with command: '{cmd}'")
-    # debug(f"  with mounts: {volumes}")
-    # debug(f"  with environment: {env}")
     remove_container_if_exists(
         docker_client=docker_client, name=ctx.docker_container_name
     )
 
     container = docker_client.containers.run(
         image,
         command=cmd,
@@ -659,65 +597,59 @@
 #
 #   create-private-key
 #
 @cli_node.command(name='create-private-key')
 @click.option("-n", "--name", default=None, help="configuration name")
 @click.option("-c", "--config", default=None,
               help='absolute path to configuration-file; overrides NAME')
-@click.option('-e', '--environment', default=N_ENV,
-              help='configuration environment to use')
 @click.option('--system', 'system_folders', flag_value=True)
 @click.option('--user', 'system_folders', flag_value=False, default=N_FOL)
 @click.option('--no-upload', 'upload', flag_value=False, default=True)
 @click.option("-o", "--organization-name", default=None,
               help="Organization name")
 @click.option('--overwrite', 'overwrite', flag_value=True, default=False)
 def cli_node_create_private_key(
-        name: str, config: str, environment: str, system_folders: bool,
-        upload: bool, organization_name: str, overwrite: bool
-        ) -> None:
+        name: str, config: str, system_folders: bool, upload: bool,
+        organization_name: str, overwrite: bool) -> None:
     """
     Create and upload a new private key (use with caution).
 
     Parameters
     ----------
     name : str
         Name of the configuration file.
     config : str
         Absolute path to configuration-file; overrides NAME.
-    environment : str
-        DTAP environment to use.
     system_folders : bool
         Wether this configuration stored in the system or in the user folders.
     upload : bool
         Wether to upload the private key to the server.
     organization_name : str
         Used to store and reference the private key.
     overwrite : bool
         Overwrite existing private key if present.
     """
     NodeContext.LOGGING_ENABLED = False
     if config:
         name = Path(config).stem
-        ctx = NodeContext(name, environment, system_folders, config)
+        ctx = NodeContext(name, system_folders, config)
     else:
         # retrieve context
-        name, environment = _select_node(name, environment, system_folders)
+        name = _select_node(name, system_folders)
 
         # raise error if config could not be found
-        if not NodeContext.config_exists(name, environment, system_folders):
+        if not NodeContext.config_exists(name, system_folders):
             error(
-                f"The configuration {Fore.RED}{name}{Style.RESET_ALL} with "
-                f"environment {Fore.RED}{environment}{Style.RESET_ALL} could "
-                f"not be found."
+                f"The configuration {Fore.RED}{name}{Style.RESET_ALL} could "
+                "not be found."
             )
             exit(1)
 
         # Create node context
-        ctx = NodeContext(name, environment, system_folders)
+        ctx = NodeContext(name, system_folders)
 
     # Authenticate with the server to obtain organization name if it wasn't
     # provided
     if organization_name is None:
         client = _create_client_and_authenticate(ctx)
         organization_name = client.whoami.organization_name
 
@@ -763,15 +695,15 @@
     # create public key
     info("Deriving public key")
     public_key = RSACryptor.create_public_key_bytes(private_key)
 
     # update config file
     info("Updating configuration")
     ctx.config["encryption"]["private_key"] = str(file_)
-    ctx.config_manager.put(environment, ctx.config)
+    ctx.config_manager.put(ctx.config)
     ctx.config_manager.save(ctx.config_file)
 
     # upload key to the server
     if upload:
         info(
             "Uploading public key to the server. "
             "This will overwrite any previously existing key!"
@@ -836,39 +768,34 @@
 
 
 #
 #   remove
 #
 @cli_node.command(name="remove")
 @click.option("-n", "--name", default=None)
-@click.option('-e', '--environment', default=N_ENV,
-              help='configuration environment to use')
 @click.option('--system', 'system_folders', flag_value=True)
 @click.option('--user', 'system_folders', flag_value=False, default=N_FOL)
-def cli_node_remove(name: str, environment: str, system_folders: bool) -> None:
+def cli_node_remove(name: str, system_folders: bool) -> None:
     """
     Delete a node permanently
 
     * if the node is still running, exit and tell user to run vnode stop first
     * remove configuration file
     * remove log file
     * remove docker volumes attached to the node
 
     Parameters
     ----------
     name : str
         Configuration name
-    environment : str
-        DTAP environment, note that regardless of the environment, the entire
-        configuration is deleted
     system_folders : bool
         If True, use system folders, otherwise use user folders
     """
     # select configuration name if none supplied
-    name, environment = _select_node(name, environment, system_folders)
+    name = _select_node(name, system_folders)
 
     client = docker.from_env()
     check_if_docker_daemon_is_running(client)
 
     # check if node is still running, otherwise don't allow deleting it
     running_node_names = _find_running_node_names(client)
 
@@ -883,16 +810,15 @@
         "This node will be deleted permanently including its configuration. "
         "Are you sure?", default=False
     ).ask():
         info("Node will not be deleted")
         exit(0)
 
     # create node context
-    ctx = NodeContext(name, environment=environment,
-                      system_folders=system_folders)
+    ctx = NodeContext(name, system_folders=system_folders)
 
     # remove the docker volume and any temporary volumes
     debug("Deleting docker volumes")
     volumes = client.volumes.list()
     for vol in volumes:
         if vol.name.startswith(ctx.docker_volume_name):  # includes tmp volumes
             info(f"Deleting docker volume {vol.name}")
@@ -962,53 +888,48 @@
 
 #
 #   set-api-key
 #
 @cli_node.command(name='set-api-key')
 @click.option("-n", "--name", default=None, help="configuration name")
 @click.option("--api-key", default=None, help="New API key")
-@click.option('-e', '--environment', default=N_ENV,
-              help='configuration environment to use')
 @click.option('--system', 'system_folders', flag_value=True)
 @click.option('--user', 'system_folders', flag_value=False, default=N_FOL)
-def cli_node_set_api_key(name: str, api_key: str, environment: str,
+def cli_node_set_api_key(name: str, api_key: str,
                          system_folders: bool) -> None:
     """
     Put a new API key into the node configuration file
 
     Parameters
     ----------
     name : str
         Node configuration name
     api_key : str
         New API key
-    environment : str
-        DTAP environment
     system_folders : bool
         If True, use system folders, otherwise use user folders
     """
-    # select name and environment
-    name, environment = _select_node(name, environment, system_folders)
+    # select node name
+    name = _select_node(name, system_folders)
 
     # Check that we can write in the config folder
     if not check_config_writeable(system_folders):
         error("Your user does not have write access to all folders. Exiting")
         exit(1)
 
     if not api_key:
         api_key = q.text("Please enter your new API key:").ask()
 
     # get configuration manager
-    ctx = NodeContext(name, environment=environment,
-                      system_folders=system_folders)
+    ctx = NodeContext(name, system_folders=system_folders)
     conf_mgr = NodeConfigurationManager.from_file(ctx.config_file)
 
     # set new api key, and save the file
     ctx.config['api_key'] = api_key
-    conf_mgr.put(environment, ctx.config)
+    conf_mgr.put(ctx.config)
     conf_mgr.save(ctx.config_file)
     info("Your new API key has been uploaded to the config file "
          f"{ctx.config_file}.")
 
 
 #  helper functions
 def _print_log_worker(logs_stream: Iterable[bytes]) -> None:
@@ -1020,72 +941,69 @@
     logs_stream : Iterable[bytes]
         Output of the container.attach() method
     """
     for log in logs_stream:
         print(log.decode(STRING_ENCODING), end="")
 
 
-def _create_client_and_authenticate(ctx: NodeContext) -> Client:
+def _create_client_and_authenticate(ctx: NodeContext) -> UserClient:
     """
     Generate a client and authenticate with the server.
 
     Parameters
     ----------
     ctx : NodeContext
         Context of the node loaded from the configuration file
 
     Returns
     -------
-    Client
+    UserClient
         vantage6 client
     """
     host = ctx.config['server_url']
     port = ctx.config['port']
     api_path = ctx.config['api_path']
 
     info(f"Connecting to server at '{host}:{port}{api_path}'")
     username = q.text("Username:").ask()
     password = q.password("Password:").ask()
 
-    client = Client(host, port, api_path)
+    client = UserClient(host, port, api_path)
 
     try:
         client.authenticate(username, password)
 
     except Exception as e:
         error("Could not authenticate with server!")
         debug(e)
         exit(1)
 
     return client
 
 
-def _select_node(name: str, environment: str, system_folders: bool) \
-        -> tuple[str, str]:
+def _select_node(name: str, system_folders: bool) -> tuple[str, str]:
     """
-    Let user select node through questionnaire if name/environment is not
-    given.
+    Let user select node through questionnaire if name is not given.
 
     Returns
     -------
-    tuple[str, str]
-        name, environment of the configuration file
+    str
+        Name of the configuration file
     """
-    name, environment = (name, environment) if name else \
+    name = name if name else \
         select_configuration_questionaire("node", system_folders)
 
     # raise error if config could not be found
-    if not NodeContext.config_exists(name, environment, system_folders):
+    if not NodeContext.config_exists(name, system_folders):
         error(
-            f"The configuration {Fore.RED}{name}{Style.RESET_ALL} with "
-            f"environment {Fore.RED}{environment}{Style.RESET_ALL} could "
+            f"The configuration {Fore.RED}{name}{Style.RESET_ALL} could "
             f"not be found."
         )
         exit(1)
-    return name, environment
+    return name
 
 
 def _find_running_node_names(client: docker.DockerClient) -> list[str]:
     """
     Returns a list of names of running nodes.
 
     Parameters
```

### Comparing `vantage6-3.9.0rc4/vantage6/cli/rabbitmq/__init__.py` & `vantage6-4.0.0a2/vantage6/cli/rabbitmq/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-3.9.0rc4/vantage6/cli/rabbitmq/definitions.py` & `vantage6-4.0.0a2/vantage6/cli/rabbitmq/definitions.py`

 * *Files identical despite different names*

### Comparing `vantage6-3.9.0rc4/vantage6/cli/rabbitmq/queue_manager.py` & `vantage6-4.0.0a2/vantage6/cli/rabbitmq/queue_manager.py`

 * *Files identical despite different names*

### Comparing `vantage6-3.9.0rc4/vantage6/cli/server.py` & `vantage6-4.0.0a2/vantage6/cli/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,16 +24,15 @@
     APPNAME,
     STRING_ENCODING,
     DEFAULT_DOCKER_REGISTRY,
     DEFAULT_SERVER_IMAGE
 )
 from vantage6.cli.rabbitmq import split_rabbitmq_uri
 
-from vantage6.cli.globals import (DEFAULT_SERVER_ENVIRONMENT,
-                                  DEFAULT_SERVER_SYSTEM_FOLDERS)
+from vantage6.cli.globals import DEFAULT_SERVER_SYSTEM_FOLDERS
 from vantage6.cli.context import ServerContext
 from vantage6.cli.configuration_wizard import (
     select_configuration_questionaire,
     configuration_wizard
 )
 from vantage6.cli.utils import check_config_name_allowed
 from vantage6.cli.rabbitmq.queue_manager import RabbitMQManager
@@ -55,63 +54,57 @@
     Callable
         Click function with context
     """
     @click.option('-n', '--name', default=None,
                   help="name of the configuration you want to use.")
     @click.option('-c', '--config', default=None,
                   help='absolute path to configuration-file; overrides NAME')
-    @click.option('-e', '--environment',
-                  default=DEFAULT_SERVER_ENVIRONMENT,
-                  help='configuration environment to use')
     @click.option('--system', 'system_folders', flag_value=True)
     @click.option('--user', 'system_folders', flag_value=False,
                   default=DEFAULT_SERVER_SYSTEM_FOLDERS)
     @wraps(func)
-    def func_with_context(name: str, config: str, environment: str,
-                          system_folders: bool, *args, **kwargs) -> callable:
+    def func_with_context(name: str, config: str, system_folders: bool, *args,
+                          **kwargs) -> callable:
         """
         Decorator function that adds the context to the function.
 
         Parameters
         ----------
         name : str
             name of the configuration you want to use.
         config : str
             path to configuration file, overrides name
-        environment : str
-            DTAP environment to use
         system_folders : bool
             Wether to use system folders or not
 
         Returns
         -------
         Callable
             Decorated function
         """
         # path to configuration file always overrides name
         if config:
             ctx = ServerContext.from_external_config_file(
                 config,
-                environment,
                 system_folders
             )
             return func(ctx, *args, **kwargs)
 
         # in case no name is supplied, ask the user to select one
         if not name:
             try:
                 # select configuration if none supplied
-                name, environment = select_configuration_questionaire(
+                name = select_configuration_questionaire(
                     "server", system_folders
                 )
             except Exception:
                 error("No configurations could be found!")
                 exit(1)
 
-        ctx = _get_server_context(name, environment, system_folders)
+        ctx = _get_server_context(name, system_folders)
         return func(ctx, *args, **kwargs)
 
     return func_with_context
 
 
 @click.group(name='server')
 def cli_server() -> None:
@@ -314,45 +307,40 @@
         filters={"label": f"{APPNAME}-type=server"})
     running_node_names = []
     for node in running_server:
         running_node_names.append(node.name)
 
     header = \
         "\nName"+(21*" ") + \
-        "Environments"+(20*" ") + \
         "Status"+(10*" ") + \
         "System/User"
 
     click.echo(header)
     click.echo("-"*len(header))
 
     running = Fore.GREEN + "Online" + Style.RESET_ALL
     stopped = Fore.RED + "Offline" + Style.RESET_ALL
 
     # system folders
-    configs, f1 = ServerContext.available_configurations(
-        system_folders=True)
+    configs, f1 = ServerContext.available_configurations(system_folders=True)
     for config in configs:
         status = running if f"{APPNAME}-{config.name}-system-server" in \
             running_node_names else stopped
         click.echo(
             f"{config.name:25}"
-            f"{str(config.available_environments):32}"
             f"{status:25} System "
         )
 
     # user folders
-    configs, f2 = ServerContext.available_configurations(
-        system_folders=False)
+    configs, f2 = ServerContext.available_configurations(system_folders=False)
     for config in configs:
         status = running if f"{APPNAME}-{config.name}-user-server" in \
             running_node_names else stopped
         click.echo(
             f"{config.name:25}"
-            f"{str(config.available_environments):32}"
             f"{status:25} User   "
         )
 
     click.echo("-"*85)
     if len(f1)+len(f2):
         warning(
              f"{Fore.RED}Failed imports: {len(f1)+len(f2)}{Style.RESET_ALL}")
@@ -379,64 +367,56 @@
 
 #
 #   new
 #
 @cli_server.command(name='new')
 @click.option('-n', '--name', default=None,
               help="name of the configuration you want to use.")
-@click.option('-e', '--environment', default=DEFAULT_SERVER_ENVIRONMENT,
-              help='configuration environment to use')
 @click.option('--system', 'system_folders', flag_value=True)
 @click.option('--user', 'system_folders', flag_value=False,
               default=DEFAULT_SERVER_SYSTEM_FOLDERS)
-def cli_server_new(name: str, environment: str, system_folders: bool) -> None:
+def cli_server_new(name: str, system_folders: bool) -> None:
     """
     Create a new server configuration.
 
     Parameters
     ----------
     name : str
         name of the new configuration
-    environment : str
-        DTAP environment you want to configure
     system_folders : bool
         Wether to use system folders or not
     """
     if not name:
         name = q.text("Please enter a configuration-name:").ask()
         if name.count(" ") > 0:
             name = name.replace(" ", "-")
             info(f"Replaced spaces from configuration name: {name}")
 
     # check if name is allowed for docker volume, else exit
     check_config_name_allowed(name)
 
     # check that this config does not exist
     try:
-        if ServerContext.config_exists(name, environment, system_folders):
-            error(
-                f"Configuration {Fore.RED}{name}{Style.RESET_ALL} with "
-                f"environment {Fore.RED}{environment}{Style.RESET_ALL} "
-                f"already exists!"
-            )
+        if ServerContext.config_exists(name, system_folders):
+            error(f"Configuration {Fore.RED}{name}{Style.RESET_ALL} already "
+                  "exists!")
             exit(1)
     except Exception as e:
         error(e)
         exit(1)
 
     # Check that we can write in this folder
     if not check_config_writeable(system_folders):
         error("Your user does not have write access to all folders. Exiting")
         info(f"Create a new server using '{Fore.GREEN}vserver new "
              f"--user{Style.RESET_ALL}' instead!")
         exit(1)
 
     # create config in ctx location
-    cfg_file = configuration_wizard("server", name, environment=environment,
-                                    system_folders=system_folders)
+    cfg_file = configuration_wizard("server", name, system_folders)
     info(f"New configuration created: {Fore.GREEN}{cfg_file}{Style.RESET_ALL}")
 
     # info(f"root user created.")
     flag = "" if system_folders else "--user"
     info(f"You can start the server by running {Fore.GREEN}vserver start "
          f"{flag}{Style.RESET_ALL}")
 
@@ -543,16 +523,16 @@
 
     else:
         warning(f"Database could not be transferred, make sure {url.host} "
                 "is reachable from the Docker container")
         info("Consider using the docker-compose method to start a server")
 
     drop_all_ = "--drop-all" if drop_all else ""
-    cmd = f'vserver-local import -c /mnt/config.yaml -e {ctx.environment} ' \
-          f'{drop_all_} /mnt/import.yaml'
+    cmd = (f'vserver-local import -c /mnt/config.yaml {drop_all_} '
+           '/mnt/import.yaml')
 
     info(cmd)
 
     info("Run Docker container")
     container = docker_client.containers.run(
         image,
         command=cmd,
@@ -607,31 +587,26 @@
 
 
 #
 #   stop
 #
 @cli_server.command(name='stop')
 @click.option("-n", "--name", default=None, help="Configuration name")
-@click.option('-e', '--environment', default=DEFAULT_SERVER_ENVIRONMENT,
-              help='configuration environment to use')
 @click.option('--system', 'system_folders', flag_value=True)
 @click.option('--user', 'system_folders', flag_value=False,
               default=DEFAULT_SERVER_SYSTEM_FOLDERS)
 @click.option('--all', 'all_servers', flag_value=True, help="Stop all servers")
-def cli_server_stop(name: str, environment: str, system_folders: bool,
-                    all_servers: bool):
+def cli_server_stop(name: str, system_folders: bool, all_servers: bool):
     """
     Stop one or all running server(s).
 
     Parameters
     ----------
     name : str
         Name of the server to stop
-    environment : str
-        DTAP environment to use
     system_folders : bool
         Wether to use system folders or not
     all_servers : bool
         Wether to stop all servers or not
     """
     client = docker.from_env()
     check_docker_running()
@@ -643,32 +618,30 @@
         warning("No servers are currently running.")
         return
 
     running_server_names = [server.name for server in running_servers]
 
     if all_servers:
         for container_name in running_server_names:
-            _stop_server_containers(client, container_name, environment,
-                                    system_folders)
+            _stop_server_containers(client, container_name, system_folders)
         return
 
     # make sure we have a configuration name to work with
     if not name:
         container_name = q.select("Select the server you wish to stop:",
                                   choices=running_server_names).ask()
     else:
         post_fix = "system" if system_folders else "user"
         container_name = f"{APPNAME}-{name}-{post_fix}-server"
 
     if container_name not in running_server_names:
         error(f"{Fore.RED}{name}{Style.RESET_ALL} is not running!")
         return
 
-    _stop_server_containers(client, container_name, environment,
-                            system_folders)
+    _stop_server_containers(client, container_name, system_folders)
 
 
 #
 #   attach
 #
 @cli_server.command(name='attach')
 @click.option("-n", "--name", default=None, help="configuration name")
@@ -762,49 +735,45 @@
     else:
         error(f"Server {name} is not running! Cannot provide version...")
 
 
 #
 # helper functions
 #
-def _get_server_context(name: str, environment: str, system_folders: bool) \
+def _get_server_context(name: str, system_folders: bool) \
         -> ServerContext:
     """
     Load the server context from the configuration file.
 
     Parameters
     ----------
     name : str
         Name of the server to inspect
-    environment : str
-        DTAP environment to use
     system_folders : bool
         Wether to use system folders or if False, the user folders
 
     Returns
     -------
     ServerContext
         Server context object
     """
-    if not ServerContext.config_exists(name, environment, system_folders):
+    if not ServerContext.config_exists(name, system_folders):
         scope = "system" if system_folders else "user"
         error(
-                f"Configuration {Fore.RED}{name}{Style.RESET_ALL} with "
-                f"{Fore.RED}{environment}{Style.RESET_ALL} does not exist "
-                f"in the {Fore.RED}{scope}{Style.RESET_ALL} folders!"
-            )
+            f"Configuration {Fore.RED}{name}{Style.RESET_ALL} does not "
+            f"exist in the {Fore.RED}{scope}{Style.RESET_ALL} folders!"
+        )
         exit(1)
 
     # We do not want to log this here, we do this in the container and not on
     # the host. We only want CLI logging here.
     ServerContext.LOGGING_ENABLED = False
 
     # create server context, and initialize db
-    ctx = ServerContext(name, environment=environment,
-                        system_folders=system_folders)
+    ctx = ServerContext(name, system_folders=system_folders)
 
     return ctx
 
 
 def _start_rabbitmq(ctx: ServerContext, rabbitmq_image: str,
                     network_mgr: NetworkManager) -> None:
     """
@@ -830,41 +799,39 @@
         rabbit_mgr.start()
     else:
         info("Detected that the RabbitMQ service is a external service. "
              "Assuming this service is up and running.")
 
 
 def _stop_server_containers(client: DockerClient, container_name: str,
-                            environment: str, system_folders: bool) -> None:
+                            system_folders: bool) -> None:
     """
     Given a server's name, kill its docker container and related (RabbitMQ)
     containers.
 
     Parameters
     ----------
     client : DockerClient
         Docker client
     container_name : str
         Name of the server to stop
-    environment : str
-        DTAP environment to use
     system_folders : bool
         Wether to use system folders or not
     """
     # kill the server
     container = client.containers.get(container_name)
     container.kill()
     info(f"Stopped the {Fore.GREEN}{container_name}{Style.RESET_ALL} server.")
 
     # find the configuration name from the docker container name
     # server name is formatted as f"{APPNAME}-{self.name}-{self.scope}-server"
     scope = "system" if system_folders else "user"
     config_name = get_server_config_name(container_name, scope)
 
-    ctx = _get_server_context(config_name, environment, system_folders)
+    ctx = _get_server_context(config_name, system_folders)
 
     # delete the server network
     network_name = f"{APPNAME}-{ctx.name}-{ctx.scope}-network"
     network = get_network(client, name=network_name)
     delete_network(network, kill_containers=False)
 
     # kill RabbitMQ if it exists and no other servers are using to it (i.e. it
```

### Comparing `vantage6-3.9.0rc4/vantage6/cli/utils.py` & `vantage6-4.0.0a2/vantage6/cli/utils.py`

 * *Files identical despite different names*

### Comparing `vantage6-3.9.0rc4/vantage6.egg-info/PKG-INFO` & `vantage6-4.0.0a2/vantage6.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6
-Version: 3.9.0rc4
+Version: 4.0.0a2
 Summary: vantage6 command line interface
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,11 +1,10 @@
-Metadata-Version: 2.1 Name: vantage6 Version: 3.9.0rc4 Summary: vantage6
-command line interface Home-page: https://github.com/vantage6/vantage6
-Requires-Python: >=3.6 Description-Content-Type: text/markdown Provides-Extra:
-dev
+Metadata-Version: 2.1 Name: vantage6 Version: 4.0.0a2 Summary: vantage6 command
+line interface Home-page: https://github.com/vantage6/vantage6 Requires-Python:
+>=3.6 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml) [![PyPI vantage6](https://badge.fury.io/py/vantage6.svg)](https://
 badge.fury.io/py/vantage6) [![Unittests](https://github.com/vantage6/vantage6/
```

### Comparing `vantage6-3.9.0rc4/vantage6.egg-info/SOURCES.txt` & `vantage6-4.0.0a2/vantage6.egg-info/SOURCES.txt`

 * *Files identical despite different names*

