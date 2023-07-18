# Comparing `tmp/cook-build-0.2.2.tar.gz` & `tmp/cook-build-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cook-build-0.2.2.tar", last modified: Mon Jun 26 21:14:30 2023, max compression
+gzip compressed data, was "cook-build-0.3.0.tar", last modified: Tue Jul 18 19:26:08 2023, max compression
```

## Comparing `cook-build-0.2.2.tar` & `cook-build-0.3.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:14:30.070451 cook-build-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-26 21:14:00.000000 cook-build-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-06-26 21:14:30.070451 cook-build-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-06-26 21:14:00.000000 cook-build-0.2.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:14:30.066450 cook-build-0.2.2/cook/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-26 21:14:00.000000 cook-build-0.2.2/cook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-06-26 21:14:00.000000 cook-build-0.2.2/cook/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-06-26 21:14:00.000000 cook-build-0.2.2/cook/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-06-26 21:14:00.000000 cook-build-0.2.2/cook/contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-06-26 21:14:00.000000 cook-build-0.2.2/cook/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-06-26 21:14:00.000000 cook-build-0.2.2/cook/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-26 21:14:00.000000 cook-build-0.2.2/cook/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-06-26 21:14:00.000000 cook-build-0.2.2/cook/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:14:30.070451 cook-build-0.2.2/cook_build.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-06-26 21:14:29.000000 cook-build-0.2.2/cook_build.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-26 21:14:30.000000 cook-build-0.2.2/cook_build.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 21:14:29.000000 cook-build-0.2.2/cook_build.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-26 21:14:29.000000 cook-build-0.2.2/cook_build.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-26 21:14:29.000000 cook-build-0.2.2/cook_build.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-26 21:14:29.000000 cook-build-0.2.2/cook_build.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-26 21:14:30.070451 cook-build-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-26 21:14:00.000000 cook-build-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:14:30.070451 cook-build-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-26 21:14:00.000000 cook-build-0.2.2/tests/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-06-26 21:14:00.000000 cook-build-0.2.2/tests/test_contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-06-26 21:14:00.000000 cook-build-0.2.2/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-26 21:14:00.000000 cook-build-0.2.2/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-26 21:14:00.000000 cook-build-0.2.2/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-06-26 21:14:00.000000 cook-build-0.2.2/tests/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-26 21:14:00.000000 cook-build-0.2.2/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:26:08.641342 cook-build-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-18 19:25:34.000000 cook-build-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-07-18 19:26:08.641342 cook-build-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-18 19:25:34.000000 cook-build-0.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:26:08.637343 cook-build-0.3.0/cook/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-18 19:25:34.000000 cook-build-0.3.0/cook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-07-18 19:25:34.000000 cook-build-0.3.0/cook/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-07-18 19:25:34.000000 cook-build-0.3.0/cook/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-07-18 19:25:34.000000 cook-build-0.3.0/cook/contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10307 2023-07-18 19:25:34.000000 cook-build-0.3.0/cook/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-07-18 19:25:34.000000 cook-build-0.3.0/cook/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-18 19:25:34.000000 cook-build-0.3.0/cook/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-18 19:25:34.000000 cook-build-0.3.0/cook/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:26:08.637343 cook-build-0.3.0/cook_build.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-07-18 19:26:08.000000 cook-build-0.3.0/cook_build.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-18 19:26:08.000000 cook-build-0.3.0/cook_build.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:26:08.000000 cook-build-0.3.0/cook_build.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-18 19:26:08.000000 cook-build-0.3.0/cook_build.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-18 19:26:08.000000 cook-build-0.3.0/cook_build.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-18 19:26:08.000000 cook-build-0.3.0/cook_build.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-18 19:26:08.641342 cook-build-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-18 19:25:34.000000 cook-build-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:26:08.641342 cook-build-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-18 19:25:34.000000 cook-build-0.3.0/tests/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-07-18 19:25:34.000000 cook-build-0.3.0/tests/test_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8293 2023-07-18 19:25:34.000000 cook-build-0.3.0/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-18 19:25:34.000000 cook-build-0.3.0/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-18 19:25:34.000000 cook-build-0.3.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-07-18 19:25:34.000000 cook-build-0.3.0/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-18 19:25:34.000000 cook-build-0.3.0/tests/test_util.py
```

### Comparing `cook-build-0.2.2/LICENSE` & `cook-build-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cook-build-0.2.2/PKG-INFO` & `cook-build-0.3.0/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,96 +1,80 @@
-Metadata-Version: 2.1
-Name: cook-build
-Version: 0.2.2
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 🧑‍🍳 Cook
 ==========
 
 .. image:: https://github.com/tillahoffmann/cook-build/actions/workflows/main.yaml/badge.svg
     :target: https://github.com/tillahoffmann/cook-build/actions/workflows/main.yaml
 .. image:: https://img.shields.io/pypi/v/cook-build
     :target: https://pypi.org/project/cook-build
 
 Cook is a task-centric build system with simple declarative recipes specified in Python.
 
 Getting Started
 ---------------
 
-Tasks are declared in a :code:`recipe.py` file using the :code:`~cook.manager.create_task` function. Each task must have a unique name, may depend on files or other tasks, and can execute an action, typically a shell command. The simple example below creates a C source file, compiles it, and executes the binary.
-
-.. code-block::
+Tasks are declared in a :code:`recipe.py` file using the :func:`~cook.manager.create_task` function. Each task must have a unique name, may depend on files or other tasks, and can execute an action, typically a shell command. The simple example below creates a C source file, compiles it, and executes the binary.
 
+.. doctest::
 
     >>> from cook import create_task
 
     >>> create_task("src", targets=["hello.c"],
     ...             action="echo 'int main() { return 0; }' > hello.c")  # doctest: +IGNORE_RESULT
     >>> create_task("cc", dependencies=["hello.c"], targets=["hello"],
     ...             action="cc -o hello hello.c")  # doctest: +IGNORE_RESULT
     >>> create_task("hello", dependencies=["hello"], action="./hello")  # doctest: +IGNORE_RESULT
 
 Running :code:`cook ls` from the command line lists all known tasks, e.g.,
 
-.. code-block::
-
+.. shtest::
     :cwd: examples/getting_started
 
     $ cook ls
     <task `src` @ /.../recipe.py:3>
     <task `cc` @ /.../recipe.py:4>
     <task `hello` @ /.../recipe.py:5>
 
-Running :code:`cook exec hello` creates the source file, compile it, and executes the binary. We use :code:`--log-level=debug` to provide additional information here.
-
-.. code-block::
+Running :code:`cook exec hello` creates the source file, compile it, and executes the binary (using :code:`--log-level=debug` can provide additional information).
 
+.. shtest::
     :cwd: examples/getting_started
     :stderr:
 
-    $ cook --log-level=debug exec hello
-    DEBUG: <task `src` @ .../recipe.py:3> is stale because one of its targets is missing
-    DEBUG: started <task `src` @ .../recipe.py:3>
-    DEBUG: completed <task `src` @ .../recipe.py:3> in ... seconds
-    DEBUG: <task `src` @ .../recipe.py:3> created `hello.c`
-    DEBUG: <task `cc` @ .../recipe.py:4> is stale because one of its targets is missing
-    DEBUG: started <task `cc` @ .../recipe.py:4>
-    DEBUG: completed <task `cc` @ .../recipe.py:4> in ... seconds
-    DEBUG: <task `cc` @ .../recipe.py:4> created `hello`
-    DEBUG: <task `hello` @ .../recipe.py:5> is "stale" because it has no targets
-    DEBUG: started <task `hello` @ .../recipe.py:5>
-    DEBUG: completed <task `hello` @ .../recipe.py:5> in ... seconds
+    $ cook exec hello
+    INFO: executing <task `src` @ /.../recipe.py:3> ...
+    INFO: completed <task `src` @ /.../recipe.py:3>
+    INFO: executing <task `cc` @ /.../recipe.py:4> ...
+    INFO: completed <task `cc` @ /.../recipe.py:4>
+    INFO: executing <task `hello` @ /.../recipe.py:5> ...
+    INFO: completed <task `hello` @ /.../recipe.py:5>
 
 To rerun a task, tell Cook to reset it.
 
-.. code-block::
-
+.. shtest::
     :cwd: examples/getting_started
     :stderr:
 
     $ cook reset cc
     INFO: reset 1 task
 
 The full set of available commands can be explored using :code:`cook --help` as shown below.
 
-.. cook --help
+.. sh:: cook --help
 
 Tasks Are Dumb; Contexts Are Smart
 ----------------------------------
 
-:code:`~cook.task.Task`\ s do not provide any functionality beyond storing metadata, including
+:class:`~cook.task.Task`\ s do not provide any functionality beyond storing metadata, including
 
 - :code:`targets`, the files generated by the task,
 - :code:`dependencies`, the files the task depends on,
-- :code:`action`, the :code:`~cook.actions.Action` to execute when the task is run,
+- :code:`action`, the :class:`~cook.actions.Action` to execute when the task is run,
 - :code:`task_dependencies`, other tasks that should be executed first,
 - :code:`location`, filename and line number where the task was defined.
 
-All logic is handled by :code:`~cook.contexts.Context`\ s which are applied to each task when it is created. For example, :code:`~cook.contexts.create_group` adds all tasks created within the context to a group. This group can be executed to execute all child tasks.
+All logic is handled by :class:`~cook.contexts.Context`\ s which are applied to each task when it is created. For example, :class:`~cook.contexts.create_group` adds all tasks created within the context to a group. This group can be executed to execute all child tasks.
 
-..
+.. toctree::
     :hidden:
     :maxdepth: 1
 
     docs/interface
```

### Comparing `cook-build-0.2.2/README.rst` & `cook-build-0.3.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,85 +1,91 @@
+Metadata-Version: 2.1
+Name: cook-build
+Version: 0.3.0
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
 🧑‍🍳 Cook
 ==========
 
 .. image:: https://github.com/tillahoffmann/cook-build/actions/workflows/main.yaml/badge.svg
     :target: https://github.com/tillahoffmann/cook-build/actions/workflows/main.yaml
 .. image:: https://img.shields.io/pypi/v/cook-build
     :target: https://pypi.org/project/cook-build
 
 Cook is a task-centric build system with simple declarative recipes specified in Python.
 
 Getting Started
 ---------------
 
-Tasks are declared in a :code:`recipe.py` file using the :func:`~cook.manager.create_task` function. Each task must have a unique name, may depend on files or other tasks, and can execute an action, typically a shell command. The simple example below creates a C source file, compiles it, and executes the binary.
+Tasks are declared in a :code:`recipe.py` file using the :code:`~cook.manager.create_task` function. Each task must have a unique name, may depend on files or other tasks, and can execute an action, typically a shell command. The simple example below creates a C source file, compiles it, and executes the binary.
+
+.. code-block::
 
-.. doctest::
 
     >>> from cook import create_task
 
     >>> create_task("src", targets=["hello.c"],
     ...             action="echo 'int main() { return 0; }' > hello.c")  # doctest: +IGNORE_RESULT
     >>> create_task("cc", dependencies=["hello.c"], targets=["hello"],
     ...             action="cc -o hello hello.c")  # doctest: +IGNORE_RESULT
     >>> create_task("hello", dependencies=["hello"], action="./hello")  # doctest: +IGNORE_RESULT
 
 Running :code:`cook ls` from the command line lists all known tasks, e.g.,
 
-.. shtest::
+.. code-block::
+
     :cwd: examples/getting_started
 
     $ cook ls
     <task `src` @ /.../recipe.py:3>
     <task `cc` @ /.../recipe.py:4>
     <task `hello` @ /.../recipe.py:5>
 
-Running :code:`cook exec hello` creates the source file, compile it, and executes the binary. We use :code:`--log-level=debug` to provide additional information here.
+Running :code:`cook exec hello` creates the source file, compile it, and executes the binary (using :code:`--log-level=debug` can provide additional information).
+
+.. code-block::
 
-.. shtest::
     :cwd: examples/getting_started
     :stderr:
 
-    $ cook --log-level=debug exec hello
-    DEBUG: <task `src` @ .../recipe.py:3> is stale because one of its targets is missing
-    DEBUG: started <task `src` @ .../recipe.py:3>
-    DEBUG: completed <task `src` @ .../recipe.py:3> in ... seconds
-    DEBUG: <task `src` @ .../recipe.py:3> created `hello.c`
-    DEBUG: <task `cc` @ .../recipe.py:4> is stale because one of its targets is missing
-    DEBUG: started <task `cc` @ .../recipe.py:4>
-    DEBUG: completed <task `cc` @ .../recipe.py:4> in ... seconds
-    DEBUG: <task `cc` @ .../recipe.py:4> created `hello`
-    DEBUG: <task `hello` @ .../recipe.py:5> is "stale" because it has no targets
-    DEBUG: started <task `hello` @ .../recipe.py:5>
-    DEBUG: completed <task `hello` @ .../recipe.py:5> in ... seconds
+    $ cook exec hello
+    INFO: executing <task `src` @ /.../recipe.py:3> ...
+    INFO: completed <task `src` @ /.../recipe.py:3>
+    INFO: executing <task `cc` @ /.../recipe.py:4> ...
+    INFO: completed <task `cc` @ /.../recipe.py:4>
+    INFO: executing <task `hello` @ /.../recipe.py:5> ...
+    INFO: completed <task `hello` @ /.../recipe.py:5>
 
 To rerun a task, tell Cook to reset it.
 
-.. shtest::
+.. code-block::
+
     :cwd: examples/getting_started
     :stderr:
 
     $ cook reset cc
     INFO: reset 1 task
 
 The full set of available commands can be explored using :code:`cook --help` as shown below.
 
-.. sh:: cook --help
+.. cook --help
 
 Tasks Are Dumb; Contexts Are Smart
 ----------------------------------
 
-:class:`~cook.task.Task`\ s do not provide any functionality beyond storing metadata, including
+:code:`~cook.task.Task`\ s do not provide any functionality beyond storing metadata, including
 
 - :code:`targets`, the files generated by the task,
 - :code:`dependencies`, the files the task depends on,
-- :code:`action`, the :class:`~cook.actions.Action` to execute when the task is run,
+- :code:`action`, the :code:`~cook.actions.Action` to execute when the task is run,
 - :code:`task_dependencies`, other tasks that should be executed first,
 - :code:`location`, filename and line number where the task was defined.
 
-All logic is handled by :class:`~cook.contexts.Context`\ s which are applied to each task when it is created. For example, :class:`~cook.contexts.create_group` adds all tasks created within the context to a group. This group can be executed to execute all child tasks.
+All logic is handled by :code:`~cook.contexts.Context`\ s which are applied to each task when it is created. For example, :code:`~cook.contexts.create_group` adds all tasks created within the context to a group. This group can be executed to execute all child tasks.
 
-.. toctree::
+..
     :hidden:
     :maxdepth: 1
 
     docs/interface
```

### Comparing `cook-build-0.2.2/cook/__main__.py` & `cook-build-0.3.0/cook/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,22 +27,24 @@
         else:
             *patterns, last = patterns
             message = "found no tasks matching patterns " + ", ".join(patterns) \
                 + (", or " if len(patterns) > 1 else " or ") + last
         super().__init__(message)
 
 
-def discover_tasks(manager: Manager, patterns: Iterable[re.Pattern], use_re: bool) -> List[Task]:
+def discover_tasks(tasks: Iterable[Task], patterns: Iterable[re.Pattern], use_re: bool) \
+        -> List[Task]:
     """
     Discover tasks based on regular expressions.
     """
     if not patterns:
-        return list(manager.tasks.values())
-    tasks = [task for name, task in manager.tasks.items() if
-             any(re.match(pat, name) if use_re else fnmatch.fnmatch(name, pat) for pat in patterns)]
+        return list(tasks)
+    tasks = [task for task in tasks if any(
+        re.match(pat, task.name) if use_re else fnmatch.fnmatch(task.name, pat) for pat in patterns
+    )]
     if not tasks:
         raise NoMatchingTaskError(patterns)
     return tasks
 
 
 class Command:
     """
@@ -76,18 +78,16 @@
         parser.add_argument("--re", "-r", action="store_true",
                             help="use regular expressions for pattern matching instead of glob")
         parser.add_argument("--jobs", "-j", help="number of concurrent jobs", type=int, default=1)
         parser.add_argument("tasks", nargs="+",
                             help="task or tasks to execute as regular expressions")
 
     def execute(self, controller: Controller, args: ExecArgs) -> None:
-        # Monkeypatch the controller semaphore.
-        controller.num_concurrent = args.jobs
-        tasks = discover_tasks(controller.manager, args.tasks, args.re)
-        controller.execute_sync(*tasks)
+        tasks = discover_tasks(controller.dependencies, args.tasks, args.re)
+        controller.execute(tasks, num_concurrent=args.jobs)
 
 
 class LsArgs(argparse.Namespace):
     tasks: Iterable[re.Pattern]
     all: bool
     re: bool
 
@@ -103,15 +103,15 @@
                             help="include tasks starting with `_` prefix")
         parser.add_argument("--re", "-r", action="store_true",
                             help="use regular expressions for pattern matching instead of glob")
         parser.add_argument("tasks", nargs="*",
                             help="task or tasks to execute as regular expressions")
 
     def execute(self, controller: Controller, args: LsArgs) -> None:
-        tasks = discover_tasks(controller.manager, args.tasks, args.re)
+        tasks = discover_tasks(controller.dependencies, args.tasks, args.re)
         if not args.all:
             tasks = [task for task in tasks if not task.name.startswith("_")]
         print("\n".join(map(str, tasks)))
 
 
 class InfoArgs(argparse.Namespace):
     pass
@@ -145,15 +145,15 @@
     def configure_parser(self, parser: argparse.ArgumentParser) -> None:
         parser.add_argument("--re", "-r", action="store_true",
                             help="use regular expressions for pattern matching instead of glob")
         parser.add_argument("tasks", nargs="*",
                             help="task or tasks to execute as regular expressions")
 
     def execute(self, controller: Controller, args: ResetArgs) -> None:
-        controller.reset(*discover_tasks(controller.manager, args.tasks, args.re))
+        controller.reset(*discover_tasks(controller.dependencies, args.tasks, args.re))
 
 
 class Formatter(logging.Formatter):
     COLOR_BY_LEVEL = {
         "DEBUG": colorama.Fore.MAGENTA,
         "INFO": colorama.Fore.BLUE,
         "WARNING": colorama.Fore.YELLOW,
@@ -183,15 +183,14 @@
         subparser.set_defaults(command=command)
 
     args = parser.parse_args(cli_args)
 
     handler = logging.StreamHandler()
     handler.setFormatter(Formatter())
     logging.basicConfig(level=args.log_level.upper(), handlers=[handler])
-    logging.getLogger("asyncio").setLevel(logging.WARNING)
 
     with Manager() as manager:
         manager.contexts.extend([
             create_target_directories(),
             normalize_action(),
             normalize_dependencies(),
         ])
@@ -208,18 +207,20 @@
             recipe = importlib.util.module_from_spec(spec)
             spec.loader.exec_module(recipe)
         else:  # pragma: no cover
             raise ValueError("recipe file or module must be specified; default recipe.py not found")
 
     with sqlite3.connect(args.db) as connection:
         connection.execute(QUERIES["schema"])
-        controller = Controller(manager, connection)
+        controller = Controller(manager.resolve_dependencies(), connection)
         command: Command = args.command
         try:
             command.execute(controller, args)
+        except KeyboardInterrupt:  # pragma: no cover
+            LOGGER.warning("interrupted by user")
         except NoMatchingTaskError as ex:
             LOGGER.warning(ex)
             sys.exit(1)
         except FailedTaskError:
             sys.exit(1)
```

### Comparing `cook-build-0.2.2/cook/actions.py` & `cook-build-0.3.0/cook/actions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,88 +1,74 @@
 r"""
 Actions
 -------
 
 Actions are performed when tasks are executed. Builtin actions include calling python functions
-using :class:`.FunctionAction`, running subprocesses using :class:`.SubprocessAction`, executing
-commands using :class:`.ShellAction`, and composing multiple actions using
-:class:`.CompositeAction`.
+using :class:`.FunctionAction`, running subprocesses using :class:`.SubprocessAction`, and composing
+multiple actions using :class:`.CompositeAction`.
 
-Custom contexts can be implemented by inheriting from :class:`.Action` and implementing the
+Custom actions can be implemented by inheriting from :class:`.Action` and implementing the
 :meth:`~.Action.execute` method which receives a :class:`~.task.Task`. The method should execute the
 action; its return value is ignored. For example, the following action waits for a specified time.
 
 .. doctest::
 
-    >>> from asyncio import sleep
     >>> from cook.actions import Action
-    >>> from cook.task import Task
-    >>> from cook.util import run_until_complete
-    >>> from time import time
+    >>> from time import sleep, time
 
     >>> class SleepAction(Action):
     ...     def __init__(self, delay: float) -> None:
     ...         self.delay = delay
     ...
-    ...     async def execute(self, task: Task) -> None:
+    ...     def execute(self, task: Task) -> None:
     ...         start = time()
-    ...         await sleep(self.delay)
+    ...         sleep(self.delay)
     ...         print(f"time: {time() - start:.3f}")
 
     >>> action = SleepAction(0.1)
-    >>> action.execute_sync(None)
+    >>> action.execute(None)
     time: 0.1...
 """
-import asyncio
-from subprocess import SubprocessError
-from typing import Awaitable, Callable, TYPE_CHECKING
-from . import util
+import subprocess
+from typing import Callable, Optional, TYPE_CHECKING
 
 
 if TYPE_CHECKING:
     from .task import Task
+    from .util import StopEvent
 
 
 class Action:
     """
-    Action to perform when a task is executed.
+    Action to perform when a task is executed in its own thread.
     """
-    async def execute(self, task: "Task") -> None:
+    def execute(self, task: "Task", stop: Optional["StopEvent"] = None) -> None:
         """
         Execute the action.
         """
         raise NotImplementedError
 
-    def execute_sync(self, task: "Task") -> None:
-        """
-        Execute the action synchronously.
-        """
-        util.run_until_complete(self.execute(task))
-
 
 class FunctionAction(Action):
     """
-    Action wrapping a python callable. Both synchronous functions and :code:`async` functions are
-    supported.
+    Action wrapping a python callable.
 
     Args:
         func: Function to call which must accept a :class:`~.task.Task` as its first argument.
         *args: Additional positional arguments.
         **kwargs: Keyword arguments.
     """
     def __init__(self, func: Callable, *args, **kwargs) -> None:
         super().__init__()
         self.func = func
         self.args = args
         self.kwargs = kwargs
 
-    async def execute(self, task: "Task") -> None:
-        result = self.func(task, *self.args, **self.kwargs)
-        if isinstance(result, Awaitable):
-            await result
+    def execute(self, task: "Task", stop: Optional["StopEvent"] = None) -> None:
+        self.func(task, *self.args, **self.kwargs)
 
 
 class SubprocessAction(Action):
     """
     Run a subprocess.
 
     Args:
@@ -93,71 +79,59 @@
     Example:
 
         .. doctest::
 
             >>> from cook.actions import SubprocessAction
             >>> from pathlib import Path
 
-            >>> action = SubprocessAction("touch", "hello.txt")
-            >>> action.execute_sync(None)
+            >>> action = SubprocessAction(["touch", "hello.txt"])
+            >>> action.execute(None)
             >>> Path("hello.txt").is_file()
             True
     """
-    def __init__(self, program: str, *args, **kwargs) -> None:
-        self.program = program
+    def __init__(self, *args, **kwargs) -> None:
         self.args = args
         self.kwargs = kwargs
 
-    async def execute(self, task: "Task") -> None:
-        process = await asyncio.create_subprocess_exec(self.program, *self.args, **self.kwargs)
-        status = await process.wait()
-        if status:
-            raise SubprocessError(f"executing {[self.program, *self.args]} returned status code "
-                                  f"{status}")
-
-
-class ShellAction(Action):
-    r"""
-    Execute a shell command.
-
-    Args:
-        cmd: Command to execute.
-        *args: Additional positional arguments.
-        **kwargs: Keyword arguments.
-
-    Example:
-
-        .. doctest::
-
-            >>> from cook.actions import ShellAction
-            >>> from pathlib import Path
-
-            >>> action = ShellAction("echo hello > world.txt")
-            >>> action.execute_sync(None)
-            >>> Path("world.txt").read_text()
-            'hello\n'
-    """
-    def __init__(self, cmd: str, *args, **kwargs) -> None:
-        self.cmd = cmd
-        self.args = args
-        self.kwargs = kwargs
+    def execute(self, task: "Task", stop: Optional["StopEvent"] = None) -> None:
+        # Repeatedly wait for the process to complete, checking the stop event after each poll.
+        interval = stop.interval if stop else None
+        process = subprocess.Popen(*self.args, **self.kwargs)
+        while True:
+            try:
+                returncode = process.wait(interval)
+                if returncode:
+                    raise subprocess.CalledProcessError(returncode, process.args)
+                return
+            except subprocess.TimeoutExpired:
+                if stop.is_set():
+                    break
+
+        # Clean up the process by trying to terminate it and then killing it.
+        for method in [process.terminate, process.kill]:
+            method()
+            try:
+                returncode = process.wait(max(interval, 3))
+                if returncode:
+                    raise subprocess.CalledProcessError(returncode, process.args)
+                # The process managed to exit gracefully after the main loop. This is unlikely.
+                return  # pragma: no cover
+            except subprocess.TimeoutExpired:  # pragma: no cover
+                pass
 
-    async def execute(self, task: "Task") -> None:
-        process = await asyncio.create_subprocess_shell(self.cmd, *self.args, **self.kwargs)
-        status = await process.wait()
-        if status:
-            raise SubprocessError(f"executing `{self.cmd}` returned status code {status}")
+        # We couldn't kill the process. Also very unlikely.
+        raise subprocess.SubprocessError(f"failed to shut down {process}")  # pragma: no cover
 
 
 class CompositeAction(Action):
     """
     Execute multiple actions in order.
 
     Args:
         *actions: Actions to execute.
     """
     def __init__(self, *actions: Action) -> None:
         self.actions = actions
 
-    async def execute(self, task: "Task") -> None:
+    def execute(self, task: "Task", stop: Optional["StopEvent"] = None) -> None:
         for action in self.actions:
-            await action.execute(task)
+            action.execute(task, stop)
```

### Comparing `cook-build-0.2.2/cook/contexts.py` & `cook-build-0.3.0/cook/contexts.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,17 @@
 :meth:`~.Context.apply` method which receives a :class:`~.task.Task` and must return a
 :class:`~.task.Task`. For example, the following context converts all task names to uppercase.
 
 .. doctest::
 
     >>> from cook import create_task
     >>> from cook.contexts import Context
-    >>> from cook.task import Task
 
     >>> class UpperCaseContext(Context):
-    ...     def apply(self, task: Task) -> Task:
+    ...     def apply(self, task):
     ...         task.name = task.name.upper()
     ...         return task
 
     >>> # Using the contexts yields uppercase task names.
     >>> with UpperCaseContext():
     ...    create_task("foo")
     <task `FOO` @ ...>
@@ -79,15 +78,16 @@
 
 
 class FunctionContext(Context):
     """
     Context wrapping a function to modify or replace a task.
 
     Args:
-        func: Function to call which must accept a :class:`~.task.Task` as its first argument.
+        func: Function to call which must accept a :class:`~.task.Task` as its first argument and
+            return a :class:`~.task.Task`.
         *args: Additional positional arguments.
         **kwargs: Keyword arguments.
 
     .. note::
 
         :code:`manager` is a reserved keyword for the constructor of all contexts and cannot be used
         as a keyword argument for the wrapped function.
@@ -104,16 +104,16 @@
             ...     task.name = task.name * n
             ...     return task
 
             >>> with FunctionContext(repeat, 3):
             ...     create_task("baz")
             <task `bazbazbaz` @ ...>
     """
-    def __init__(self, func: Callable, *args, manager: Optional["Manager"] = None, **kwargs) \
-            -> None:
+    def __init__(self, func: Callable[["Task"], Task], *args, manager: Optional["Manager"] = None,
+                 **kwargs) -> None:
         super().__init__(manager)
         self.func = func
         self.args = args or ()
         self.kwargs = kwargs or {}
 
     def apply(self, task: "Task") -> "Task":
         return self.func(task, *self.args, **self.kwargs)
@@ -130,46 +130,48 @@
     def apply(self, task: "Task") -> Task:
         for target in task.targets:
             name = f"_create_target_directories:{target.parent}"
             # No need to create a task if the parent already exists.
             if target.parent.is_dir():
                 continue
             # Create a task if necessary.
-            if (create := self.manager.tasks.get(name)) is None:
+            create = self.manager.tasks.get(name)
+            if create is None:
                 create = self.manager.create_task(name, action=actions.FunctionAction(
                     lambda _: target.parent.mkdir(parents=True, exist_ok=True)
                 ))
             task.task_dependencies.append(create)
         return task
 
 
 class normalize_action(Context):
     """
     Normalize actions of tasks.
 
     - If the action is a callable, it will be wrapped in a :class:`~.actions.FunctionAction`.
-    - If the action is a string, it will be executed using a :class:`~.actions.ShellAction`.
+    - If the action is a string, it will be executed using a :class:`~.actions.SubprocessAction`
+        with :code:`shell = True`.
     - If the action is a list of actions, a :class:`~.actions.CompositeAction` will be created.
     - If the action is any other list, it will be executed using a
       :class:`.actions.SubprocessAction` after converting elements to strings.
 
     .. note::
 
         This context is active by default.
     """
     def apply(self, task: "Task") -> "Task":
         if isinstance(task.action, Callable):
             task.action = actions.FunctionAction(task.action)
         elif isinstance(task.action, str):
-            task.action = actions.ShellAction(task.action)
+            task.action = actions.SubprocessAction(task.action, shell=True)
         elif isinstance(task.action, List):
             if all(isinstance(x, actions.Action) for x in task.action):
                 task.action = actions.CompositeAction(*task.action)
             else:
-                task.action = actions.SubprocessAction(*list(map(str, task.action)))
+                task.action = actions.SubprocessAction(list(map(str, task.action)))
         return task
 
 
 class normalize_dependencies(Context):
     """
     Normalize dependencies of tasks.
```

### Comparing `cook-build-0.2.2/cook/controller.py` & `cook-build-0.3.0/cook/controller.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,198 +1,262 @@
-import asyncio
+import hashlib
 import logging
-import os
+import networkx as nx
 from pathlib import Path
+from queue import Empty, Queue
 from sqlite3 import Connection
 import sys
-from typing import Dict, Iterable, Optional, Set, Tuple, TYPE_CHECKING, Union
+import threading
+import time
+from typing import Dict, List, Optional, Sequence, Set, Tuple, TYPE_CHECKING, Union
 from . import util
 
 if TYPE_CHECKING:
-    from .manager import Manager
     from .task import Task
 
 
 LOGGER = logging.getLogger(__name__)
 QUERIES = {
     "schema": """
-    CREATE TABLE IF NOT EXISTS "files" (
+    CREATE TABLE IF NOT EXISTS "tasks" (
         "name" TEXT PRIMARY KEY,
-        "size" INTEGER NOT NULL,
         "digest" TEXT NOT NULL
     )
     """,
     "select": """
-        SELECT "size", "digest" FROM "files" WHERE "name" = :name
+        SELECT "digest" FROM "files" WHERE "name" = :name
     """,
     "upsert": """
-        INSERT INTO "files" ("name", "size", "digest") VALUES (:name, :size, :digest)
-        ON CONFLICT("name") DO UPDATE SET "size" = :size, "digest" = :digest
+        INSERT INTO "tasks" ("name", "digest") VALUES (:name, :digest)
+        ON CONFLICT("name") DO UPDATE SET "digest" = :digest
     """
 }
 
 
 class Controller:
     """
     Controller to manage dependencies and execute tasks.
     """
-    def __init__(self, manager: "Manager", connection: Connection, num_concurrent: int = 1) -> None:
-        self.manager = manager
+    def __init__(self, dependencies: nx.DiGraph, connection: Connection) -> None:
+        self.dependencies = dependencies
         self.connection = connection
-        self.dependencies = manager.resolve_dependencies()
-        self.status: Dict[Task, bool] = {}
-        self.futures: Dict[Task, asyncio.Future] = {}
-        self.size_digest: Dict[str, Tuple[int, str]] = {}
-        self.num_concurrent = num_concurrent
-        self._semaphore = None
-        self.cancelled = False
-
-    @property
-    def semaphore(self) -> asyncio.Semaphore:
-        # Create the semaphore upon first use for python 3.9 and below (see
-        # https://stackoverflow.com/a/55918049/1150961 for details).
-        if self._semaphore is None:
-            self._semaphore = asyncio.Semaphore(self.num_concurrent)
-        return self._semaphore
-
-    def resolve_stale_tasks(self, tasks: Optional[Iterable["Task"]] = None) -> Set["Task"]:
-        tasks = tasks or self.manager.tasks.values()
-        for task in tasks:
-            self.is_stale(task)
-        return {task for task, is_stale in self.status.items() if is_stale}
-
-    def path_to_name(self, path: Union[str, Path]) -> str:
-        """
-        Convert a path to a unique name by resolving it relative to the working directory.
-        """
-        return str(Path(path).resolve().relative_to(os.getcwd()))
-
-    def evaluate_size_digest(self, path: Union[str, Path]) -> Tuple[int, str]:
-        """
-        Evaluate the size and hex digest of a file.
-        """
-        path = Path(path)
-        name = self.path_to_name(path)
-        if result := self.size_digest.get(name):
-            return result
-        size = path.stat().st_size
-        digest = util.evaluate_hexdigest(path)
-        self.size_digest[name] = size, digest
-        return size, digest
+        self._digest_cache: Dict[Path, Tuple[float, bytes]] = {}
+
+    def resolve_stale_tasks(self, tasks: Optional[List["Task"]] = None) -> Set["Task"]:
+        self.is_stale(tasks or list(self.dependencies))
+        return {node for node, data in self.dependencies.nodes(True) if data.get("is_stale")}
+
+    def _evaluate_path_digest(self, path: Path) -> bytes:
+        """
+        Evaluate the digest of a file.
+        """
+        path = Path(path).resolve()
+        cached = self._digest_cache.get(path)
+        if cached:
+            digested, digest = cached
+            if path.stat().st_mtime < digested:
+                return digest
+        digest = util.evaluate_digest(path)
+        self._digest_cache[path] = (time.time(), digest)
+        return digest
+
+    def _evaluate_task_hexdigest(self, task: "Task") -> bytes:
+        """
+        Evaluate the digest of a task by combining the digest of all its dependencies.
+        """
+        dependencies = []
+        for dependency in task.dependencies:
+            dependency = Path(dependency).resolve()
+            if not dependency.is_file():
+                LOGGER.debug("dependency %s of %s is missing", dependency, task)
+                return None
+            dependencies.append(dependency)
+
+        hasher = hashlib.sha1()
+        for dependency in sorted(dependencies):
+            hasher.update(util.evaluate_digest(dependency))
+        return hasher.hexdigest()
+
+    def is_stale(self, task: Union["Task", Sequence["Task"]]) -> Union[bool, List[bool]]:
+        """
+        Determine if one or more tasks are stale.
+
+        Args:
+            task: Task or tasks to check.
+
+        Returns:
+            If the task or tasks are stale.
+        """
+        if isinstance(task, Sequence):
+            return [self.is_stale(x) for x in task]
+
+        is_stale = self.dependencies.nodes[task].get("is_stale")
+        if is_stale is not None:
+            return is_stale
+        is_stale = self._is_self_stale(task)
+        successors = list(self.dependencies.successors(task))
+        if successors:
+            is_stale |= any(self.is_stale(successors))
+        self.dependencies.nodes[task]["is_stale"] = is_stale
+        return is_stale
 
     def _is_self_stale(self, task: "Task") -> bool:
         """
         Determine whether a task is *itself* stale irrespective of other tasks it may depend on.
+
+        Args:
+            task: Task to check.
+
+        Returns:
+            If the task is stale, ignoring dependencies.
         """
         # If there are no targets or the targets are missing, the task is stale.
         if not task.targets:
-            LOGGER.debug('%s is "stale" because it has no targets', task)
+            LOGGER.debug('%s is stale because it has no targets', task)
             return True
-        if not all(path.is_file() for path in task.targets):
-            LOGGER.debug("%s is stale because one of its targets is missing", task)
+        for target in task.targets:
+            if not target.is_file():
+                LOGGER.debug("%s is stale because its target `%s` is missing", task, target)
+                return True
+
+        # If there is no digest in the database, the task is stale.
+        cached_digest = self.connection.execute("SELECT digest FROM tasks WHERE name = :name",
+                                                {"name": task.name}).fetchone()
+        if cached_digest is None:
+            LOGGER.debug("%s is stale because it does not have a hash entry", task)
             return True
 
-        # If any dependency is outdated, the task is stale.
-        for dependency in task.dependencies:
-            name = self.path_to_name(dependency)
-            result = self.connection.execute("SELECT size, digest FROM files WHERE name = :name",
-                                             {"name": name}).fetchone()
-            if result is None:
-                LOGGER.debug("%s is stale because its dependency `%s` does not have a hash entry",
-                             task, name)
-                return True
-            expected_size, expected_digest = result
-            if dependency.stat().st_size != expected_size \
-                    or util.evaluate_hexdigest(dependency) != expected_digest:
-                LOGGER.debug("%s is stale because its dependency `%s` has changed", task, name)
-                return True
+        # If one of the dependencies is missing, the task is stale.
+        current_digest = self._evaluate_task_hexdigest(task)
+        if current_digest is None:
+            LOGGER.debug("%s is stale because one of its dependencies is missing", task)
+
+        # If the digest has changed, the task is stale.
+        cached_digest, = cached_digest
+        if current_digest != cached_digest:
+            LOGGER.debug("%s is stale because one of its dependencies has changed (cached digest: "
+                         "%s, current digest: %s)", task, cached_digest, current_digest)
+            return True
 
         LOGGER.debug("%s is up to date", task)
         return False
 
-    def is_stale(self, task: "Task", recursive: bool = True) -> bool:
-        if not recursive:
-            return self._is_self_stale(task)
-
-        # Return the status if we have already evaluated it.
-        if (status := self.status.get(task)) is not None:
-            return status
-
-        # We will evaluate all dependents (rather than using "any" with a generator expression)
-        # because we want to find all stale tasks. Not just the first one in the hierarchy.
-        dependents = [self.is_stale(dependent) for dependent in self.dependencies.get(task, [])]
-        if any(dependents):
-            return self.status.setdefault(task, True)
-
-        return self.status.setdefault(task, self._is_self_stale(task))
-
-    async def execute(self, task: "Task") -> None:
-        if self.cancelled:  # pragma: no cover
-            return
+    def execute(self, tasks: "Task", num_concurrent: int = 1, interval: float = 1) -> None:
+        """
+        Execute one or more tasks.
 
-        # If there already is a future, just wait for it and return.
-        if future := self.futures.get(task):
-            await future
+        Args:
+            tasks: Tasks to execute.
+            num_concurrent: Number of concurrent threads to run.
+        """
+        if not isinstance(tasks, Sequence):
+            tasks = [tasks]
+        if not any(self.is_stale(tasks)):
             return
 
-        # Create a new future and add it to the lookup.
-        future = self.futures.setdefault(task, asyncio.Future())
-
-        # First execute all the dependents.
-        await asyncio.gather(*(self.execute(dependency) for dependency in
-                               self.dependencies.get(task, [])))
+        # Start the worker threads.
+        threads: List[threading.Thread] = []
+        input_queue = Queue()
+        output_queue = Queue()
+        stop = util.StopEvent(interval)
+        for i in range(num_concurrent):
+            thread = threading.Thread(target=self._target, name=f"cook-thread-{i}",
+                                      args=(stop, input_queue, output_queue), daemon=True)
+            thread.start()
+            threads.append(thread)
+
+        # Create a copy of the dependency graph and filter it to remove all non-stale tasks.
+        dependencies: nx.DiGraph = self.dependencies.copy()
+        not_stale = [node for node, data in dependencies.nodes.data() if not data.get("is_stale")]
+        dependencies.remove_nodes_from(not_stale)
+
+        # Initialize the input queue with leaf nodes.
+        for node, out_degree in dependencies.out_degree():
+            if out_degree == 0:
+                input_queue.put(node)
 
-        # Then do the actual processing within the semaphore to limit concurrency.
         try:
-            if self.is_stale(task):
-                async with self.semaphore:
-                    LOGGER.debug("started %s", task)
-                    with util.Timer() as timer:
-                        await task.execute()
-                    LOGGER.debug("completed %s in %.3f seconds", task, timer.duration)
+            while dependencies.number_of_nodes():
+                # Try to get the next item in the queue, continuing if there's nothing available.
+                try:
+                    item: Optional[Tuple["Task", sys._OptExcInfo]] = \
+                        output_queue.get(timeout=interval)
+                except Empty:
+                    continue
+
+                # Check if the stop event is set and abort if so.
+                if stop.is_set():
+                    break
+
+                assert item is not None, "output queue returned `None`; this is a bug"
+
+                # Unpack the results.
+                task, exc_info = item
+                if exc_info:
+                    raise util.FailedTaskError(task=task) from exc_info[1]
+
+                # Add tasks that are now leaf nodes to the tree.
+                predecessors = list(dependencies.predecessors(task))
+                dependencies.remove_node(task)
+                self.dependencies.add_node(task, is_stale=False)
+                for node, out_degree in dependencies.out_degree(predecessors):
+                    if out_degree == 0:
+                        input_queue.put(node)
 
-                # Validate that all desired targets exist.
+                # Verify that targets were created.
                 for target in task.targets:
                     if not target.is_file():
-                        raise FileNotFoundError(f"`{task}` did not create `{target}`")
+                        raise util.FailedTaskError(f"`{task}` did not create `{target}`",
+                                                   task=task)
                     LOGGER.debug("%s created `%s`", task, target)
 
-                # Update the state and write to the database.
-                self.status[task] = False
-                records = []
-                for dependency in task.dependencies:
-                    size, digest = self.evaluate_size_digest(dependency)
-                    records.append({
-                        "name": self.path_to_name(dependency),
-                        "size": size,
-                        "digest": digest,
-                    })
-                self.connection.executemany(QUERIES["upsert"], records)
-        except Exception as ex:
-            message = f"failed to execute {task}: {ex}"
-            LOGGER.exception(message)
-            error = util.FailedTaskError(message, task=task)
-            error.__cause__ = ex
-            future.set_exception(error)
-            # Cancel all other futures.
-            self.cancelled = True
-            for future in self.futures.values():
-                future.cancel(message) if sys.version_info[:2] > (3, 8) else future.cancel()
-        else:
-            future.set_result(None)
-
-        try:
-            await future
-        except asyncio.CancelledError:  # pragma: no cover
-            pass
-
-    def execute_sync(self, *tasks: "Task") -> None:
-        util.run_until_complete(*(self.execute(task) for task in tasks))
+                # Update the status in the database.
+                params = {"name": task.name, "digest": self._evaluate_task_hexdigest(task)}
+                self.connection.execute(QUERIES["upsert"], params)
+                self.connection.commit()
+        finally:
+            # Set the stop event and add "None" to the queue so the workers stop waiting.
+            LOGGER.debug("set stop event for threads: %s", [thread.name for thread in threads])
+            stop.set()
+            for thread in threads:
+                input_queue.put(None)
+
+            # Shut down the worker threads.
+            for thread in threads:
+                thread.join(stop.interval)
+                if thread.is_alive():  # pragma: no cover
+                    raise RuntimeError(f"thread {thread} failed to join")
+
+    def _target(self, stop: util.StopEvent, input_queue: Queue, output_queue: Queue) -> None:
+        LOGGER.debug(f"started thread `{threading.current_thread().name}`")
+        while not stop.is_set():
+            try:
+                task: "Task" = input_queue.get(stop.interval)
+            except Empty:  # pragma: no cover
+                # It's unlikely there's nothing on the queue, but let's handle it anyway.
+                continue
+            # Check the stop event before executing the task; it may have been set while we were
+            # waiting for the next task in the queue.
+            if stop.is_set():
+                break
+
+            assert task is not None, "input queue returned `None`; this is a bug"
+
+            try:
+                LOGGER.info("executing %s ...", task)
+                task.execute(stop)
+                output_queue.put((task, None))
+                LOGGER.info("completed %s", task)
+            except:  # noqa: E722
+                exc_info = sys.exc_info()
+                LOGGER.exception("failed to execute %s", task, exc_info=exc_info)
+                output_queue.put((task, sys.exc_info()))
+
+        # Put anything on the queue in case the parent is waiting.
+        LOGGER.debug(f"exiting thread `{threading.current_thread().name}`")
+        output_queue.put(None)
 
     def reset(self, *tasks: "Task") -> None:
-        names = []
-        for task in tasks:
-            for dependency in task.dependencies:
-                names.append({"name": self.path_to_name(dependency)})
-        self.connection.executemany("DELETE FROM files WHERE name = :name", names)
+        params = [{"name": task.name for task in tasks}]
+        self.connection.executemany("DELETE FROM tasks WHERE name = :name", params)
         self.connection.commit()
         LOGGER.info("reset %d %s", len(tasks), "task" if len(tasks) == 1 else "tasks")
```

### Comparing `cook-build-0.2.2/cook/manager.py` & `cook-build-0.3.0/cook/manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from __future__ import annotations
+import networkx as nx
 from pathlib import Path
 from typing import Dict, List, Optional, Set, Tuple, TYPE_CHECKING
 from . import task as task_
+from . import util
 
 
 if TYPE_CHECKING:
     from .actions import Action
     from .contexts import Context
     from .task import Task
 
@@ -50,15 +52,15 @@
         for context in reversed(self.contexts):
             task = context.apply(task)
             if task is None:
                 raise ValueError(f"{context} did not return a task")
         self.tasks[name] = task
         return task
 
-    def resolve_dependencies(self) -> Dict["Task", Set["Task"]]:
+    def resolve_dependencies(self) -> nx.DiGraph:
         """
         Resolve dependencies between tasks.
 
         Returns:
             Mapping from each task to the tasks it depends on.
         """
         # Run over all the targets and dependencies to explore connections between tasks.
@@ -86,15 +88,25 @@
                     dependencies.setdefault(dependent_task, set()).add(task)
             elif not file_dependency.is_file():
                 raise FileNotFoundError(
                     f"file {file_dependency} required by tasks {dependent_tasks} does not exist "
                     "nor is there a task to create it"
                 )
 
-        return dependencies
+        graph = nx.DiGraph()
+        graph.add_nodes_from(self.tasks.values())
+        graph.add_edges_from((task, dep) for task, deps in dependencies.items() for dep in deps)
+
+        try:
+            cycle = nx.find_cycle(graph)
+            raise util.CookError(f"dependency graph contains a cycle: {cycle}")
+        except nx.NetworkXNoCycle:
+            pass
+
+        return graph
 
 
 def create_task(name: str, *, action: Optional["Action"] = None,
                 targets: Optional[List["Path"]] = None, dependencies: Optional[List["Path"]] = None,
                 task_dependencies: Optional[List["Task"]] = None,
                 location: Optional[Tuple[str, int]] = None) -> "Task":
     """
```

### Comparing `cook-build-0.2.2/cook/task.py` & `cook-build-0.3.0/cook/task.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 from pathlib import Path
+import threading
 from typing import List, Optional, Tuple, TYPE_CHECKING
 from . import util
 
 
 if TYPE_CHECKING:
     from .util import PathOrStr
     from .actions import Action
@@ -26,17 +27,17 @@
         self.name = name
         self.dependencies = dependencies or []
         self.targets = [Path(path) for path in (targets or [])]
         self.action = action
         self.task_dependencies = task_dependencies or []
         self.location = location or util.get_location()
 
-    async def execute(self) -> None:
+    def execute(self, stop: Optional[threading.Event] = None) -> None:
         if self.action:
-            await self.action.execute(self)
+            self.action.execute(self, stop)
 
     def __hash__(self) -> int:
         return hash(self.name)
 
     def __repr__(self) -> str:
         filename, lineno = self.location
         return f"<task `{self.name}` @ {filename}:{lineno}>"
```

### Comparing `cook-build-0.2.2/cook_build.egg-info/PKG-INFO` & `cook-build-0.3.0/cook_build.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cook-build
-Version: 0.2.2
+Version: 0.3.0
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 🧑‍🍳 Cook
 ==========
 
@@ -38,33 +38,28 @@
     :cwd: examples/getting_started
 
     $ cook ls
     <task `src` @ /.../recipe.py:3>
     <task `cc` @ /.../recipe.py:4>
     <task `hello` @ /.../recipe.py:5>
 
-Running :code:`cook exec hello` creates the source file, compile it, and executes the binary. We use :code:`--log-level=debug` to provide additional information here.
+Running :code:`cook exec hello` creates the source file, compile it, and executes the binary (using :code:`--log-level=debug` can provide additional information).
 
 .. code-block::
 
     :cwd: examples/getting_started
     :stderr:
 
-    $ cook --log-level=debug exec hello
-    DEBUG: <task `src` @ .../recipe.py:3> is stale because one of its targets is missing
-    DEBUG: started <task `src` @ .../recipe.py:3>
-    DEBUG: completed <task `src` @ .../recipe.py:3> in ... seconds
-    DEBUG: <task `src` @ .../recipe.py:3> created `hello.c`
-    DEBUG: <task `cc` @ .../recipe.py:4> is stale because one of its targets is missing
-    DEBUG: started <task `cc` @ .../recipe.py:4>
-    DEBUG: completed <task `cc` @ .../recipe.py:4> in ... seconds
-    DEBUG: <task `cc` @ .../recipe.py:4> created `hello`
-    DEBUG: <task `hello` @ .../recipe.py:5> is "stale" because it has no targets
-    DEBUG: started <task `hello` @ .../recipe.py:5>
-    DEBUG: completed <task `hello` @ .../recipe.py:5> in ... seconds
+    $ cook exec hello
+    INFO: executing <task `src` @ /.../recipe.py:3> ...
+    INFO: completed <task `src` @ /.../recipe.py:3>
+    INFO: executing <task `cc` @ /.../recipe.py:4> ...
+    INFO: completed <task `cc` @ /.../recipe.py:4>
+    INFO: executing <task `hello` @ /.../recipe.py:5> ...
+    INFO: completed <task `hello` @ /.../recipe.py:5>
 
 To rerun a task, tell Cook to reset it.
 
 .. code-block::
 
     :cwd: examples/getting_started
     :stderr:
```

### Comparing `cook-build-0.2.2/cook_build.egg-info/SOURCES.txt` & `cook-build-0.3.0/cook_build.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cook-build-0.2.2/setup.py` & `cook-build-0.3.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,20 +10,21 @@
     .replace(":class:", ":code:") \
     .replace(".. toctree::", "..") \
     .replace(".. sh::", "..")
 
 
 setup(
     name="cook-build",
-    version="0.2.2",
+    version="0.3.0",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     python_requires=">=3.8",
     install_requires=[
         "colorama",
+        "networkx",
     ],
     packages=find_packages(),
     entry_points={
         "console_scripts": [
             "cook = cook.__main__:__main__",
         ],
     },
```

### Comparing `cook-build-0.2.2/tests/test_actions.py` & `cook-build-0.3.0/tests/test_actions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,51 +1,60 @@
-from cook.actions import CompositeAction, FunctionAction, ShellAction, SubprocessAction
+from cook.actions import CompositeAction, FunctionAction, SubprocessAction
+from cook.util import StopEvent, Timer
 from pathlib import Path
 import pytest
 from subprocess import SubprocessError
+import threading
+import time
 
 
 def test_shell_action(tmp_wd: Path) -> None:
-    action = ShellAction("echo hello > world.txt")
-    action.execute_sync(None)
+    action = SubprocessAction("echo hello > world.txt", shell=True)
+    action.execute(None)
     assert (tmp_wd / "world.txt").read_text().strip() == "hello"
 
 
+def test_shell_action_timeout() -> None:
+    stop = StopEvent(0.01)
+
+    def target():
+        time.sleep(1)
+        stop.set()
+
+    thread = threading.Thread(target=target)
+    thread.start()
+
+    action = SubprocessAction(["sleep", "2"])
+    with Timer() as timer, pytest.raises(SubprocessError, match="SIGTERM"):
+        action.execute(None, stop)
+
+    assert 1 < timer.duration < 2
+    assert not thread.is_alive()
+
+
 def test_subprocess_action(tmp_wd: Path) -> None:
-    action = SubprocessAction("touch", "foo")
-    action.execute_sync(None)
+    action = SubprocessAction(["touch", "foo"])
+    action.execute(None)
     assert (tmp_wd / "foo").is_file()
 
 
 def test_bad_subprocess_action() -> None:
     action = SubprocessAction("false")
     with pytest.raises(SubprocessError):
-        action.execute_sync(None)
+        action.execute(None)
 
 
 def test_function_action() -> None:
     args = []
 
     action = FunctionAction(args.append)
-    action.execute_sync(42)
+    action.execute(42)
 
     assert args == [42]
 
 
-def test_async_function_action() -> None:
-    args = []
-
-    async def func(*x) -> None:
-        args.append(*x)
-
-    action = FunctionAction(func)
-    action.execute_sync(17)
-
-    assert args == [17]
-
-
 def test_composite_action() -> None:
     args = []
 
     action = CompositeAction(FunctionAction(args.append), FunctionAction(args.append))
-    action.execute_sync("hello")
+    action.execute("hello")
     assert args == ["hello", "hello"]
```

### Comparing `cook-build-0.2.2/tests/test_contexts.py` & `cook-build-0.3.0/tests/test_contexts.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from cook import Manager, Task
-from cook.actions import CompositeAction, FunctionAction, ShellAction, SubprocessAction
+from cook.actions import CompositeAction, FunctionAction, SubprocessAction
 from cook.contexts import Context, create_target_directories, FunctionContext, create_group, \
     normalize_action, normalize_dependencies
 from cook.controller import Controller
 from pathlib import Path
 import pytest
 import sqlite3
 from typing import List
@@ -38,41 +38,43 @@
 
 def test_create_target_directories(m: Manager, tmp_wd: Path, conn: sqlite3.Connection) -> None:
     filename = tmp_wd / "this/is/a/hierarchy.txt"
     with normalize_action(), create_target_directories():
         task = m.create_task("foo", targets=[filename], action=["touch", filename])
     assert not filename.parent.is_dir()
 
-    controller = Controller(m, conn)
-    controller.execute_sync(task)
+    controller = Controller(m.resolve_dependencies(), conn)
+    controller.execute(task)
     assert filename.parent.is_dir()
 
 
 def test_create_target_directories_with_multiple_targets(m: Manager, tmp_wd: Path, conn: sqlite3) \
         -> None:
     filenames = [tmp_wd / "this/is/a/hierarchy.txt", tmp_wd / "this/is/a/hierarchy2.txt"]
     with normalize_action(), create_target_directories():
         for filename in filenames:
             task = m.create_task(filename.name, targets=[filename], action=["touch", filename])
     assert not filename.parent.is_dir()
 
-    controller = Controller(m, conn)
-    controller.execute_sync(task)
+    controller = Controller(m.resolve_dependencies(), conn)
+    controller.execute(task)
     assert filename.parent.is_dir()
 
 
 def test_normalize_action(m: Manager) -> None:
     with normalize_action():
         task = m.create_task("foo", action="bar")
-        assert isinstance(task.action, ShellAction) and task.action.cmd == "bar"
+        assert isinstance(task.action, SubprocessAction) and task.action.args[0] == "bar" \
+            and task.action.kwargs["shell"]
 
         task = m.create_task("bar", action=["baz"])
-        assert isinstance(task.action, SubprocessAction) and task.action.program == "baz"
+        assert isinstance(task.action, SubprocessAction) and task.action.args[0] == ["baz"] \
+            and not task.action.kwargs.get("shell")
 
-        actions = [ShellAction("hello"), SubprocessAction("world")]
+        actions = [SubprocessAction("hello", shell=True), SubprocessAction("world")]
         task = m.create_task("baz", action=actions)
         assert isinstance(task.action, CompositeAction) and task.action.actions == tuple(actions)
 
         task = m.create_task("xyz", action=lambda x: None)
         assert isinstance(task.action, FunctionAction)
```

### Comparing `cook-build-0.2.2/tests/test_main.py` & `cook-build-0.3.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `cook-build-0.2.2/tests/test_manager.py` & `cook-build-0.3.0/tests/test_manager.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from cook import Manager
 from cook.contexts import create_group, normalize_dependencies
+from cook.util import CookError
 from pathlib import Path
 import pytest
 
 
 def test_resolve_dependencies(m: Manager) -> None:
     Path("input1.txt").write_text("input1.txt")
     Path("input2.txt").write_text("input2.txt")
@@ -16,21 +17,23 @@
                                     targets=["output1.txt"])
             output2 = m.create_task("output2", targets=["output2.txt"],
                                     dependencies=["intermediate.txt", "input2.txt", "output1.txt"])
         special = m.create_task("special", dependencies=["intermediate.txt"])
         dependent = m.create_task("dependent", task_dependencies=[output1])
     dependencies = m.resolve_dependencies()
 
-    assert dependencies == {
+    expected = {
         output1: {intermediate},
         output2: {intermediate, output1},
         special: {intermediate},
         dependent: {output1},
         outputs.task: {output1, output2},
     }
+    for task, deps in expected.items():
+        assert set(dependencies.successors(task)) == deps
 
 
 def test_missing_file(m: Manager) -> None:
     with normalize_dependencies():
         m.create_task("has_missing_file_dependency", dependencies=["missing-file.txt"])
     with pytest.raises(FileNotFoundError, match="does not exist nor is"):
         m.resolve_dependencies()
@@ -54,7 +57,24 @@
         Manager.get_instance()
     with Manager() as m:
         assert Manager.get_instance() is m
     with pytest.raises(RuntimeError, match="unexpected manager"), Manager():
         Manager._INSTANCE = "asdf"
     with pytest.raises(ValueError, match="already active"), Manager(), Manager():
         pass
+
+
+def test_dependency_graph(m: Manager) -> None:
+    with normalize_dependencies():
+        bar = m.create_task("bar", targets=["a"])
+        foo = m.create_task("foo", dependencies=["a"])
+    dependencies = m.resolve_dependencies()
+    assert set(dependencies.successors(foo)) == {bar}
+    assert set(dependencies.predecessors(bar)) == {foo}
+
+
+def test_dependency_graph_cycle(m: Manager) -> None:
+    with normalize_dependencies():
+        m.create_task("bar", targets=["bar"], dependencies=["foo"])
+        m.create_task("foo", targets=["foo"], dependencies=["bar"])
+    with pytest.raises(CookError, match="contains a cycle"):
+        m.resolve_dependencies()
```

