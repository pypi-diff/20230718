# Comparing `tmp/cotea-1.3.11.tar.gz` & `tmp/cotea-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cotea-1.3.11.tar", last modified: Tue Jul 18 16:30:46 2023, max compression
+gzip compressed data, was "cotea-1.3.9.tar", last modified: Tue Nov 29 11:02:09 2022, max compression
```

## Comparing `cotea-1.3.11.tar` & `cotea-1.3.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-18 16:30:46.506526 cotea-1.3.11/
--rw-rw-r--   0 david     (1000) david     (1000)    11357 2022-06-27 18:13:28.000000 cotea-1.3.11/LICENSE.md
--rw-rw-r--   0 david     (1000) david     (1000)     2881 2023-07-18 16:30:46.506526 cotea-1.3.11/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     2347 2022-06-27 18:13:28.000000 cotea-1.3.11/README.md
--rw-rw-r--   0 david     (1000) david     (1000)       85 2022-06-27 18:13:28.000000 cotea-1.3.11/pyproject.toml
--rw-rw-r--   0 david     (1000) david     (1000)      656 2023-07-18 16:30:46.506526 cotea-1.3.11/setup.cfg
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-18 16:30:46.502526 cotea-1.3.11/src/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-18 16:30:46.506526 cotea-1.3.11/src/cotea/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-16 14:08:25.000000 cotea-1.3.11/src/cotea/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     1551 2023-06-16 14:08:25.000000 cotea-1.3.11/src/cotea/ansible_execution_sync.py
--rw-rw-r--   0 david     (1000) david     (1000)     1754 2023-06-16 14:08:25.000000 cotea-1.3.11/src/cotea/ansible_execution_tree.py
--rw-rw-r--   0 david     (1000) david     (1000)     1425 2023-06-16 14:08:25.000000 cotea-1.3.11/src/cotea/arguments_maker.py
--rw-rw-r--   0 david     (1000) david     (1000)     4894 2023-06-16 14:08:25.000000 cotea-1.3.11/src/cotea/debug_utils.py
--rw-rw-r--   0 david     (1000) david     (1000)     1505 2023-06-16 14:08:25.000000 cotea-1.3.11/src/cotea/progress_bar.py
--rw-rw-r--   0 david     (1000) david     (1000)    15174 2023-06-16 15:02:32.000000 cotea-1.3.11/src/cotea/runner.py
--rw-rw-r--   0 david     (1000) david     (1000)      991 2023-06-16 14:08:25.000000 cotea-1.3.11/src/cotea/task_result.py
--rw-rw-r--   0 david     (1000) david     (1000)      327 2023-06-16 14:08:25.000000 cotea-1.3.11/src/cotea/utils.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-18 16:30:46.506526 cotea-1.3.11/src/cotea/wrappers/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-16 14:08:25.000000 cotea-1.3.11/src/cotea/wrappers/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)      208 2023-06-16 14:08:25.000000 cotea-1.3.11/src/cotea/wrappers/ansi_breakpoint.py
--rw-rw-r--   0 david     (1000) david     (1000)     6062 2023-06-16 14:08:25.000000 cotea-1.3.11/src/cotea/wrappers/get_next_task_wrapper.py
--rw-rw-r--   0 david     (1000) david     (1000)     2921 2023-06-16 14:08:25.000000 cotea-1.3.11/src/cotea/wrappers/iterator_add_task_wrapper.py
--rw-rw-r--   0 david     (1000) david     (1000)      818 2023-06-16 14:08:25.000000 cotea-1.3.11/src/cotea/wrappers/pbcli_run_wrapper.py
--rw-rw-r--   0 david     (1000) david     (1000)      643 2023-06-16 14:08:25.000000 cotea-1.3.11/src/cotea/wrappers/play_prereqs_wrapper.py
--rw-rw-r--   0 david     (1000) david     (1000)     3654 2023-06-16 14:08:25.000000 cotea-1.3.11/src/cotea/wrappers/playbook_executor_wrapper.py
--rw-rw-r--   0 david     (1000) david     (1000)     1584 2023-06-16 14:08:25.000000 cotea-1.3.11/src/cotea/wrappers/strategy_run_wrapper.py
--rw-rw-r--   0 david     (1000) david     (1000)     1611 2023-06-16 14:08:25.000000 cotea-1.3.11/src/cotea/wrappers/update_active_conn_wrapper.py
--rw-rw-r--   0 david     (1000) david     (1000)      368 2023-06-16 14:08:25.000000 cotea-1.3.11/src/cotea/wrappers/wrapper_base.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-18 16:30:46.506526 cotea-1.3.11/src/cotea.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)     2881 2023-07-18 16:30:46.000000 cotea-1.3.11/src/cotea.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)      834 2023-07-18 16:30:46.000000 cotea-1.3.11/src/cotea.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-07-18 16:30:46.000000 cotea-1.3.11/src/cotea.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)        6 2023-07-18 16:30:46.000000 cotea-1.3.11/src/cotea.egg-info/top_level.txt
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-11-29 11:02:09.022590 cotea-1.3.9/
+-rw-rw-r--   0 david     (1000) david     (1000)    11357 2022-06-27 18:13:28.000000 cotea-1.3.9/LICENSE.md
+-rw-rw-r--   0 david     (1000) david     (1000)     2880 2022-11-29 11:02:09.022590 cotea-1.3.9/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     2347 2022-06-27 18:13:28.000000 cotea-1.3.9/README.md
+-rw-rw-r--   0 david     (1000) david     (1000)       85 2022-06-27 18:13:28.000000 cotea-1.3.9/pyproject.toml
+-rw-rw-r--   0 david     (1000) david     (1000)      655 2022-11-29 11:02:09.022590 cotea-1.3.9/setup.cfg
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-11-29 11:02:09.022590 cotea-1.3.9/src/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-11-29 11:02:09.022590 cotea-1.3.9/src/cotea/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2022-07-04 14:20:54.000000 cotea-1.3.9/src/cotea/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1551 2022-07-04 14:20:54.000000 cotea-1.3.9/src/cotea/ansible_execution_sync.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1754 2022-08-11 17:04:27.000000 cotea-1.3.9/src/cotea/ansible_execution_tree.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1425 2022-07-04 14:20:54.000000 cotea-1.3.9/src/cotea/arguments_maker.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4568 2022-09-19 14:32:15.000000 cotea-1.3.9/src/cotea/debug_utils.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1505 2022-08-11 17:05:12.000000 cotea-1.3.9/src/cotea/progress_bar.py
+-rw-rw-r--   0 david     (1000) david     (1000)    15940 2022-11-28 13:59:45.000000 cotea-1.3.9/src/cotea/runner.py
+-rw-rw-r--   0 david     (1000) david     (1000)      991 2022-07-04 14:20:54.000000 cotea-1.3.9/src/cotea/task_result.py
+-rw-rw-r--   0 david     (1000) david     (1000)      327 2022-08-11 17:05:50.000000 cotea-1.3.9/src/cotea/utils.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-11-29 11:02:09.022590 cotea-1.3.9/src/cotea/wrappers/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2022-07-04 14:20:54.000000 cotea-1.3.9/src/cotea/wrappers/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)      208 2022-07-04 14:20:54.000000 cotea-1.3.9/src/cotea/wrappers/ansi_breakpoint.py
+-rw-rw-r--   0 david     (1000) david     (1000)     6488 2022-11-28 13:59:01.000000 cotea-1.3.9/src/cotea/wrappers/get_next_task_wrapper.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2921 2022-07-04 14:20:54.000000 cotea-1.3.9/src/cotea/wrappers/iterator_add_task_wrapper.py
+-rw-rw-r--   0 david     (1000) david     (1000)      818 2022-07-04 14:20:54.000000 cotea-1.3.9/src/cotea/wrappers/pbcli_run_wrapper.py
+-rw-rw-r--   0 david     (1000) david     (1000)      643 2022-07-04 14:20:54.000000 cotea-1.3.9/src/cotea/wrappers/play_prereqs_wrapper.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3654 2022-08-11 17:03:18.000000 cotea-1.3.9/src/cotea/wrappers/playbook_executor_wrapper.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1584 2022-07-04 14:20:54.000000 cotea-1.3.9/src/cotea/wrappers/strategy_run_wrapper.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1611 2022-07-06 13:30:14.000000 cotea-1.3.9/src/cotea/wrappers/update_active_conn_wrapper.py
+-rw-rw-r--   0 david     (1000) david     (1000)      368 2022-07-04 14:20:54.000000 cotea-1.3.9/src/cotea/wrappers/wrapper_base.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-11-29 11:02:09.022590 cotea-1.3.9/src/cotea.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)     2880 2022-11-29 11:02:09.000000 cotea-1.3.9/src/cotea.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)      834 2022-11-29 11:02:09.000000 cotea-1.3.9/src/cotea.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2022-11-29 11:02:09.000000 cotea-1.3.9/src/cotea.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        6 2022-11-29 11:02:09.000000 cotea-1.3.9/src/cotea.egg-info/top_level.txt
```

### Comparing `cotea-1.3.11/LICENSE.md` & `cotea-1.3.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cotea-1.3.11/PKG-INFO` & `cotea-1.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cotea
-Version: 1.3.11
+Version: 1.3.9
 Summary: Tool that provides Python API to run Ansible programmatically.
 Home-page: https://github.com/ispras/cotea
 Author: David Badalyan
 Author-email: dbadalyan@ispras.ru
 Project-URL: Bug Tracker, https://github.com/ispras/cotea/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `cotea-1.3.11/README.md` & `cotea-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `cotea-1.3.11/setup.cfg` & `cotea-1.3.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cotea
-version = 1.3.11
+version = 1.3.9
 author = David Badalyan
 author_email = dbadalyan@ispras.ru
 description = Tool that provides Python API to run Ansible programmatically.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ispras/cotea
 project_urls =
```

### Comparing `cotea-1.3.11/src/cotea/ansible_execution_sync.py` & `cotea-1.3.9/src/cotea/ansible_execution_sync.py`

 * *Files identical despite different names*

### Comparing `cotea-1.3.11/src/cotea/ansible_execution_tree.py` & `cotea-1.3.9/src/cotea/ansible_execution_tree.py`

 * *Files identical despite different names*

### Comparing `cotea-1.3.11/src/cotea/arguments_maker.py` & `cotea-1.3.9/src/cotea/arguments_maker.py`

 * *Files identical despite different names*

### Comparing `cotea-1.3.11/src/cotea/debug_utils.py` & `cotea-1.3.9/src/cotea/debug_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     help_msg += "'p' - print Progress bar\n"
     help_msg += "'h'/'help' - print this msg\n"
     help_msg += "\nAction commands:\n"
     help_msg += "'re' - RErun of the failed task\n"
     help_msg += "'v' - add new Variable as extra var\n"
     help_msg += "'c' - Continue ansible execution (go to the next task)\n"
     help_msg += "'nt' - add New Task\n"
-    help_msg += "'w' - Watch ansible variable value\n"
     #help_msg += "'f' - Finish ansible execution\n"
 
     print(help_msg)
 
 
 def pretty_print_task(task: Task):
     pretty_print = "Name: {}\nAction: {}\nArgs: {}\nbecome: {}\n".format(task.name,
@@ -102,22 +101,13 @@
 
             if not add_ok:
                 print("\nThe adding process was failed with the error:\n", err_msg)
             else:
                 print("\nNew task was added! It will run on every host of current inventory.")
                 print("Press 'c' after this, not 're'. This will run new task and the failed one after it.\n")
                 r.progress_bar.add_to_total_task_count(1)
-        
-        elif command == "w":
-            print("Enter var name: ", end="")
-            
-            var_name = input()
-            value = r.get_variable(var_name)
-            msg = "{} var value:\n{}".format(var_name, value)
-            
-            print(msg)
 
         elif command == "help" or command == "h":
             print_help_msg()
 
         else:
             print("Enter commands correctly! 'help' or just 'h' will help you\n")
```

### Comparing `cotea-1.3.11/src/cotea/progress_bar.py` & `cotea-1.3.9/src/cotea/progress_bar.py`

 * *Files identical despite different names*

### Comparing `cotea-1.3.11/src/cotea/runner.py` & `cotea-1.3.9/src/cotea/runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 from cotea.wrappers.iterator_add_task_wrapper import iterator_add_task_wrapper
 from cotea.progress_bar import ansible_progress_bar
 from cotea.ansible_execution_tree import AnsibleExecTree
 
 import logging
 
 
+
 class runner:
     def __init__(self, pb_path, arg_maker, debug_mod=None, show_progress_bar=False):
         logging_lvl = logging.INFO
         if debug_mod:
             logging_lvl= logging.DEBUG
         
         self.show_progress_bar = show_progress_bar
@@ -176,17 +177,15 @@
         self.logger.debug("run_next_task: %s", current_bp_label)
 
         if current_bp_label != self.breakpoint_labeles["after_task"]:
             self.logger.debug("run_next_task() has come not in to the 'after_task'")
         
         for task_result_ansible_obj in self.update_conn_wrapper.current_results:
             res.append(TaskResult(task_result_ansible_obj))
-
-        self.task_wrp.set_next_to_prev()
-
+        
         return res
     
 
     def rerun_last_task(self):
         self.task_wrp.rerun_last_task = True
     
 
@@ -400,8 +399,32 @@
     
 
     def add_var_as_extra_var(self, new_var_name, value):
         variable_manager = self.play_wrp.variable_manager
 
         ansible_way_var = AnsibleUnicode(new_var_name)
         variable_manager._extra_vars[ansible_way_var] = value
+   
+    
+    def _getIP(self):
+        var_name = "openstack_servers"
+        host_name = "localhost"
+        ip1_field_name = "interface_ip"
+        ip2_field_name = "private_v4"
+
+        res = ""
+        ostack_var = self.get_variable(var_name)
+
+        try:
+            if ip1_field_name in ostack_var[host_name][0]:
+                res = str(ostack_var[host_name][0][ip1_field_name])
+            elif ip2_field_name in ostack_var[host_name][0]:
+                res = str(ostack_var[host_name][0][ip2_field_name])
+        except Exception as e:
+            self.logger.info("During runner._getIP() call error was occured. We skipped it.")
+            self.logger.info("Error is:\n%s", e)
+
+        self.logger.debug("get_ip res = %s", res)
+        self.logger.debug(type(res))
+
+        return res
```

### Comparing `cotea-1.3.11/src/cotea/task_result.py` & `cotea-1.3.9/src/cotea/task_result.py`

 * *Files identical despite different names*

### Comparing `cotea-1.3.11/src/cotea/wrappers/get_next_task_wrapper.py` & `cotea-1.3.9/src/cotea/wrappers/get_next_task_wrapper.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,50 +11,46 @@
 # wraps ansible.plugins.strategy.linear.StrategyModule._get_next_task_lockstep()
 class get_next_task_wrapper(wrapper_base):
     def __init__(self, func, sync_obj, logger, bp_label, progress_bar: ansible_progress_bar, show_progr_bar=False):
         super().__init__(func, sync_obj, logger)
         self.before_task_bp = ansi_breakpoint(sync_obj, bp_label)
         self.prev_tasks = []
         self.next_tasks = []
-        self.task_before_new = None
         self.show_progress_bar = show_progr_bar
-        self.hosts_left = None
 
         self.rerun_last_task = False
         self.next_task_ignore_errors = False
 
         self.new_task_to_add = False
         self.new_task = None
 
         self.already_ignore_failed = []
         self.already_ignore_unrch = []
 
         self.progress_bar = progress_bar
 
 
     def __call__(self, real_obj, hosts_left, iterator):
-        self.hosts_left = real_obj.get_hosts_left(iterator)
         result = None
 
+        new_prev_tasks = self._copy_hosttasks(self.prev_tasks)
+        self.prev_tasks = new_prev_tasks
+
         if self.new_task_to_add:
-            self.task_before_new = self._copy_hosttasks(self.prev_tasks)
-            prev_tasks_with_new_task_set = self._set_task_in_hosttasks(self.new_task, self.task_before_new)
-            self.next_tasks = prev_tasks_with_new_task_set
-            result = prev_tasks_with_new_task_set
+            next_tasks_copy = self._copy_hosttasks(self.next_tasks)
+            next_tasks_with_new_task = self._set_task_in_hosttasks(self.new_task, next_tasks_copy)
+            result = next_tasks_with_new_task
 
         elif self.rerun_last_task:
-            if self.task_before_new:
-                self.next_tasks = self._copy_hosttasks(self.task_before_new)
-                self.task_before_new = None
-            else:
-                self.next_tasks = self._copy_hosttasks(self.prev_tasks)
-            
             result = self.next_tasks
 
         else:
+            new_prev_tasks = self._copy_hosttasks(self.next_tasks)
+            self.prev_tasks = new_prev_tasks
+
             result = self.func(real_obj, hosts_left, iterator)
             self.next_tasks = result
 
             self.already_ignore_failed = []
             self.already_ignore_unrch = []
                         
         for hosttask in result:
@@ -97,17 +93,38 @@
             self.rerun_last_task = False
 
         self.next_task_ignore_errors = False
         self.new_task_to_add = False
         self.new_task = None
 
         self.before_task_bp.stop()
+        
+        '''
+        self.logger.info("task run")
+        #print(dir(result[0][1]))
+        #print(dir(result[0][1]._name))
+        if result[0][1] != None:
+            if result[0][1].name == "Execute bad command":
+                self.zapas_task = result[0][1].copy()
+        else:
+            if self.zapas_task != None:
+                print("aaaaa")
+                return [(result[0][0], self.zapas_task)]
+        #self.sync_obj.continue_runner_with_stop()
+
+        print("zapas:", type(self.zapas_task))
+        '''
 
         return result
 
+        # все следующие - meta -> прокручиваем их без стопа и без
+        #                         возврата управления
+        # следующий - норм таск -> возвращаем управление, говоря true
+        # следующих не осталось -> возвращаем управление, говоря false
+
 
     def _copy_hosttasks(self, hosttasks):
         hosttasks_copy = []
 
         for hosttask in hosttasks:
             temp_host = None
             temp_task = None
@@ -119,20 +136,15 @@
             if hosttask[TASK_IND]:
                 temp_task = hosttask[TASK_IND].copy()
 
             if temp_host:
                 hosttasks_copy.append( (temp_host, temp_task) )
         
         return hosttasks_copy
-
-
-    def set_next_to_prev(self):
-        self.prev_tasks = self._copy_hosttasks(self.next_tasks)
-        self.next_tasks = []
-
+    
 
     def _set_task_in_hosttasks(self, new_task, hosttasks):
         hosttasks_with_new_task = []
 
         for hosttask in hosttasks:
             temp_host = None
 
@@ -179,13 +191,8 @@
     def get_prev_task_name(self):
         res = None
         prev_task = self.get_prev_task()
 
         if prev_task:
             res = prev_task.get_name()
         
-        return res
-    
-    
-    def skip_next_task(self):
-        for host in self.hosts_left:
-            self.ansible_iterator.get_next_task_for_host(host)
+        return res
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cotea-1.3.11/src/cotea/wrappers/iterator_add_task_wrapper.py` & `cotea-1.3.9/src/cotea/wrappers/iterator_add_task_wrapper.py`

 * *Files identical despite different names*

### Comparing `cotea-1.3.11/src/cotea/wrappers/pbcli_run_wrapper.py` & `cotea-1.3.9/src/cotea/wrappers/pbcli_run_wrapper.py`

 * *Files identical despite different names*

### Comparing `cotea-1.3.11/src/cotea/wrappers/play_prereqs_wrapper.py` & `cotea-1.3.9/src/cotea/wrappers/play_prereqs_wrapper.py`

 * *Files identical despite different names*

### Comparing `cotea-1.3.11/src/cotea/wrappers/playbook_executor_wrapper.py` & `cotea-1.3.9/src/cotea/wrappers/playbook_executor_wrapper.py`

 * *Files identical despite different names*

### Comparing `cotea-1.3.11/src/cotea/wrappers/strategy_run_wrapper.py` & `cotea-1.3.9/src/cotea/wrappers/strategy_run_wrapper.py`

 * *Files identical despite different names*

### Comparing `cotea-1.3.11/src/cotea/wrappers/update_active_conn_wrapper.py` & `cotea-1.3.9/src/cotea/wrappers/update_active_conn_wrapper.py`

 * *Files identical despite different names*

### Comparing `cotea-1.3.11/src/cotea.egg-info/PKG-INFO` & `cotea-1.3.9/src/cotea.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cotea
-Version: 1.3.11
+Version: 1.3.9
 Summary: Tool that provides Python API to run Ansible programmatically.
 Home-page: https://github.com/ispras/cotea
 Author: David Badalyan
 Author-email: dbadalyan@ispras.ru
 Project-URL: Bug Tracker, https://github.com/ispras/cotea/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `cotea-1.3.11/src/cotea.egg-info/SOURCES.txt` & `cotea-1.3.9/src/cotea.egg-info/SOURCES.txt`

 * *Files identical despite different names*

