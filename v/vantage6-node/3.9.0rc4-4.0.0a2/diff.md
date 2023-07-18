# Comparing `tmp/vantage6-node-3.9.0rc4.tar.gz` & `tmp/vantage6-node-4.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-node-3.9.0rc4.tar", last modified: Wed May 24 09:34:09 2023, max compression
+gzip compressed data, was "vantage6-node-4.0.0a2.tar", last modified: Tue Jul 18 13:32:09 2023, max compression
```

## Comparing `vantage6-node-3.9.0rc4.tar` & `vantage6-node-4.0.0a2.tar`

### file list

```diff
@@ -1,38 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:09.957728 vantage6-node-3.9.0rc4/
--rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-05-24 09:34:09.957728 vantage6-node-3.9.0rc4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 09:34:09.957728 vantage6-node-3.9.0rc4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-24 09:33:56.000000 vantage6-node-3.9.0rc4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:09.957728 vantage6-node-3.9.0rc4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 09:33:56.000000 vantage6-node-3.9.0rc4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 09:33:56.000000 vantage6-node-3.9.0rc4/tests/test_ssh_tunnel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:09.957728 vantage6-node-3.9.0rc4/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:09.957728 vantage6-node-3.9.0rc4/vantage6/node/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 09:33:56.000000 vantage6-node-3.9.0rc4/vantage6/node/__build__
--rw-r--r--   0 runner    (1001) docker     (123)    42264 2023-05-24 09:33:56.000000 vantage6-node-3.9.0rc4/vantage6/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-24 09:33:56.000000 vantage6-node-3.9.0rc4/vantage6/node/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:09.957728 vantage6-node-3.9.0rc4/vantage6/node/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 09:33:56.000000 vantage6-node-3.9.0rc4/vantage6/node/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8188 2023-05-24 09:33:56.000000 vantage6-node-3.9.0rc4/vantage6/node/cli/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-24 09:33:56.000000 vantage6-node-3.9.0rc4/vantage6/node/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:09.957728 vantage6-node-3.9.0rc4/vantage6/node/docker/
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-24 09:33:56.000000 vantage6-node-3.9.0rc4/vantage6/node/docker/docker_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    24977 2023-05-24 09:33:56.000000 vantage6-node-3.9.0rc4/vantage6/node/docker/docker_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-24 09:33:56.000000 vantage6-node-3.9.0rc4/vantage6/node/docker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-05-24 09:33:56.000000 vantage6-node-3.9.0rc4/vantage6/node/docker/squid.py
--rw-r--r--   0 runner    (1001) docker     (123)     9599 2023-05-24 09:33:56.000000 vantage6-node-3.9.0rc4/vantage6/node/docker/ssh_tunnel.py
--rw-r--r--   0 runner    (1001) docker     (123)    19729 2023-05-24 09:33:56.000000 vantage6-node-3.9.0rc4/vantage6/node/docker/task_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    22663 2023-05-24 09:33:56.000000 vantage6-node-3.9.0rc4/vantage6/node/docker/vpn_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-24 09:33:56.000000 vantage6-node-3.9.0rc4/vantage6/node/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11555 2023-05-24 09:33:56.000000 vantage6-node-3.9.0rc4/vantage6/node/proxy_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    11813 2023-05-24 09:33:56.000000 vantage6-node-3.9.0rc4/vantage6/node/server_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-05-24 09:33:56.000000 vantage6-node-3.9.0rc4/vantage6/node/socket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:09.957728 vantage6-node-3.9.0rc4/vantage6/node/util/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-24 09:33:56.000000 vantage6-node-3.9.0rc4/vantage6/node/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-05-24 09:33:56.000000 vantage6-node-3.9.0rc4/vantage6/node/util/colorer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:09.957728 vantage6-node-3.9.0rc4/vantage6_node.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-05-24 09:34:09.000000 vantage6-node-3.9.0rc4/vantage6_node.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-24 09:34:09.000000 vantage6-node-3.9.0rc4/vantage6_node.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 09:34:09.000000 vantage6-node-3.9.0rc4/vantage6_node.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-24 09:34:09.000000 vantage6-node-3.9.0rc4/vantage6_node.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-24 09:34:09.000000 vantage6-node-3.9.0rc4/vantage6_node.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-24 09:34:09.000000 vantage6-node-3.9.0rc4/vantage6_node.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:32:09.012682 vantage6-node-4.0.0a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-07-18 13:32:09.012682 vantage6-node-4.0.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 13:32:09.012682 vantage6-node-4.0.0a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-18 13:31:55.000000 vantage6-node-4.0.0a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:32:09.008682 vantage6-node-4.0.0a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:31:55.000000 vantage6-node-4.0.0a2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:31:55.000000 vantage6-node-4.0.0a2/tests/test_ssh_tunnel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:32:09.008682 vantage6-node-4.0.0a2/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:32:09.008682 vantage6-node-4.0.0a2/vantage6/node/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 13:31:55.000000 vantage6-node-4.0.0a2/vantage6/node/__build__
+-rw-r--r--   0 runner    (1001) docker     (123)    41597 2023-07-18 13:31:55.000000 vantage6-node-4.0.0a2/vantage6/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-18 13:31:55.000000 vantage6-node-4.0.0a2/vantage6/node/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:32:09.008682 vantage6-node-4.0.0a2/vantage6/node/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:31:55.000000 vantage6-node-4.0.0a2/vantage6/node/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-07-18 13:31:55.000000 vantage6-node-4.0.0a2/vantage6/node/cli/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-18 13:31:55.000000 vantage6-node-4.0.0a2/vantage6/node/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:32:09.008682 vantage6-node-4.0.0a2/vantage6/node/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-18 13:31:55.000000 vantage6-node-4.0.0a2/vantage6/node/docker/docker_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23561 2023-07-18 13:31:55.000000 vantage6-node-4.0.0a2/vantage6/node/docker/docker_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-18 13:31:55.000000 vantage6-node-4.0.0a2/vantage6/node/docker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-07-18 13:31:55.000000 vantage6-node-4.0.0a2/vantage6/node/docker/squid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9599 2023-07-18 13:31:55.000000 vantage6-node-4.0.0a2/vantage6/node/docker/ssh_tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19632 2023-07-18 13:31:55.000000 vantage6-node-4.0.0a2/vantage6/node/docker/task_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23828 2023-07-18 13:31:55.000000 vantage6-node-4.0.0a2/vantage6/node/docker/vpn_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-18 13:31:55.000000 vantage6-node-4.0.0a2/vantage6/node/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11482 2023-07-18 13:31:55.000000 vantage6-node-4.0.0a2/vantage6/node/proxy_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-07-18 13:31:55.000000 vantage6-node-4.0.0a2/vantage6/node/socket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:32:09.008682 vantage6-node-4.0.0a2/vantage6/node/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-18 13:31:55.000000 vantage6-node-4.0.0a2/vantage6/node/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-07-18 13:31:55.000000 vantage6-node-4.0.0a2/vantage6/node/util/colorer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:32:09.008682 vantage6-node-4.0.0a2/vantage6_node.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-07-18 13:32:08.000000 vantage6-node-4.0.0a2/vantage6_node.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-18 13:32:08.000000 vantage6-node-4.0.0a2/vantage6_node.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 13:32:08.000000 vantage6-node-4.0.0a2/vantage6_node.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-18 13:32:08.000000 vantage6-node-4.0.0a2/vantage6_node.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-18 13:32:08.000000 vantage6-node-4.0.0a2/vantage6_node.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-18 13:32:08.000000 vantage6-node-4.0.0a2/vantage6_node.egg-info/top_level.txt
```

### Comparing `vantage6-node-3.9.0rc4/PKG-INFO` & `vantage6-node-4.0.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-node
-Version: 3.9.0rc4
+Version: 4.0.0a2
 Summary: vantage6 node
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-node Version: 3.9.0rc4 Summary: vantage6
+Metadata-Version: 2.1 Name: vantage6-node Version: 4.0.0a2 Summary: vantage6
 node Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-node-3.9.0rc4/setup.py` & `vantage6-node-4.0.0a2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,15 +44,14 @@
     extras_require={
         'dev': [
             'coverage==6.4.4',
             'python-coveralls==2.9.3',
             'SQLAlchemy==1.4.46',
             'schema==0.7.5',
             'appdirs==1.4.4',
-            'PyJWT==2.6.0',
             'flask==2.2.5'
         ]
     },
     package_data={
         'vantage6.node': [
             '__build__',
             '_data/*.*',
```

### Comparing `vantage6-node-3.9.0rc4/vantage6/node/__init__.py` & `vantage6-node-4.0.0a2/vantage6/node/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 from vantage6.common.log import get_file_logger
 from vantage6.cli.context import NodeContext
 from vantage6.node.context import DockerNodeContext
 from vantage6.node.globals import (
     NODE_PROXY_SERVER_HOSTNAME, SLEEP_BTWN_NODE_LOGIN_TRIES,
     TIME_LIMIT_RETRY_CONNECT_NODE, TIME_LIMIT_INITIAL_CONNECTION_WEBSOCKET
 )
-from vantage6.node.server_io import NodeClient
+from vantage6.common.client.node_client import NodeClient
 from vantage6.node import proxy_server
 from vantage6.node.util import get_parent_id
 from vantage6.node.docker.docker_manager import DockerManager
 from vantage6.node.docker.vpn_manager import VPNManager
 from vantage6.node.socket import NodeTaskNamespace
 from vantage6.node.docker.ssh_tunnel import SSHTunnel
 from vantage6.node.docker.squid import Squid
@@ -104,21 +104,21 @@
 
         self.config = self.ctx.config
         self.debug: dict = self.config.get('debug', {})
         self.queue = queue.Queue()
         self._using_encryption = None
 
         # initialize Node connection to the server
-        self.server_io = NodeClient(
+        self.client = NodeClient(
             host=self.config.get('server_url'),
             port=self.config.get('port'),
             path=self.config.get('api_path')
         )
 
-        self.log.info(f"Connecting server: {self.server_io.base_path}")
+        self.log.info(f"Connecting server: {self.client.base_path}")
 
         # Authenticate with the server, obtaining a JSON Web Token.
         # Note that self.authenticate() blocks until it succeeds.
         self.log.debug("Authenticating")
         self.authenticate()
 
         # Setup encryption
@@ -156,15 +156,15 @@
         # setup the docker manager
         self.log.debug("Setting up the docker manager")
         self.__docker = DockerManager(
             ctx=self.ctx,
             isolated_network_mgr=isolated_network_mgr,
             vpn_manager=self.vpn_manager,
             tasks_dir=self.__tasks_dir,
-            client=self.server_io,
+            client=self.client,
             proxy=self.squid
         )
 
         # Create a long-lasting websocket connection.
         self.log.debug("Creating websocket connection with the server")
         self.connect_to_socket()
 
@@ -218,16 +218,16 @@
         proxy_port = int(os.environ.get("PROXY_SERVER_PORT", 8080))
 
         # 'app' is defined in vantage6.node.proxy_server
         debug_mode = self.debug.get("proxy_server", False)
         if debug_mode:
             self.log.debug("Debug mode enabled for proxy server")
             proxy_server.app.debug = True
-        proxy_server.app.config["SERVER_IO"] = self.server_io
-        proxy_server.server_url = self.server_io.base_path
+        proxy_server.app.config["SERVER_IO"] = self.client
+        proxy_server.server_url = self.client.base_path
 
         # set up proxy server logging
         log_level = getattr(logging, self.config["logging"]["level"].upper())
         self.proxy_log = get_file_logger(
             'proxy_server', self.ctx.proxy_log_file, log_level_file=log_level
         )
 
@@ -256,19 +256,18 @@
 
             except Exception as e:
                 self.log.error('Proxyserver could not be started or crashed!')
                 self.log.error(e)
 
     def sync_task_queue_with_server(self) -> None:
         """ Get all unprocessed tasks from the server for this node."""
-        assert self.server_io.cryptor, "Encrpytion has not been setup"
+        assert self.client.cryptor, "Encrpytion has not been setup"
 
         # request open tasks from the server
-        task_results = self.server_io.get_results(state="open",
-                                                  include_task=True)
+        task_results = self.client.run.list(state="open", include_task=True)
         self.log.debug(task_results)
 
         # add the tasks to the queue
         self.__add_tasks_to_queue(task_results)
         self.log.info(f"Received {self.queue._qsize()} tasks")
 
     def get_task_and_add_to_queue(self, task_id: int) -> None:
@@ -278,15 +277,15 @@
 
         Parameters
         ----------
         task_id : int
             Task identifier
         """
         # fetch (open) result for the node with the task_id
-        task_results = self.server_io.get_results(
+        task_results = self.client.run.list(
             include_task=True,
             state='open',
             task_id=task_id
         )
 
         # add the tasks to the queue
         self.__add_tasks_to_queue(task_results)
@@ -310,68 +309,68 @@
                         f"Not starting task {task_result['task']['id']} - "
                         f"{task_result['task']['name']} as it is already "
                         "running"
                     )
             except Exception:
                 self.log.exception("Error while syncing task queue")
 
-    def __start_task(self, taskresult: dict) -> None:
+    def __start_task(self, task_incl_run: dict) -> None:
         """
         Start the docker image and notify the server that the task has been
         started.
 
         Parameters
         ----------
-        taskresult : dict
+        task_incl_run : dict
             A dictionary with information required to run the algorithm
         """
-        task = taskresult['task']
+        task = task_incl_run['task']
         self.log.info("Starting task {id} - {name}".format(**task))
 
         # notify that we are processing this task
-        self.server_io.set_task_start_time(taskresult["id"])
+        self.client.set_task_start_time(task_incl_run["id"])
 
-        token = self.server_io.request_token_for_container(
+        token = self.client.request_token_for_container(
             task["id"],
             task["image"]
         )
         token = token["container_token"]
 
-        # create a temporary volume for each run_id
-        vol_name = self.ctx.docker_temporary_volume_name(task["run_id"])
+        # create a temporary volume for each job_id
+        vol_name = self.ctx.docker_temporary_volume_name(task["job_id"])
         self.__docker.create_volume(vol_name)
 
         # For some reason, if the key 'input' consists of JSON, it is
         # automatically marshalled? This causes trouble, so we'll serialize it
         # again.
         # FIXME: should probably find & fix the root cause?
-        if type(taskresult['input']) == dict:
-            taskresult['input'] = json.dumps(taskresult['input'])
+        if type(task_incl_run['input']) == dict:
+            task_incl_run['input'] = json.dumps(task_incl_run['input'])
 
         # Run the container. This adds the created container/task to the list
         # __docker.active_tasks
         task_status, vpn_ports = self.__docker.run(
-            result_id=taskresult["id"],
+            run_id=task_incl_run["id"],
             task_info=task,
             image=task["image"],
-            docker_input=taskresult['input'],
+            docker_input=task_incl_run['input'],
             tmp_vol_name=vol_name,
             token=token,
-            database=task.get('database', 'default')
+            databases_to_use=task.get('databases', ['default'])
         )
 
         # save task status to the server
         update = {'status': task_status}
         if task_status == TaskStatus.NOT_ALLOWED:
             # set finished_at to now, so that the task is not picked up again
             # (as the task is not started at all, unlike other crashes, it will
             # never finish and hence not be set to finished)
             update['finished_at'] = datetime.datetime.now().isoformat()
-        self.server_io.patch_results(
-            id_=taskresult['id'], result=update
+        self.client.run.patch(
+            id_=task_incl_run['id'], data=update
         )
 
         # ensure that the /tasks namespace is connected. This may take a while
         # (usually < 5s) when the socket just (re)connected
         MAX_ATTEMPTS = 30
         retries = 0
         while '/tasks' not in self.socketIO.namespaces and \
@@ -383,44 +382,36 @@
         # in case the namespace is still not connected, the socket notification
         # will not be sent to other nodes, but the task will still be processed
 
         # send socket event to alert everyone of task status change
         self.socketIO.emit(
             'algorithm_status_change',
             data={
-                'node_id': self.server_io.whoami.id_,
+                'node_id': self.client.whoami.id_,
                 'status': task_status,
-                'result_id': taskresult['id'],
+                'run_id': task_incl_run['id'],
                 'task_id': task['id'],
-                'collaboration_id': self.server_io.collaboration_id,
-                'organization_id': self.server_io.whoami.organization_id,
+                'collaboration_id': self.client.collaboration_id,
+                'organization_id': self.client.whoami.organization_id,
                 'parent_id': get_parent_id(task),
             },
             namespace='/tasks',
         )
 
         if vpn_ports:
             # Save port of VPN client container at which it redirects traffic
             # to the algorithm container. First delete any existing port
             # assignments in case algorithm has crashed
-            self.server_io.request(
-                'port', params={'result_id': taskresult['id']}, method="DELETE"
+            self.client.request(
+                'port', params={'result_id': task_incl_run['id']},
+                method="DELETE"
             )
             for port in vpn_ports:
-                port['result_id'] = taskresult['id']
-                self.server_io.request('port', method='POST', json=port)
-
-            # Save IP address of VPN container
-            # FIXME BvB 2023-02-21: node IP is now updated when task is started
-            # but this should be done when VPN connection is established
-            node_id = self.server_io.whoami.id_
-            node_ip = self.vpn_manager.get_vpn_ip()
-            self.server_io.request(
-                f"node/{node_id}", json={"ip": node_ip}, method="PATCH"
-            )
+                port['result_id'] = task_incl_run['id']
+                self.client.request('port', method='POST', json=port)
 
     def __listening_worker(self) -> None:
         """
         Listen for incoming (websocket) messages from the server.
 
         Runs in a separate thread. Received events are handled by the
         appropriate action handler.
@@ -454,81 +445,81 @@
             try:
                 results = self.__docker.get_result()
 
                 # notify socket channel of algorithm status change
                 self.socketIO.emit(
                     'algorithm_status_change',
                     data={
-                        'node_id': self.server_io.whoami.id_,
+                        'node_id': self.client.whoami.id_,
                         'status': results.status,
-                        'result_id': results.result_id,
+                        'run_id': results.run_id,
                         'task_id': results.task_id,
-                        'collaboration_id': self.server_io.collaboration_id,
+                        'collaboration_id': self.client.collaboration_id,
                         'organization_id':
-                            self.server_io.whoami.organization_id,
+                            self.client.whoami.organization_id,
                         'parent_id': results.parent_id,
                     },
                     namespace='/tasks',
                 )
 
                 self.log.info(
-                    f"Sending result (id={results.result_id}) to the server!")
+                    f"Sending result (run={results.run_id}) to the server!")
 
                 # FIXME: why are we retrieving the result *again*? Shouldn't we
                 # just store the task_id when retrieving the task the first
                 # time?
-                response = self.server_io.request(
-                    f"result/{results.result_id}"
+                response = self.client.request(
+                    f"run/{results.run_id}"
                 )
                 task_id = response.get("task").get("id")
 
                 if not task_id:
                     self.log.error(
-                        f"task_id of result (id={results.result_id}) "
+                        f"task_id of run (id={results.run_id}) "
                         f"could not be retrieved"
                     )
                     return
 
-                response = self.server_io.request(f"task/{task_id}")
+                response = self.client.request(f"task/{task_id}")
 
-                init_org_id = response.get("initiator")
-                if not init_org_id:
+                init_org = response.get("init_org")
+                if not init_org:
                     self.log.error(
-                        f"Initiator organization from task (id={task_id})could"
-                        " not be retrieved!"
+                        f"Initiator organization from task (id={task_id}) "
+                        "could not be retrieved!"
                     )
 
-                self.server_io.patch_results(
-                    id_=results.result_id,
-                    result={
+                self.client.run.patch(
+                    id_=results.run_id,
+                    data={
                         'result': results.data,
                         'log': results.logs,
                         'status': results.status,
                         'finished_at': datetime.datetime.now().isoformat(),
                     },
-                    init_org_id=init_org_id,
+                    init_org_id=init_org.get("id"),
                 )
             except Exception:
                 self.log.exception('Speaking thread had an exception')
 
     def __print_connection_error_logs(self):
         """ Print error message when node cannot find the server """
         self.log.warning(
             "Could not connect to the server. Retrying in 10 seconds")
-        if self.server_io.host == 'http://localhost' and running_in_docker():
+        if self.client.host == 'http://localhost' and running_in_docker():
             self.log.warn(
-                f"You are trying to reach the server at {self.server_io.host}."
+                f"You are trying to reach the server at {self.client.host}."
                 " As your node is running inside a Docker container, it cannot"
                 " reach localhost on your host system. Probably, you have to "
                 "change your serverl URL to http://host.docker.internal "
                 "(Windows/MacOS) or http://172.17.0.1 (Linux)."
             )
         else:
             self.log.debug("Are you sure the server can be reached at "
-                           f"{self.server_io.base_path}?")
+                           f"{self.client.base_path}?")
 
     def authenticate(self) -> None:
         """
         Authenticate with the server using the api-key from the configuration
         file. If the server rejects for any reason -other than a wrong API key-
         serveral attempts are taken to retry.
         """
@@ -536,15 +527,15 @@
         api_key = self.config.get("api_key")
 
         success = False
         i = 0
         while i < TIME_LIMIT_RETRY_CONNECT_NODE / SLEEP_BTWN_NODE_LOGIN_TRIES:
             i = i + 1
             try:
-                self.server_io.authenticate(api_key)
+                self.client.authenticate(api_key)
 
             except AuthenticationException as e:
                 msg = "Authentication failed: API key is wrong!"
                 self.log.warning(msg)
                 self.log.debug(e)
                 break
             except requests.exceptions.ConnectionError:
@@ -559,21 +550,21 @@
 
             else:
                 # This is only executed if try-block executed without error.
                 success = True
                 break
 
         if success:
-            self.log.info(f"Node name: {self.server_io.name}")
+            self.log.info(f"Node name: {self.client.name}")
         else:
             self.log.critical('Unable to authenticate. Exiting')
             exit(1)
 
         # start thread to keep the connection alive by refreshing the token
-        self.server_io.auto_refresh_token()
+        self.client.auto_refresh_token()
 
     def private_key_filename(self) -> Path:
         """Get the path to the private key."""
 
         # FIXME: Code duplication: vantage6/cli/node.py uses a lot of the same
         #   logic. Suggest moving this to ctx.get_private_key()
         filename = self.config['encryption']["private_key"]
@@ -588,29 +579,29 @@
         # If ctx.get_data_file() receives an absolute path, its returned as-is
         fullpath = Path(self.ctx.get_data_file(filename))
 
         return fullpath
 
     def setup_encryption(self) -> None:
         """ Setup encryption if the node is part of encrypted collaboration """
-        encrypted_collaboration = self.server_io.is_encrypted_collaboration()
+        encrypted_collaboration = self.client.is_encrypted_collaboration()
         encrypted_node = self.config['encryption']["enabled"]
 
         if encrypted_collaboration != encrypted_node:
             # You can't force it if it just ain't right, you know?
             raise Exception("Expectations on encryption don't match?!")
 
         if encrypted_collaboration:
             self.log.warn('Enabling encryption!')
             private_key_file = self.private_key_filename()
-            self.server_io.setup_encryption(private_key_file)
+            self.client.setup_encryption(private_key_file)
 
         else:
             self.log.warn('Disabling encryption!')
-            self.server_io.setup_encryption(None)
+            self.client.setup_encryption(None)
 
     def _set_task_dir(self, ctx) -> None:
         """
         Set the task dir
 
         Parameters
         ----------
@@ -781,32 +772,29 @@
         """
         ovpn_file = os.path.join(self.__vpn_dir, VPN_CONFIG_FILE)
 
         self.log.info("Setting up VPN client container")
         vpn_volume_name = self.ctx.docker_vpn_volume_name \
             if ctx.running_in_docker else self.__vpn_dir
 
-        # FIXME: remove me in 4+. alpine image has been moved into the `images`
-        # key. This is to support older configuration files.
-        legacy_alpine = self.config.get('alpine')
-
         # user can specify custom images in the configuration file
         custom_alpine = self.config['images'].get('alpine') \
             if 'images' in self.config else None
         custom_vpn_client = self.config['images'].get('vpn_client') \
             if 'images' in self.config else None
         custom_network = self.config['images'].get('network_config') \
             if 'images' in self.config else None
 
         vpn_manager = VPNManager(
             isolated_network_mgr=isolated_network_mgr,
             node_name=self.ctx.name,
+            node_client=self.client,
             vpn_volume_name=vpn_volume_name,
             vpn_subnet=self.config.get('vpn_subnet'),
-            alpine_image=custom_alpine or legacy_alpine,
+            alpine_image=custom_alpine,
             vpn_client_image=custom_vpn_client,
             network_config_image=custom_network
         )
 
         if not self.config.get('vpn_subnet'):
             self.log.warn("VPN subnet is not defined! VPN disabled.")
         elif not os.path.isfile(ovpn_file):
@@ -839,15 +827,15 @@
         """
         do_try = True
         if connect_mode == VPNConnectMode.FIRST_TRY:
             self.log.debug("Using existing config file to connect to VPN")
             next_mode = VPNConnectMode.REFRESH_KEYPAIR
         elif connect_mode == VPNConnectMode.REFRESH_KEYPAIR:
             self.log.debug("Refreshing VPN keypair...")
-            do_try = self.server_io.refresh_vpn_keypair(ovpn_file=ovpn_file)
+            do_try = self.client.refresh_vpn_keypair(ovpn_file=ovpn_file)
             next_mode = VPNConnectMode.REFRESH_COMPLETE
         elif connect_mode == VPNConnectMode.REFRESH_COMPLETE:
             self.log.debug("Requesting new VPN configuration file...")
             do_try = self._get_vpn_config_file(ovpn_file)
             next_mode = None  # if new config file doesn't work, give up
 
         if do_try:
@@ -872,15 +860,15 @@
 
         Returns
         -------
         bool
             Whether or not configuration file was successfully obtained
         """
         # get the ovpn configuration from the server
-        success, ovpn_config = self.server_io.get_vpn_config()
+        success, ovpn_config = self.client.get_vpn_config()
         if not success:
             self.log.warn("Obtaining VPN configuration file not successful!")
             self.log.warn("Disabling node-to-node communication via VPN")
             return False
 
         # write ovpn config to node docker volume
         with open(ovpn_file, 'w') as f:
@@ -908,32 +896,32 @@
         self.socketIO = SocketIO(request_timeout=60, logger=debug_mode,
                                  engineio_logger=debug_mode)
 
         self.socketIO.register_namespace(NodeTaskNamespace('/tasks'))
         NodeTaskNamespace.node_worker_ref = self
 
         self.socketIO.connect(
-            url=f'{self.server_io.host}:{self.server_io.port}',
-            headers=self.server_io.headers,
+            url=f'{self.client.host}:{self.client.port}',
+            headers=self.client.headers,
             wait=False
         )
 
         # Log the outcome
         i = 0
         while not self.socketIO.connected:
             if i > TIME_LIMIT_INITIAL_CONNECTION_WEBSOCKET:
                 self.log.critical('Could not connect to the websocket '
                                   'channels, do you have a slow connection?')
                 exit(1)
             self.log.debug('Waiting for socket connection...')
             time.sleep(1)
             i += 1
 
-        self.log.info(f'Connected to host={self.server_io.host} on port='
-                      f'{self.server_io.port}')
+        self.log.info(f'Connected to host={self.client.host} on port='
+                      f'{self.client.port}')
 
         self.log.debug("Starting thread for to ping the server to notify this"
                        " node is online.")
         self.socketIO.start_background_task(self.__socket_ping_worker)
 
     def __socket_ping_worker(self) -> None:
         """
@@ -1000,37 +988,37 @@
             Dictionary received over websocket with instructions for which
             tasks to kill
 
         Returns
         -------
         list[dict]:
             List of dictionaries with information on killed task (keys:
-            result_id, task_id and parent_id)
+            run_id, task_id and parent_id)
         """
-        if kill_info['collaboration_id'] != self.server_io.collaboration_id:
+        if kill_info['collaboration_id'] != self.client.collaboration_id:
             self.log.debug(
                 "Not killing tasks as this node is in another collaboration."
             )
             return []
         elif 'node_id' in kill_info and \
-                kill_info['node_id'] != self.server_io.whoami.id_:
+                kill_info['node_id'] != self.client.whoami.id_:
             self.log.debug(
                 "Not killing tasks as instructions to kill tasks were directed"
                 " at another node in this collaboration.")
             return []
 
         # kill specific task if specified, else kill all algorithms
         kill_list = kill_info.get('kill_list')
         killed_algos = self.__docker.kill_tasks(
-            org_id=self.server_io.whoami.organization_id, kill_list=kill_list
+            org_id=self.client.whoami.organization_id, kill_list=kill_list
         )
         # update status of killed tasks
         for killed_algo in killed_algos:
-            self.server_io.patch_results(
-                id_=killed_algo.result_id, result={'status': TaskStatus.KILLED}
+            self.client.run.patch(
+                id_=killed_algo.run_id, data={'status': TaskStatus.KILLED}
             )
         return killed_algos
 
     def share_node_details(self) -> None:
         """
         Share part of the node's configuration with the server.
 
@@ -1047,30 +1035,35 @@
 
         encryption_config = self.config.get('encryption')
         if encryption_config:
             if encryption_config.get('enabled') is not None:
                 config_to_share['encryption'] = \
                     encryption_config.get('enabled')
 
-        # TODO v4+ remove the old 'allowed_images' key, it's now inside
-        # 'policies'. It's now overwritten below if 'policies' is set.
-        allowed_algos = self.config.get('allowed_images')
-        config_to_share['allowed_algorithms'] = allowed_algos \
-            if allowed_algos else 'all'
-
         # share node policies (e.g. who can run which algorithms)
         policies = self.config.get('policies', {})
         config_to_share['allowed_algorithms'] = \
             policies.get('allowed_algorithms', 'all')
         if policies.get('allowed_users') is not None:
             config_to_share['allowed_users'] = policies.get('allowed_users')
         if policies.get('allowed_organizations') is not None:
             config_to_share['allowed_orgs'] = \
                 policies.get('allowed_organizations')
 
+        # share node database labels and types
+        labels = []
+        types = {}
+        for db in self.config.get('databases', []):
+            label = db.get('label')
+            type_ = db.get('type')
+            labels.append(label)
+            types[f"db_type_{label}"] = type_
+        config_to_share['database_labels'] = labels
+        config_to_share['database_types'] = types
+
         self.log.debug(f"Sharing node configuration: {config_to_share}")
         self.socketIO.emit(
             'node_info_update', config_to_share, namespace='/tasks'
         )
 
     def cleanup(self) -> None:
```

### Comparing `vantage6-node-3.9.0rc4/vantage6/node/_version.py` & `vantage6-node-4.0.0a2/vantage6/node/_version.py`

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
 pre_release = f'' if version_info[3] == 'final' else \
   '.'+_specifier_[version_info[3]]+str(version_info[4])
 post_release = f'' if not version_info[5] else f'.post{version_info[5]}'
```

### Comparing `vantage6-node-3.9.0rc4/vantage6/node/cli/node.py` & `vantage6-node-4.0.0a2/vantage6/node/cli/node.py`

 * *Files 18% similar despite different names*

```diff
@@ -38,111 +38,94 @@
 #   list
 #
 @cli_node.command(name="list")
 def cli_node_list() -> None:
     """Lists all nodes in the default configuration directories."""
 
     # FIXME: use package 'table' for this.
-    click.echo("\nName"+(21*" ")+"Environments"+(21*" ")+"System/User")
+    click.echo("\nName"+(21*" ")+"System/User")
     click.echo("-" * 70)
 
     configs, f1 = NodeContext.available_configurations(system_folders=True)
     for config in configs:
-        click.echo(f"{config.name:25}{str(config.available_environments):32} "
-                   f"System ")
+        click.echo(f"{config.name:25} System ")
 
     configs, f2 = NodeContext.available_configurations(system_folders=False)
     for config in configs:
-        click.echo(f"{config.name:25}{str(config.available_environments):32} "
-                   f"User   ")
+        click.echo(f"{config.name:25} User   ")
 
     click.echo("-"*70)
     warning(f"Number of failed imports: "
             f"{Fore.YELLOW}{len(f1)+len(f2)}{Style.RESET_ALL}")
 
 
 #
 #   new
 #
 @cli_node.command(name="new")
 @click.option("-n", "--name", default=None, help="Configuration name")
-@click.option('-e', '--environment',
-              default=None,
-              help='Configuration environment to use')
 @click.option('--system', 'system_folders', flag_value=True,
               help="Use configuration from system folders (default)")
 @click.option('--user', 'system_folders', flag_value=False,
               default=constants.DEFAULT_NODE_SYSTEM_FOLDERS,
               help="Use configuration from user folders")
-def cli_node_new_configuration(name: str, environment: str,
-                               system_folders: bool) -> None:
+def cli_node_new_configuration(name: str, system_folders: bool) -> None:
     """Create a new configation file.
 
     Checks if the configuration already exists. If this is not the case
     a questionaire is invoked to create a new configuration file.
     """
     # select configuration name if none supplied
     if not name:
         name = q.text("Please enter a configuration-name:").ask()
         name_new = name.replace(" ", "-")
         if name != name_new:
             info(f"Replaced spaces from configuration name: {name}")
             name = name_new
 
-    if not environment:
-        environment = q.select(
-            "Please select the environment you want to configure:",
-            ["application", "prod", "acc", "test", "dev"]
-        ).ask()
-
     # Check that we can write in this folder
     if not check_config_writeable(system_folders):
         error("Your user does not have write access to all folders. Exiting")
         exit(1)
 
     # check that this config does not exist
-    if NodeContext.config_exists(name, environment, system_folders):
-        raise FileExistsError(f"Configuration {name} and environment"
-                              f"{environment} already exists!")
+    if NodeContext.config_exists(name, system_folders):
+        raise FileExistsError(f"Configuration {name} already exists!")
 
     # create config in ctx location
-    cfg_file = configuration_wizard("node", name, environment, system_folders)
+    cfg_file = configuration_wizard("node", name, system_folders)
     info(f"New configuration created: {Fore.GREEN}{cfg_file}{Style.RESET_ALL}")
 
 
 #
 #   files
 #
 @cli_node.command(name="files")
 @click.option("-n", "--name", default=None, help="Configuration name")
-@click.option('-e', '--environment',
-              default=constants.DEFAULT_NODE_ENVIRONMENT,
-              help='Configuration environment to use')
 @click.option('--system', 'system_folders', flag_value=True,
               help="Use configuration from system folders (default)")
 @click.option('--user', 'system_folders', flag_value=False,
               default=constants.DEFAULT_NODE_SYSTEM_FOLDERS,
               help="Use configuration from user folders")
-def cli_node_files(name: str, environment: str, system_folders: bool) -> None:
+def cli_node_files(name: str, system_folders: bool) -> None:
     """Print out the paths of important files.
 
     If the specified configuration cannot be found, it exits. Otherwise
     it returns the absolute path to the output.
     """
     # select configuration name if none supplied
-    name, environment = (name, environment) if name else \
+    name = name if name else \
         select_configuration_questionaire("node", system_folders)
 
     # raise error if config could not be found
-    if not NodeContext.config_exists(name, environment, system_folders):
+    if not NodeContext.config_exists(name, system_folders):
         raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), name)
 
     # create node context
-    ctx = NodeContext(name, environment=environment,
-                      system_folders=system_folders)
+    ctx = NodeContext(name, system_folders=system_folders)
 
     # return path of the configuration
     click.echo(f"Configuration file = {ctx.config_file}")
     click.echo(f"Log file           = {ctx.log_file}")
     click.echo(f"data folders       = {ctx.data_dir}")
     click.echo("Database labels and files:")
     for label, path in ctx.databases.items():
@@ -152,67 +135,59 @@
 #
 #   start
 #
 @cli_node.command(name='start')
 @click.option("-n", "--name", default=None, help="Configuration name")
 @click.option("-c", "--config", default=None,
               help='Absolute path to configuration-file; overrides "name"')
-@click.option('-e', '--environment',
-              default=constants.DEFAULT_NODE_ENVIRONMENT,
-              help='Configuration environment to use')
 @click.option('--system', 'system_folders', flag_value=True,
               help="Use configuration from system folders (default)")
 @click.option('--user', 'system_folders', flag_value=False,
               default=constants.DEFAULT_NODE_SYSTEM_FOLDERS,
               help="Use configuration from user folders")
 @click.option('--dockerized/-non-dockerized', default=False,
               help=("Whether to use DockerNodeContext or regular NodeContext "
                     "(default)"))
-def cli_node_start(name: str, config: str, environment: str,
-                   system_folders: bool, dockerized: bool) -> None:
+def cli_node_start(name: str, config: str, system_folders: bool,
+                   dockerized: bool) -> None:
     """Start the node instance.
 
     If no name or config is specified the default.yaml configuation is used.
-    In case the configuration file not excists, a questionaire is
-    invoked to create one. Note that in this case it is not possible to
-    specify specific environments for the configuration (e.g. test,
-    prod, acc).
+    In case the configuration file not exists, a questionaire is
+    invoked to create one.
     """
     ContextClass = DockerNodeContext if dockerized else NodeContext
 
     # in case a configuration file is given, we bypass all the helper
     # stuff since you know what you are doing
     if config:
         name = Path(config).stem
-        ctx = ContextClass(name, environment, system_folders, config)
+        ctx = ContextClass(name, system_folders, config)
 
     else:
         # in case no name is supplied, ask user to select one
         if not name:
-            name, environment = select_configuration_questionaire(
-                "node",
-                system_folders
-            )
+            name = select_configuration_questionaire("node", system_folders)
 
         # check that config exists in the APP, if not a questionaire will
         # be invoked
-        if not ContextClass.config_exists(name, environment, system_folders):
+        if not ContextClass.config_exists(name, system_folders):
             question = (
-                f"Configuration '{name}' using environment '{environment}' "
-                "does not exist.\n  Do you want to create this config now?"
+                f"Configuration '{name}' does not exist.\n  Do you want to "
+                "create this config now?"
             )
 
             if q.confirm(question).ask():
-                configuration_wizard("node", name, environment, system_folders)
+                configuration_wizard("node", name, system_folders)
 
             else:
                 sys.exit(0)
 
         # create dummy node context
-        ctx = ContextClass(name, environment, system_folders)
+        ctx = ContextClass(name, system_folders)
 
     # run the node application
     node.run(ctx)
 
 
 #
 #   version
```

### Comparing `vantage6-node-3.9.0rc4/vantage6/node/context.py` & `vantage6-node-4.0.0a2/vantage6/node/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,16 +59,15 @@
 
     INST_CONFIG_MANAGER = TestingConfigurationManager
     LOGGING_ENABLED = False
 
     @classmethod
     def from_external_config_file(cls, path):
         return super().from_external_config_file(
-            cls.test_config_location(),
-            "unittest", "application", True
+            cls.test_config_location(), "unittest", True
         )
 
     @staticmethod
     def test_config_location():
         return (PACKAGE_FOLDER / APPNAME /
                 "_data" / "unittest_config.yaml")
```

### Comparing `vantage6-node-3.9.0rc4/vantage6/node/docker/docker_base.py` & `vantage6-node-4.0.0a2/vantage6/node/docker/docker_base.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.9.0rc4/vantage6/node/docker/docker_manager.py` & `vantage6-node-4.0.0a2/vantage6/node/docker/docker_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,67 +24,66 @@
 from vantage6.common.docker.network_manager import NetworkManager
 from vantage6.cli.context import NodeContext
 from vantage6.node.context import DockerNodeContext
 from vantage6.node.docker.docker_base import DockerBaseManager
 from vantage6.node.docker.vpn_manager import VPNManager
 from vantage6.node.docker.task_manager import DockerTaskManager
 from vantage6.node.docker.squid import Squid
-from vantage6.node.server_io import NodeClient
+from vantage6.common.client.node_client import NodeClient
 from vantage6.node.docker.exceptions import (
     UnknownAlgorithmStartFail,
     PermanentAlgorithmStartFail,
     AlgorithmContainerNotFound
 )
 
 log = logging.getLogger(logger_name(__name__))
 
 
 class Result(NamedTuple):
-    # """ Data class to store the result of the docker image."""
     """
     Data class to store the result of the docker image.
 
     Attributes
     ----------
-    result_id: int
+    run_id: int
         ID of the current algorithm run
     logs: str
         Logs attached to current algorithm run
     data: str
         Output data of the algorithm
     status_code: int
         Status code of the algorithm run
     """
-    result_id: int
+    run_id: int
     task_id: int
     logs: str
     data: str
     status: str
     parent_id: int | None
 
 
 class ToBeKilled(NamedTuple):
     """ Data class to store which tasks should be killed """
     task_id: int
-    result_id: int
+    run_id: int
     organization_id: int
 
 
-class KilledResult(NamedTuple):
+class KilledRun(NamedTuple):
     """ Data class to store which algorithms have been killed """
-    result_id: int
+    run_id: int
     task_id: int
     parent_id: int
 
 
 class DockerManager(DockerBaseManager):
     """
     Wrapper for the docker-py module.
 
-    This classes manages tasks related to Docker, such as logging in to
+    This class manages tasks related to Docker, such as logging in to
     docker registries, managing input/output files, logs etc. Results
     can be retrieved through `get_result()` which returns the first available
     algorithm result.
     """
     log = logging.getLogger(logger_name(__name__))
 
     def __init__(self, ctx: DockerNodeContext | NodeContext,
@@ -123,17 +122,15 @@
 
         # keep track of the running containers
         self.active_tasks: list[DockerTaskManager] = []
 
         # keep track of the containers that have failed to start
         self.failed_tasks: list[DockerTaskManager] = []
 
-        # before a task is executed it gets exposed to these regex
-        # TODO remove in v4+ as it is supersed by the 'policies' block
-        self._allowed_images = config.get("allowed_images")
+        # before a task is executed it gets exposed to these policies
         self._policies = config.get("policies", {})
 
         # node name is used to identify algorithm containers belonging
         # to this node. This is required as multiple nodes may run at
         # a single machine sharing the docker daemon while using a
         # different server. Using a different server means that there
         # could be duplicate result_id's running at the node at the same
@@ -165,29 +162,15 @@
         Set database location and whether or not it is a file
 
         Parameters
         ----------
         databases: dict | list
             databases as specified in the config file
         """
-
-        # Check wether the new or old database config is used.
-        # TODO: we should remove the old way in v4+
-        old_format = isinstance(databases, dict)
-
-        # Check that the `default` database label is present. If this is
-        # not the case, older algorithms will break
-        if old_format:
-            db_labels = databases.keys()
-        else:
-            db_labels = [db['label'] for db in databases]
-
-        if 'default' not in db_labels:
-            self.log.error("'default' database not specified in the config!")
-            self.log.debug(f'databases in config={db_labels}')
+        db_labels = [db['label'] for db in databases]
 
         # If we're running in a docker container, database_uri would point
         # to a path on the *host* (since it's been read from the config
         # file). That's no good here. Therefore, we expect the CLI to set
         # the environment variables for us. This has the added bonus that we
         # can override the URI from the command line as well.
         self.databases = {}
@@ -195,17 +178,20 @@
             label_upper = label.upper()
             db_config = get_database_config(databases, label)
             if running_in_docker():
                 uri = os.environ[f'{label_upper}_DATABASE_URI']
             else:
                 uri = db_config['uri']
 
-            db_is_file = Path(uri).exists()
-            if running_in_docker() and db_is_file:
-                uri = f'/mnt/{uri}'
+            if running_in_docker():
+                db_is_file = Path(f'/mnt/{uri}').exists()
+                if db_is_file:
+                    uri = f'/mnt/{uri}'
+            else:
+                db_is_file = Path(uri).exists()
 
             if db_is_file:
                 # We'll copy the file to the folder `data` in our task_dir.
                 self.log.info(f'Copying {uri} to {self.__tasks_dir}')
                 shutil.copy(uri, self.__tasks_dir)
                 uri = self.__tasks_dir / os.path.basename(uri)
 
@@ -233,15 +219,15 @@
         self.algorithm_device_requests = device_requests
 
     def create_volume(self, volume_name: str) -> None:
         """
         Create a temporary volume for a single run.
 
         A single run can consist of multiple algorithm containers. It is
-        important to note that all algorithm containers having the same run_id
+        important to note that all algorithm containers having the same job_id
         have access to this container.
 
         Parameters
         ----------
         volume_name: str
             Name of the volume to be created
         """
@@ -294,88 +280,73 @@
                               " node does not allow to run.")
                 return False
 
         # check if user or their organization is allowed
         allowed_users = self._policies.get('allowed_users', [])
         allowed_orgs = self._policies.get('allowed_organizations', [])
         if allowed_users or allowed_orgs:
-            # TODO in v4+, simpify this logic when part below is removed (
-            # simply return the result of the check_user_allowed_to_send_task)
             is_allowed = self.client.check_user_allowed_to_send_task(
-                allowed_users, allowed_orgs, task_info['initiator'],
-                task_info['init_user']
+                allowed_users, allowed_orgs, task_info['init_org']['id'],
+                task_info['init_user']['id']
             )
             if not is_allowed:
-                self.log.warn(
-                    "A task was sent by a user or organization that this node"
-                    " does not allow to start tasks.")
+                self.log.warn("A task was sent by a user or organization that "
+                              "this node does not allow to start tasks.")
                 return False
 
-        # --------------------------------------------------------------------
-        # TODO in v4+, remove part below as it is superseded by the 'policies'
-        # block
-        # --------------------------------------------------------------------
-        # if no limits are declared
-        if not self._allowed_images:
+        # if no limits are declared, log warning
+        if not self._policies:
             self.log.warn("All docker images are allowed on this Node!")
-            return True
-
-        # check if it matches any of the regex cases
-        for regex_expr in self._allowed_images:
-            expr_ = re.compile(regex_expr)
-            if expr_.match(docker_image_name):
-                return True
 
-        # if not, it is considered an illegal image
-        return False
+        return True
 
-    def is_running(self, result_id: int) -> bool:
+    def is_running(self, run_id: int) -> bool:
         """
-        Check if a container is already running for <result_id>.
+        Check if a container is already running for <run_id>.
 
         Parameters
         ----------
-        result_id: int
-            result_id of the algorithm container to be found
+        run_id: int
+            run_id of the algorithm container to be found
 
         Returns
         -------
         bool
             Whether or not algorithm container is running already
         """
         running_containers = self.docker.containers.list(filters={
             "label": [
                 f"{APPNAME}-type=algorithm",
                 f"node={self.node_name}",
-                f"result_id={result_id}"
+                f"run_id={run_id}"
             ]
         })
         return bool(running_containers)
 
-    def cleanup_tasks(self) -> list[KilledResult]:
+    def cleanup_tasks(self) -> list[KilledRun]:
         """
         Stop all active tasks
 
         Returns
         -------
-        list[KilledResult]:
+        list[KilledRun]:
             List of information on tasks that have been killed
         """
-        result_ids_killed = []
+        run_ids_killed = []
         if self.active_tasks:
             self.log.debug(f'Killing {len(self.active_tasks)} active task(s)')
         while self.active_tasks:
             task = self.active_tasks.pop()
             task.cleanup()
-            result_ids_killed.append(KilledResult(
-                result_id=task.result_id,
+            run_ids_killed.append(KilledRun(
+                run_id=task.run_id,
                 task_id=task.task_id,
                 parent_id=task.parent_id
             ))
-        return result_ids_killed
+        return run_ids_killed
 
     def cleanup(self) -> None:
         """
         Stop all active tasks and delete the isolated network
 
         Note: the temporary docker volumes are kept as they may still be used
         by a master container
@@ -390,87 +361,88 @@
         # remove the node container from the network, it runs this code.. so
         # it does not make sense to delete it just yet
         self.isolated_network_mgr.disconnect(self.node_container_name)
 
         # remove the connected containers and the network
         self.isolated_network_mgr.delete(kill_containers=True)
 
-    def run(self, result_id: int, task_info: dict, image: str,
-            docker_input: bytes, tmp_vol_name: str, token: str, database: str
-            ) -> list[dict] | None:
+    def run(self, run_id: int, task_info: dict, image: str,
+            docker_input: bytes, tmp_vol_name: str, token: str,
+            databases_to_use: list[str]
+            ) -> tuple[TaskStatus, list[dict] | None]:
         """
         Checks if docker task is running. If not, creates DockerTaskManager to
         run the task
 
         Parameters
         ----------
-        result_id: int
-            Server result identifier
+        run_id: int
+            Server run identifier
         task_info: dict
             Dictionary with task information
         image: str
             Docker image name
         docker_input: bytes
             Input that can be read by docker container
         tmp_vol_name: str
             Name of temporary docker volume assigned to the algorithm
         token: str
             Bearer token that the container can use
-        database: str
-            Name of the Database to use
+        databases_to_use: list[str]
+            Labels of the databases to use
 
         Returns
         -------
-        list[dict] | None
-            Description of each port on the VPN client that forwards traffic to
-            the algo container. None if VPN is not set up.
+        TaskStatus, list[dict] | None
+            Returns a tuple with the status of the task and a description of
+            each port on the VPN client that forwards traffic to the algorithm
+            container (``None`` if VPN is not set up).
         """
         # Verify that an allowed image is used
         if not self.is_docker_image_allowed(image, task_info):
             msg = f"Docker image {image} is not allowed on this Node!"
             self.log.critical(msg)
             return TaskStatus.NOT_ALLOWED,  None
 
         # Check that this task is not already running
-        if self.is_running(result_id):
+        if self.is_running(run_id):
             self.log.warn("Task is already being executed, discarding task")
-            self.log.debug(f"result_id={result_id} is discarded")
+            self.log.debug(f"run_id={run_id} is discarded")
             return TaskStatus.ACTIVE, None
 
         task = DockerTaskManager(
             image=image,
-            result_id=result_id,
+            run_id=run_id,
             task_info=task_info,
             vpn_manager=self.vpn_manager,
             node_name=self.node_name,
             tasks_dir=self.__tasks_dir,
             isolated_network_mgr=self.isolated_network_mgr,
             databases=self.databases,
             docker_volume_name=self.data_volume_name,
             alpine_image=self.alpine_image,
             proxy=self.proxy,
             device_requests=self.algorithm_device_requests
         )
-        database = database if (database and len(database)) else 'default'
 
         # attempt to kick of the task. If it fails do to unknown reasons we try
         # again. If it fails permanently we add it to the failed tasks to be
         # handled by the speaking worker of the node
         attempts = 1
         while not (task.status == TaskStatus.ACTIVE) and attempts < 3:
             try:
                 vpn_ports = task.run(
                     docker_input=docker_input, tmp_vol_name=tmp_vol_name,
                     token=token, algorithm_env=self.algorithm_env,
-                    database=database
+                    databases_to_use=databases_to_use
                 )
 
             except UnknownAlgorithmStartFail:
-                self.log.exception(f'Failed to start result {result_id} due '
-                                   'to unknown reason. Retrying')
+                self.log.exception(f'Failed to start run {run_id} for an '
+                                   'unknown reason. Retrying...')
                 time.sleep(1)  # add some time before retrying the next attempt
 
             except PermanentAlgorithmStartFail:
                 break
 
             attempts += 1
 
@@ -517,38 +489,38 @@
             # sleep for a second before checking again
             time.sleep(1)
 
         if finished_tasks:
             # at least one task is finished
 
             finished_task = finished_tasks.pop()
-            self.log.debug(f"Result id={finished_task.result_id} is finished")
+            self.log.debug(f"Run id={finished_task.run_id} is finished")
 
             # Check exit status and report
             logs = finished_task.report_status()
 
             # Cleanup containers
             finished_task.cleanup()
 
             # Retrieve results from file
             results = finished_task.get_results()
 
             # remove the VPN ports of this run from the database
             self.client.request(
-                'port', params={'result_id': finished_task.result_id},
+                'port', params={'run_id': finished_task.run_id},
                 method="DELETE"
             )
         else:
             # at least one task failed to start
             finished_task = self.failed_tasks.pop()
             logs = 'Container failed'
             results = b''
 
         return Result(
-            result_id=finished_task.result_id,
+            run_id=finished_task.run_id,
             task_id=finished_task.task_id,
             logs=logs,
             data=results,
             status=finished_task.status,
             parent_id=finished_task.parent_id,
         )
 
@@ -598,87 +570,87 @@
             container_name=container_name,
             aliases=[config_alias]
         )
         self.linked_services.append(container_name)
 
     def kill_selected_tasks(
         self, org_id: int, kill_list: list[ToBeKilled] = None
-    ) -> list[KilledResult]:
+    ) -> list[KilledRun]:
         """
         Kill tasks specified by a kill list, if they are currently running on
         this node
 
         Parameters
         ----------
         org_id: int
             The organization id of this node
         kill_list: list[ToBeKilled]
             A list of info about tasks that should be killed.
 
         Returns
         -------
-        list[KilledResult]
+        list[KilledRun]
             List with information on killed tasks
         """
         killed_list = []
         for container_to_kill in kill_list:
             if container_to_kill['organization_id'] != org_id:
-                continue  # this result is on another node
+                continue  # this run is on another node
             # find the task
             task = next((
                 t for t in self.active_tasks
-                if t.result_id == container_to_kill['result_id']
+                if t.run_id == container_to_kill['run_id']
             ), None)
             if task:
                 self.log.info(
-                    f"Killing containers for result_id={task.result_id}")
+                    f"Killing containers for run_id={task.run_id}")
                 self.active_tasks.remove(task)
                 task.cleanup()
-                killed_list.append(KilledResult(
-                    result_id=task.result_id,
+                killed_list.append(KilledRun(
+                    run_id=task.run_id,
                     task_id=task.task_id,
                     parent_id=task.parent_id,
                 ))
             else:
                 self.log.warn(
-                    "Received instruction to kill result_id="
-                    f"{container_to_kill['result_id']}, but it was not "
+                    "Received instruction to kill run_id="
+                    f"{container_to_kill['run_id']}, but it was not "
                     "found running on this node.")
         return killed_list
 
     def kill_tasks(self, org_id: int,
-                   kill_list: list[ToBeKilled] = None) -> list[KilledResult]:
+                   kill_list: list[ToBeKilled] = None) -> list[KilledRun]:
         """
         Kill tasks currently running on this node.
 
         Parameters
         ----------
         org_id: int
             The organization id of this node
         kill_list: list[ToBeKilled] (optional)
             A list of info on tasks that should be killed. If the list
             is not specified, all running algorithm containers will be killed.
 
         Returns
         -------
-        list[KilledResult]
+        list[KilledRun]
             List of dictionaries with information on killed tasks
         """
         if kill_list:
-            killed_results = self.kill_selected_tasks(org_id=org_id,
-                                                      kill_list=kill_list)
+            killed_runs = self.kill_selected_tasks(org_id=org_id,
+                                                   kill_list=kill_list)
         else:
             # received instruction to kill all tasks on this node
             self.log.warn(
                 "Received instruction from server to kill all algorithms "
                 "running on this node. Executing that now...")
-            killed_results = self.cleanup_tasks()
-            if len(killed_results):
+            killed_runs = self.cleanup_tasks()
+            if len(killed_runs):
                 self.log.warn(
-                    "Killed the following result ids as instructed via socket:"
-                    f" {', '.join([str(r.result_id) for r in killed_results])}"
+                    "Killed the following run ids as instructed via socket:"
+                    f" {', '.join([str(r.run_id) for r in killed_runs])}"
                 )
             else:
                 self.log.warn(
                     "Instructed to kill tasks but none were running"
                 )
-        return killed_results
+        return killed_runs
```

### Comparing `vantage6-node-3.9.0rc4/vantage6/node/docker/exceptions.py` & `vantage6-node-4.0.0a2/vantage6/node/docker/exceptions.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.9.0rc4/vantage6/node/docker/squid.py` & `vantage6-node-4.0.0a2/vantage6/node/docker/squid.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 The Squid container is used to whitelist ips, domains and ports for the
 algorithm container. This can then be used by the algorithm containers to
 access the data sources or other services.
 """
 import logging
 import os
 
-from typing import NamedTuple
+from dataclasses import dataclass, field, asdict
 from jinja2 import Environment, FileSystemLoader
 from pathlib import Path
 
 from vantage6.common import logger_name
 from vantage6.common.globals import APPNAME
 from vantage6.common.docker.addons import (
     remove_container,
@@ -24,18 +24,19 @@
 from vantage6.node.docker.docker_base import DockerBaseManager
 from vantage6.node.docker.docker_manager import NetworkManager
 from vantage6.node.globals import SQUID_IMAGE, PACKAGE_FOLDER
 
 log = logging.getLogger(logger_name(__name__))
 
 
-class SquidConfig(NamedTuple):
-    domains: list[str]
-    ips: list[str]
-    ports: list[int]
+@dataclass
+class SquidConfig:
+    domains: list[str] = field(default_factory=lambda: [])
+    ips: list[str] = field(default_factory=lambda: [])
+    ports: list[int] = field(default_factory=lambda: [])
 
 
 class Squid(DockerBaseManager):
 
     def __init__(self, isolated_network_mgr: NetworkManager, config: dict,
                  node_name: str, config_volume: str,
                  squid_image: str | None = None) -> None:
@@ -81,16 +82,16 @@
         self.hostname = 'squid'
         # This is the default port of the squid container, which is exposed
         # to the algorithm containers.
         self.port = 3128
         log.debug(f"Squid hostname: {self.hostname}, port: {self.port}")
 
         try:
-            # Create the SSH configuration, which can later be mounted by the
-            # SSH tunnel container
+            # Create squid configuration, which can later be mounted by the
+            # squid container
             self.squid_config = self.read_config(config)
         except KeyError as e:
             # parent class should handle this
             raise KeyError(f"Invalid Squid configuration: {e}")
 
         log.debug(f"Squid configuration: {self.squid_config}")
 
@@ -153,14 +154,20 @@
         for ip in whitelist.ips:
             if not any(ip.startswith(safe_ip) for safe_ip in safe_ips):
                 log.warning("Whitelist contains non-internal IP addresses!")
                 log.warning("This is not safe!")
                 log.debug(f"Whitelisted IP: {ip}")
                 safe = False
 
+        if not (has_domains or len(whitelist.ips) > 0):
+            log.critical("No domains or IP addresses are whitelisted!")
+
+        if not len(whitelist.ports) > 0:
+            log.critical("No ports are whitelisted!")
+
         return safe
 
     @staticmethod
     def read_config(config: dict) -> SquidConfig:
         """
         Read the Squid configuration from the config
 
@@ -210,15 +217,15 @@
                 PACKAGE_FOLDER / APPNAME / "node" / "template"
             ),
             autoescape=True
         )
         template = environment.get_template("squid.conf.j2")
 
         # inject template with vars
-        squid_config = template.render(**config._asdict())
+        squid_config = template.render(**asdict(config))
 
         with open(self.config_folder / "squid.conf", "w") as f:
             f.write(squid_config)
 
         # This is done also in the container, however vnode-local breaks
         # if we dont do it here
         os.chmod(self.config_folder / "squid.conf", 0o600)
```

### Comparing `vantage6-node-3.9.0rc4/vantage6/node/docker/ssh_tunnel.py` & `vantage6-node-4.0.0a2/vantage6/node/docker/ssh_tunnel.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.9.0rc4/vantage6/node/docker/task_manager.py` & `vantage6-node-4.0.0a2/vantage6/node/docker/task_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-""" TODO the task folder is also created by this class. This folder needs
-to be cleaned at some point. """
+# TODO the task folder is also created by this class. This folder needs
+# to be cleaned at some point.
 import logging
 import os
-import pickle
 import docker.errors
 import json
 
 from pathlib import Path
 
 from vantage6.common.globals import APPNAME
 from vantage6.common.docker.addons import (
@@ -34,15 +33,15 @@
     Ensures that the environment is properly set up (docker volumes,
     directories, environment variables, etc). Then runs the algorithm as a
     docker container. Finally, it monitors the container state and can return
     it's results when the algorithm finished.
     """
 
     def __init__(self, image: str, vpn_manager: VPNManager, node_name: str,
-                 result_id: int, task_info: dict, tasks_dir: Path,
+                 run_id: int, task_info: dict, tasks_dir: Path,
                  isolated_network_mgr: NetworkManager,
                  databases: dict, docker_volume_name: str,
                  alpine_image: str | None = None, proxy: Squid | None = None,
                  device_requests: list | None = None):
         """
         Initialization creates DockerTaskManager instance
 
@@ -50,16 +49,16 @@
         ----------
         image: str
             Name of docker image to be run
         vpn_manager: VPNManager
             VPN manager required to set up traffic forwarding via VPN
         node_name: str
             Name of the node, to track running algorithms
-        result_id: int
-            Server result identifier
+        run_id: int
+            Algorithm run identifier
         task_info: dict
             Dictionary with info about the task
         tasks_dir: Path
             Directory in which this task's data are stored
         isolated_network_mgr: NetworkManager
             Manager of isolated network to which algorithm needs to connect
         databases: dict
@@ -74,15 +73,16 @@
         """
         self.task_id = task_info['id']
         self.log = logging.getLogger(f"task ({self.task_id})")
 
         super().__init__(isolated_network_mgr)
         self.image = image
         self.__vpn_manager = vpn_manager
-        self.result_id = result_id
+        self.run_id = run_id
+        self.task_id = task_info['id']
         self.parent_id = get_parent_id(task_info)
         self.__tasks_dir = tasks_dir
         self.databases = databases
         self.data_volume_name = docker_volume_name
         self.node_name = node_name
         self.alpine_image = ALPINE_IMAGE if alpine_image is None \
             else alpine_image
@@ -91,15 +91,15 @@
         self.container = None
         self.status_code = None
         self.docker_input = None
 
         self.labels = {
             f"{APPNAME}-type": "algorithm",
             "node": node_name,
-            "result_id": str(result_id)
+            "run_id": str(run_id)
         }
         self.helper_labels = self.labels.copy()
         self.helper_labels[f"{APPNAME}-type"] = "algorithm-helper"
 
         # FIXME: these values should be retrieved from DockerNodeContext
         #   in some way.
         self.tmp_folder = "/mnt/tmp"
@@ -182,16 +182,18 @@
             raise PermanentAlgorithmStartFail
         except Exception as e:
             self.log.debug('Failed to pull image')
             self.log.exception(e)
             self.status = TaskStatus.FAILED
             raise PermanentAlgorithmStartFail
 
-    def run(self, docker_input: bytes, tmp_vol_name: str, token: str,
-            algorithm_env: dict, database: str) -> list[dict] | None:
+    def run(
+        self, docker_input: bytes, tmp_vol_name: str, token: str,
+        algorithm_env: dict, databases_to_use: list[str]
+    ) -> list[dict] | None:
         """
         Runs the docker-image in detached mode.
 
         It will will attach all mounts (input, output and datafile) to the
         docker image. And will supply some environment variables.
 
         Parameters
@@ -200,14 +202,16 @@
             Input that can be read by docker container
         tmp_vol_name: str
             Name of temporary docker volume assigned to the algorithm
         token: str
             Bearer token that the container can use
         algorithm_env: dict
             Dictionary with additional environment variables to set
+        databases_to_use: list[str]
+            List of labels of databases to use in the task
 
         Returns
         -------
         list[dict] | None
             Description of each port on the VPN client that forwards traffic to
             the algo container. None if VPN is not set up.
         """
@@ -218,40 +222,40 @@
         self.docker_input = docker_input
         self.volumes = self._prepare_volumes(tmp_vol_name, token)
         self.log.debug(f"volumes: {self.volumes}")
 
         # setup environment variables
         self.environment_variables = \
             self._setup_environment_vars(algorithm_env=algorithm_env,
-                                         database=database)
+                                         databases_to_use=databases_to_use)
 
         # run the algorithm as docker container
         vpn_ports = self._run_algorithm()
         return vpn_ports
 
     def cleanup(self) -> None:
         """Cleanup the containers generated for this task"""
         remove_container(self.helper_container, kill=True)
         remove_container(self.container, kill=True)
 
-    def _run_algorithm(self) -> list[dict]:
+    def _run_algorithm(self) -> list[dict] | None:
         """
         Run the algorithm container
 
         Start up a helper container to complete VPN setup, pull the latest
         image and then run the algorithm
 
         Returns
         -------
         list[dict] or None
             Description of each port on the VPN client that forwards traffic to
             the algo container. None if VPN is inactive
         """
         vpn_ports = None
-        container_name = f'{APPNAME}-{self.node_name}-result-{self.result_id}'
+        container_name = f'{APPNAME}-{self.node_name}-run-{self.run_id}'
         helper_container_name = container_name + '-helper'
 
         # Try to pull the latest image
         self.pull()
 
         # remove algorithm containers if they were already running
         self.log.debug("Check if algorithm container is already running")
@@ -281,19 +285,21 @@
             self.log.debug("Setup port forwarder")
             vpn_ports = self.__vpn_manager.forward_vpn_traffic(
                 helper_container=self.helper_container,
                 algo_image_name=self.image
             )
 
         # try reading docker input
+        # FIXME BvB 2023-02-03: why do we read docker input here? It is never
+        # really used below. Should it?
         deserialized_input = None
         if self.docker_input:
             self.log.debug("Deserialize input")
             try:
-                deserialized_input = pickle.loads(self.docker_input)
+                deserialized_input = json.loads(self.docker_input)
             except Exception:
                 pass
 
         # attempt to run the image
         try:
             if deserialized_input:
                 self.log.info(f"Run docker image {self.image} with input "
@@ -350,15 +356,15 @@
         #   from windows to unix several times...).
 
         # If we're running in docker __tasks_dir will point to a location on
         # the data volume.
         # Alternatively, if we're not running in docker it should point to the
         # folder on the host that can act like a data volume. In both cases,
         # we can just copy the required files to it
-        self.task_folder_name = f"task-{self.result_id:09d}"
+        self.task_folder_name = f"task-{self.run_id:09d}"
         self.task_folder_path = \
             os.path.join(self.__tasks_dir, self.task_folder_name)
         os.makedirs(self.task_folder_path, exist_ok=True)
         self.output_file = os.path.join(self.task_folder_path, "output")
 
     def _prepare_volumes(self, tmp_vol_name: str, token: str) -> dict:
         """
@@ -402,24 +408,24 @@
                 {"bind": self.data_folder, "mode": "rw"}
         else:
             volumes[self.__tasks_dir] = \
                 {"bind": self.data_folder, "mode": "rw"}
         return volumes
 
     def _setup_environment_vars(self, algorithm_env: dict,
-                                database: str = 'default') -> dict:
+                                databases_to_use: list[str]) -> dict:
         """"
         Set environment variables required to run the algorithm
 
         Parameters
         ----------
         algorithm_env: dict
             Dictionary with additional environment variables to set
-        database: str
-            Label of the database to use
+        databases_to_use: list[str]
+            Labels of the databases to use
 
         Returns
         -------
         dict:
             Environment variables required to run algorithm
         """
         try:
@@ -468,24 +474,26 @@
             no_proxy.append("localhost")
             no_proxy.append(proxy_host)
 
             # Add the NO_PROXY and no_proxy environment variable.
             environment_variables["NO_PROXY"] = ', '.join(no_proxy)
             environment_variables["no_proxy"] = ', '.join(no_proxy)
 
-        if database in self.databases:
-            environment_variables["USER_REQUESTED_DATABASE_LABEL"] = database
-        else:
-            # In this case the algorithm might crash if it tries to access
-            # the DATABASE_LABEL environment variable
-            self.log.warning("A user specified a database that does not "
-                             "exist. Available databases are: "
-                             f"{', '.join(list(self.databases.keys()))}. This "
-                             "is likely to result in an algorithm crash.")
-            self.log.debug(f"User specified database: {database}")
+        for database in databases_to_use:
+            if database not in self.databases:
+                # In this case the algorithm might crash if it tries to access
+                # the DATABASE_LABEL environment variable
+                self.log.warning("A user specified a database that does not "
+                                 "exist. Available databases are: "
+                                 f"{self.databases.keys()}. This is likely to "
+                                 "result in an algorithm crash.")
+                self.log.debug(f"User specified database: {database}")
+
+        environment_variables["USER_REQUESTED_DATABASE_LABELS"] = \
+            ",".join(databases_to_use)
 
         # Only prepend the data_folder is it is a file-based database
         # This allows algorithms to access multiple data sources at the
         # same time
         db_labels = []
         for label in self.databases:
             db = self.databases[label]
@@ -497,26 +505,14 @@
 
             type_var_name = f'{label.upper()}_DATABASE_TYPE'
             environment_variables[type_var_name] = db['type']
 
             db_labels.append(label)
         environment_variables['DB_LABELS'] = json.dumps(db_labels)
 
-        # Support legacy algorithms
-        # TODO remove in v4+
-        try:
-            environment_variables["DATABASE_URI"] = (
-                f"{self.data_folder}/"
-                f"{os.path.basename(self.databases[database]['uri'])}"
-            )
-        except KeyError as e:
-            self.log.error(f"'{database}' database missing! This could crash "
-                           "legacy algorithms")
-            self.log.debug(e)
-
         self.log.debug(f"environment: {environment_variables}")
 
         # Load additional environment variables
         if algorithm_env:
             environment_variables = \
                 {**environment_variables, **algorithm_env}
             self.log.info('Custom environment variables are loaded!')
```

### Comparing `vantage6-node-3.9.0rc4/vantage6/node/docker/vpn_manager.py` & `vantage6-node-4.0.0a2/vantage6/node/docker/vpn_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,32 +8,33 @@
 from docker.models.containers import Container
 
 from vantage6.common import logger_name
 from vantage6.common.globals import APPNAME, VPN_CONFIG_FILE
 from vantage6.common.docker.addons import (
     remove_container_if_exists, remove_container, pull_if_newer
 )
+from vantage6.common.docker.network_manager import NetworkManager
 from vantage6.node.globals import (
     MAX_CHECK_VPN_ATTEMPTS, NETWORK_CONFIG_IMAGE, VPN_CLIENT_IMAGE,
     FREE_PORT_RANGE, DEFAULT_ALGO_VPN_PORT, ALPINE_IMAGE
 )
-from vantage6.common.docker.network_manager import NetworkManager
+from vantage6.common.client.node_client import NodeClient
 from vantage6.node.docker.docker_base import DockerBaseManager
 
 
 class VPNManager(DockerBaseManager):
     """
     Setup a VPN client in a Docker container and configure the network so that
     the VPN container can forward traffic to and from algorithm containers.
     """
     log = logging.getLogger(logger_name(__name__))
 
     def __init__(self, isolated_network_mgr: NetworkManager,
-                 node_name: str, vpn_volume_name: str, vpn_subnet: str,
-                 alpine_image: str | None = None,
+                 node_name: str, node_client: NodeClient, vpn_volume_name: str,
+                 vpn_subnet: str, alpine_image: str | None = None,
                  vpn_client_image: str | None = None,
                  network_config_image: str | None = None) -> None:
         """
         Initializes a VPN manager instance
 
         Parameters
         ----------
@@ -52,14 +53,15 @@
         network_config_image: str | None
             Name of alternative network config image to be used
         """
         super().__init__(isolated_network_mgr)
 
         self.vpn_client_container_name = f'{APPNAME}-{node_name}-vpn-client'
         self.vpn_volume_name = vpn_volume_name
+        self.client = node_client
         self.subnet = vpn_subnet
         self.alpine_image = ALPINE_IMAGE if not alpine_image \
             else alpine_image
         self.vpn_client_image = VPN_CLIENT_IMAGE if not vpn_client_image else \
             vpn_client_image
         self.network_config_image = NETWORK_CONFIG_IMAGE \
             if not network_config_image else network_config_image
@@ -134,14 +136,17 @@
 
         # check successful initiation of VPN connection
         if self.has_connection():
             self.log.info("VPN client container was successfully started!")
         else:
             raise ConnectionError("VPN connection not established!")
 
+        # send VPN IP address to server
+        self.send_vpn_ip_to_server()
+
         # check that the VPN connection IP address is part of the subnet
         # defined in the node configuration. If not, the VPN connection would
         # not work.
         if not self._vpn_in_right_subnet():
             self.log.error(
                 "The VPN subnet defined in the node configuration file does "
                 "not match the VPN server subnet. Turning off VPN..."
@@ -197,14 +202,17 @@
         """
         if not self.has_vpn:
             return
         self.has_vpn = False
         self.log.debug("Stopping and removing the VPN client container")
         remove_container(self.vpn_client_container, kill=True)
 
+        # clear VPN IP address from server
+        self.send_vpn_ip_to_server()
+
         # Clean up host network changes. We have added two rules to the front
         # of the DOCKER-USER chain. We now execute more or less the same
         # commands, but with -D (delete) instead of -I (insert)
         if cleanup_host_rules:
             command = (
                 'sh -c "'
                 f'iptables -D DOCKER-USER -d {self.subnet} '
@@ -242,14 +250,30 @@
         except (JSONDecodeError, docker.errors.APIError):
             # JSONDecodeError if VPN is not setup yet, APIError if VPN
             # container is restarting (e.g. due to connection errors)
             raise ConnectionError(
                 "Could not get VPN IP: VPN is not connected!")
         return vpn_interface[0]['addr_info'][0]['local']
 
+    def send_vpn_ip_to_server(self) -> None:
+        """
+        Send VPN IP address to the server
+        """
+        node_id = self.client.whoami.id_
+        if self.has_vpn:
+            node_ip = self.get_vpn_ip()
+            self.client.request(
+                f"node/{node_id}", json={"ip": node_ip}, method="PATCH"
+            )
+        else:
+            # VPN is disconnected, send NULL IP address
+            self.client.request(
+                f"node/{node_id}", json={"clear_ip": True}, method="PATCH"
+            )
+
     def forward_vpn_traffic(self, helper_container: Container,
                             algo_image_name: str) -> list[dict] | None:
         """
         Setup rules so that traffic is properly forwarded between the VPN
         container and the algorithm container (and its helper container)
 
         Parameters
@@ -322,37 +346,45 @@
             Description of each port on the VPN client that forwards traffic to
             the algo container. None if VPN is not set up.
         """
         if not self.has_vpn:
             return None  # no port assigned if no VPN is available
 
         # Get IP Address of the algorithm container
+        self.log.debug("Getting IP address of algorithm container")
         algo_helper_container.reload()  # update attributes
         algo_ip = self.get_isolated_netw_ip(algo_helper_container)
 
         # Set ports at which algorithm containers receive traffic
+        self.log.debug("Finding exposed ports of algorithm container")
         ports = self._find_exposed_ports(algo_image_name)
 
         # Find ports on VPN container that are already occupied
         cmd = (
             'sh -c '
-            '"iptables -t nat -L PREROUTING | awk \'{print $7}\' | cut -c 5-"'
+            '"iptables -t nat -L PREROUTING -n | '
+            'awk \'{print $7}\' | cut -c 5-"'
         )
         occupied_ports = self.vpn_client_container.exec_run(cmd=cmd)
+
         occupied_ports = occupied_ports.output.decode('utf-8')
         occupied_ports = occupied_ports.split('\n')
         occupied_ports = \
             [int(port) for port in occupied_ports if port != '']
+        self.log.debug(f"Occupied ports: {occupied_ports}")
 
         # take first available port
         vpn_client_port_options = set(FREE_PORT_RANGE) - set(occupied_ports)
         for port in ports:
-            port['port'] = vpn_client_port_options.pop()
+            port_ = vpn_client_port_options.pop()
+            self.log.debug(f"Assigning port {port_} to algorithm port")
+            port['port'] = port_
 
         vpn_ip = self.get_vpn_ip()
+        self.log.debug(f"VPN IP: {vpn_ip}")
 
         # Set up forwarding VPN traffic to algorithm container
         command = 'sh -c "'
         for port in ports:
             # Rule for directing external vpn traffic to algorithms
             command += (
                 'iptables -t nat -A PREROUTING -i tun0 -p tcp '
```

### Comparing `vantage6-node-3.9.0rc4/vantage6/node/globals.py` & `vantage6-node-4.0.0a2/vantage6/node/globals.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,17 +2,14 @@
 from vantage6.common.globals import APPNAME
 
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
 
 NODE_PROXY_SERVER_HOSTNAME = "proxyserver"
 
@@ -45,10 +42,7 @@
 #
 SSH_TUNNEL_IMAGE = "harbor2.vantage6.ai/infrastructure/ssh-tunnel"
 
 #
 #   SQUID RELATED CONSTANTS
 #
 SQUID_IMAGE = "harbor2.vantage6.ai/infrastructure/squid"
-
-# start trying to refresh the JWT token 10 minutes before it expires.
-REFRESH_BEFORE_EXPIRES_SECONDS = 600
```

### Comparing `vantage6-node-3.9.0rc4/vantage6/node/proxy_server.py` & `vantage6-node-4.0.0a2/vantage6/node/proxy_server.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from http import HTTPStatus
 from requests import Response
 
 from flask import Flask, request, jsonify
 
 from vantage6.common import bytes_to_base64s, base64s_to_bytes, logger_name
-from vantage6.node.server_io import NodeClient
+from vantage6.common.client.node_client import NodeClient
 
 # Initialize FLASK
 app = Flask(__name__)
 log = logging.getLogger(logger_name(__name__))
 
 # Need to be set when the proxy server is initialized
 app.config["SERVER_IO"] = None
@@ -132,43 +132,43 @@
             log.exception(f'On attempt {i}, the proxy request raised an '
                           f'exception: <{url}>')
 
     # if all attemps fail, raise an exception to be handled by its parent
     raise Exception("Proxy request failed")
 
 
-def decrypt_result(result: dict) -> dict:
+def decrypt_result(run: dict) -> dict:
     """
-    Decrypt the `result` from a result dictonary
+    Decrypt the `result` from a run dictonary
 
     Parameters
     ----------
-    result: dict
-        Result dict
+    run: dict
+        Run dict
 
     Returns
     -------
     dict
-        Result dict with the `result` decrypted
+        Run dict with the `result` decrypted
     """
-    server_io: NodeClient = app.config.get('SERVER_IO')
+    client: NodeClient = app.config.get('SERVER_IO')
 
     # if the result is a None, there is no need to decrypt that..
     try:
-        if result['result']:
-            result["result"] = bytes_to_base64s(
-                server_io.cryptor.decrypt_str_to_bytes(
-                    result["result"]
+        if run['result']:
+            run["result"] = bytes_to_base64s(
+                client.cryptor.decrypt_str_to_bytes(
+                    run["result"]
                 )
             )
     except Exception:
         log.exception("Unable to decrypt and/or decode results, sending them "
                       "to the algorithm...")
 
-    return result
+    return run
 
 
 def get_response_json_and_handle_exceptions(
         response: Response) -> dict | None:
     """
     Obtain json content from request response
 
@@ -196,16 +196,16 @@
 
     Returns
     -------
     requests.Response
         Response from the vantage6 server
     """
     # We need the server io for the decryption of the results
-    server_io: NodeClient = app.config.get("SERVER_IO")
-    if not server_io:
+    client: NodeClient = app.config.get("SERVER_IO")
+    if not client:
         log.error("Task proxy request received but proxy server was not "
                   "initialized properly.")
         return jsonify({'msg': 'Proxy server not initialized properly'}), 500
 
     # All requests from algorithms are unencrypted. We encrypt the input
     # field for a specific organization(s) specified by the algorithm
     data = request.get_json()
@@ -248,25 +248,25 @@
         # retrieve public key of the organization
         log.debug(f"Retrieving public key of org: {organization_id}")
         response = make_request('get', f'organization/{organization_id}',
                                 headers=headers)
         public_key = response.json().get("public_key")
 
         # Encrypt the input field
-        server_io: NodeClient = app.config.get("SERVER_IO")
-        organization["input"] = server_io.cryptor.encrypt_bytes_to_str(
+        client: NodeClient = app.config.get("SERVER_IO")
+        organization["input"] = client.cryptor.encrypt_bytes_to_str(
             base64s_to_bytes(input_),
             public_key
         )
 
         log.debug("Input succesfully encrypted for organization "
                   f"{organization_id}!")
         return organization
 
-    if server_io.is_encrypted_collaboration():
+    if client.is_encrypted_collaboration():
 
         log.debug("Applying end-to-end encryption")
         data["organizations"] = [encrypt_input(o) for o in organizations]
 
     # Attempt to send the task to the central server
     try:
         response = make_request('post', 'task', data, headers=headers)
@@ -274,89 +274,89 @@
         log.exception('post task failed')
         return {'msg': 'Request failed, see node logs'},\
             HTTPStatus.INTERNAL_SERVER_ERROR
 
     return response.json(), HTTPStatus.OK
 
 
-@app.route('/task/<int:id>/result', methods=["GET"])
-def proxy_task_result(id: int) -> Response:
+@app.route('/result?task_id=<int:id_>', methods=["GET"])
+def proxy_result(id_: int) -> Response:
     """
     Obtain and decrypt all results to belong to a certain task
 
     Parameters
     ----------
     id : int
         Task id from which the results need to be obtained
 
     Returns
     -------
     requests.Response
         Reponse from the vantage6 server
     """
     # We need the server io for the decryption of the results
-    server_io = app.config.get("SERVER_IO")
-    if not server_io:
+    client = app.config.get("SERVER_IO")
+    if not client:
         return jsonify({'msg': 'Proxy server not initialized properly'}),\
             HTTPStatus.INTERNAL_SERVER_ERROR
 
     # Forward the request
     try:
-        response: Response = make_proxied_request(f"task/{id}/result")
+        response: Response = make_proxied_request(f"result?task_id={id_}")
     except Exception:
-        log.exception('Error on /result/<int:id>')
+        log.exception(f'Error on "result?task_id={id_}"')
         return {'msg': 'Request failed, see node logs'},\
             HTTPStatus.INTERNAL_SERVER_ERROR
 
     # Attempt to decrypt the results. The enpoint should have returned
     # a list of results
     unencrypted = []
-    results = get_response_json_and_handle_exceptions(response)
-    for result in results:
-        result = decrypt_result(result)
-        unencrypted.append(result)
+    runs = get_response_json_and_handle_exceptions(response)
+    for run in runs:
+        run = decrypt_result(run)
+        unencrypted.append(run)
 
     return jsonify(unencrypted), HTTPStatus.OK
 
 
-@app.route('/result/<int:id>', methods=["GET"])
-def proxy_results(id: int) -> Response:
+@app.route('/run/<int:id>', methods=["GET"])
+def proxy_runs(id_: int) -> Response:
     """
-    Obtain and decrypt the result from the vantage6 server to be used by
+    Obtain and decrypt the algorithm run from the vantage6 server to be used by
     an algorithm container.
 
     Parameters
     ----------
-    id : int
-        Id of the result to be obtained
+    id_ : int
+        Id of the run to be obtained
 
     Returns
     -------
     requests.Response
         Response of the vantage6 server
     """
     # We need the server io for the decryption of the results
-    server_io: NodeClient = app.config.get("SERVER_IO")
-    if not server_io:
+    client: NodeClient = app.config.get("SERVER_IO")
+    if not client:
         return {'msg': 'Proxy server not initialized properly'},\
             HTTPStatus.INTERNAL_SERVER_ERROR
 
     # Make the proxied request
     try:
-        response: Response = make_proxied_request(f"result/{id}")
+        response: Response = make_proxied_request(f"run/{id_}")
     except Exception:
-        log.exception('Error on /result/<int:id>')
+        log.exception('Error on /run/<int:id>')
         return {'msg': 'Request failed, see node logs...'},\
             HTTPStatus.INTERNAL_SERVER_ERROR
 
     # Try to decrypt the results
-    result = get_response_json_and_handle_exceptions(response)
-    result = decrypt_result(result)
+    run = get_response_json_and_handle_exceptions(response)
+    run = decrypt_result(run)
 
-    return result, HTTPStatus.OK
+    return run, HTTPStatus.OK
 
 
 @app.route('/<path:central_server_path>', methods=["GET", "POST", "PATCH",
                                                    "PUT", "DELETE"])
 def proxy(central_server_path: str) -> Response:
     """
     Generalized http proxy request
```

### Comparing `vantage6-node-3.9.0rc4/vantage6/node/socket.py` & `vantage6-node-4.0.0a2/vantage6/node/socket.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,40 +64,40 @@
         Actions to be taken when an algorithm container in the collaboration
         has changed its status.
 
         Parameters
         ----------
         data: Dict
             Dictionary with relevant data to the status change. Should include:
-            run_id: int
-                run_id of the algorithm container that changed status
+            job_id: int
+                job_id of the algorithm container that changed status
             status: str
                 New status of the algorithm container
         """
         status = data.get('status')
-        run_id = data.get('run_id')
+        job_id = data.get('job_id')
         if has_task_failed(status):
             # TODO handle run sequence at this node. Maybe terminate all
-            #     containers with the same run_id?
+            #     containers with the same job_id?
             self.log.critical(
                 f"A container on a node within your collaboration part of "
-                f"run_id={run_id} has exited with status '{status}'"
+                f"job_id={job_id} has exited with status '{status}'"
             )
         # else: no need to do anything when a task has started/finished/... on
         # another node
 
     def on_expired_token(self):
         """
         Action to be taken when node is notified by server that its token
         has expired.
         """
         self.log.warning("Your token is no longer valid... reconnecting")
         self.node_worker_ref.socketIO.disconnect()
         self.log.debug("Old socket connection terminated")
-        self.node_worker_ref.server_io.refresh_token()
+        self.node_worker_ref.client.refresh_token()
         self.log.debug("Token refreshed")
         self.node_worker_ref.connect_to_socket()
         self.log.debug("Connected to socket")
         self.node_worker_ref.sync_task_queue_with_server()
         self.log.debug("Tasks synced again with the server...")
 
     def on_kill_containers(self, kill_info: dict):
@@ -112,19 +112,19 @@
         """
         self.log.info(f"Received instruction to kill task: {kill_info}")
         killed_ids = self.node_worker_ref.kill_containers(kill_info)
         for killed in killed_ids:
             self.emit(
                 "algorithm_status_change",
                 {
-                    'result_id': killed.result_id,
+                    'run_id': killed.run_id,
                     'task_id': killed.task_id,
                     'collaboration_id':
-                        self.node_worker_ref.server_io.collaboration_id,
-                    'node_id': self.node_worker_ref.server_io.whoami.id_,
+                        self.node_worker_ref.client.collaboration_id,
+                    'node_id': self.node_worker_ref.client.whoami.id_,
                     'status': TaskStatus.KILLED,
                     'organization_id':
-                        self.node_worker_ref.server_io.whoami.organization_id,
+                        self.node_worker_ref.client.whoami.organization_id,
                     'parent_id': killed.parent_id,
                 },
                 namespace='/tasks'
             )
```

### Comparing `vantage6-node-3.9.0rc4/vantage6/node/util/colorer.py` & `vantage6-node-4.0.0a2/vantage6/node/util/colorer.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.9.0rc4/vantage6_node.egg-info/PKG-INFO` & `vantage6-node-4.0.0a2/vantage6_node.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-node
-Version: 3.9.0rc4
+Version: 4.0.0a2
 Summary: vantage6 node
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-node Version: 3.9.0rc4 Summary: vantage6
+Metadata-Version: 2.1 Name: vantage6-node Version: 4.0.0a2 Summary: vantage6
 node Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-node-3.9.0rc4/vantage6_node.egg-info/SOURCES.txt` & `vantage6-node-4.0.0a2/vantage6_node.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 tests/test_ssh_tunnel.py
 vantage6/node/__build__
 vantage6/node/__init__.py
 vantage6/node/_version.py
 vantage6/node/context.py
 vantage6/node/globals.py
 vantage6/node/proxy_server.py
-vantage6/node/server_io.py
 vantage6/node/socket.py
 vantage6/node/cli/__init__.py
 vantage6/node/cli/node.py
 vantage6/node/docker/docker_base.py
 vantage6/node/docker/docker_manager.py
 vantage6/node/docker/exceptions.py
 vantage6/node/docker/squid.py
```

