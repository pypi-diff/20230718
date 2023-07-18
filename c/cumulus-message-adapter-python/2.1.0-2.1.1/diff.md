# Comparing `tmp/cumulus_message_adapter_python-2.1.0.tar.gz` & `tmp/cumulus_message_adapter_python-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cumulus_message_adapter_python-2.1.0.tar", last modified: Wed Feb  8 21:08:58 2023, max compression
+gzip compressed data, was "cumulus_message_adapter_python-2.1.1.tar", last modified: Tue Jul 18 19:15:48 2023, max compression
```

## Comparing `cumulus_message_adapter_python-2.1.0.tar` & `cumulus_message_adapter_python-2.1.1.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-08 21:08:58.000000 cumulus_message_adapter_python-2.1.0/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-08 21:08:58.000000 cumulus_message_adapter_python-2.1.0/cumulus_message_adapter_python.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7999 2023-02-08 21:08:58.000000 cumulus_message_adapter_python-2.1.0/cumulus_message_adapter_python.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      373 2023-02-08 21:08:58.000000 cumulus_message_adapter_python-2.1.0/cumulus_message_adapter_python.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-02-08 21:08:58.000000 cumulus_message_adapter_python-2.1.0/cumulus_message_adapter_python.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-02-08 21:08:58.000000 cumulus_message_adapter_python-2.1.0/cumulus_message_adapter_python.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       32 2023-02-08 21:08:58.000000 cumulus_message_adapter_python-2.1.0/cumulus_message_adapter_python.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9768 2023-02-08 21:08:45.000000 cumulus_message_adapter_python-2.1.0/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)       61 2023-02-08 21:08:45.000000 cumulus_message_adapter_python-2.1.0/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7351 2023-02-08 21:08:45.000000 cumulus_message_adapter_python-2.1.0/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13875 2023-02-08 21:08:45.000000 cumulus_message_adapter_python-2.1.0/cumulus_logger.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       39 2023-02-08 21:08:45.000000 cumulus_message_adapter_python-2.1.0/requirements.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3235 2023-02-08 21:08:45.000000 cumulus_message_adapter_python-2.1.0/run_cumulus_task.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2419 2023-02-08 21:08:45.000000 cumulus_message_adapter_python-2.1.0/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       23 2023-02-08 21:08:45.000000 cumulus_message_adapter_python-2.1.0/version.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7999 2023-02-08 21:08:58.000000 cumulus_message_adapter_python-2.1.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-02-08 21:08:58.000000 cumulus_message_adapter_python-2.1.0/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-18 19:15:48.208299 cumulus_message_adapter_python-2.1.1/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9768 2023-07-18 19:15:31.000000 cumulus_message_adapter_python-2.1.1/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2023-07-18 19:15:31.000000 cumulus_message_adapter_python-2.1.1/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8105 2023-07-18 19:15:48.208299 cumulus_message_adapter_python-2.1.1/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7494 2023-07-18 19:15:31.000000 cumulus_message_adapter_python-2.1.1/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13875 2023-07-18 19:15:31.000000 cumulus_message_adapter_python-2.1.1/cumulus_logger.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-18 19:15:48.208299 cumulus_message_adapter_python-2.1.1/cumulus_message_adapter_python.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8105 2023-07-18 19:15:48.000000 cumulus_message_adapter_python-2.1.1/cumulus_message_adapter_python.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      430 2023-07-18 19:15:48.000000 cumulus_message_adapter_python-2.1.1/cumulus_message_adapter_python.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-18 19:15:48.000000 cumulus_message_adapter_python-2.1.1/cumulus_message_adapter_python.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       31 2023-07-18 19:15:48.000000 cumulus_message_adapter_python-2.1.1/cumulus_message_adapter_python.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       32 2023-07-18 19:15:48.000000 cumulus_message_adapter_python-2.1.1/cumulus_message_adapter_python.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       31 2023-07-18 19:15:31.000000 cumulus_message_adapter_python-2.1.1/requirements.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3235 2023-07-18 19:15:31.000000 cumulus_message_adapter_python-2.1.1/run_cumulus_task.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-07-18 19:15:48.208299 cumulus_message_adapter_python-2.1.1/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2419 2023-07-18 19:15:31.000000 cumulus_message_adapter_python-2.1.1/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-18 19:15:48.208299 cumulus_message_adapter_python-2.1.1/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2859 2023-07-18 19:15:31.000000 cumulus_message_adapter_python-2.1.1/tests/test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1864 2023-07-18 19:15:31.000000 cumulus_message_adapter_python-2.1.1/tests/test_env_var.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6668 2023-07-18 19:15:31.000000 cumulus_message_adapter_python-2.1.1/tests/test_logger.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       23 2023-07-18 19:15:31.000000 cumulus_message_adapter_python-2.1.1/version.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cumulus_message_adapter_python-2.1.0/cumulus_message_adapter_python.egg-info/PKG-INFO` & `cumulus_message_adapter_python-2.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
-Name: cumulus-message-adapter-python
-Version: 2.1.0
+Name: cumulus_message_adapter_python
+Version: 2.1.1
 Summary: A handler library for cumulus tasks written in python
 Home-page: https://github.com/cumulus-nasa/cumulus-message-adapter-python
 Author: Cumulus Authors
 Author-email: info@developmentseed.org
-License: UNKNOWN
 Keywords: nasa cumulus
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -99,23 +97,24 @@
 
 ## Example
 
 Simple example of using this package's `run_cumulus_task` function as a wrapper
 around another function:
 
 ```python
-from run_cumulus_task import run_cumulus_task
+>>> from run_cumulus_task import run_cumulus_task
 
 # simple task that returns the event
-def task(event, context):
-    return event
+>>> def task(event, context):
+...     return event
 
 # handler that is provided to aws lambda
-def handler(event, context):
-    return run_cumulus_task(task, event, context)
+>>> def handler(event, context):
+...     return run_cumulus_task(task, event, context)
+
 ```
 
 For a full example see the [example folder](./example).
 
 ## Creating a deployment package
 
 Tasks that use this library are just standard AWS Lambda tasks. See
@@ -140,73 +139,84 @@
 Included in this package is the `cumulus_logger` which contains a logging class
 `CumulusLogger` that standardizes the log format for Cumulus. Methods are
 provided to log error, fatal, warning, debug, info, and trace.
 
 **Import the `CumulusLogger` class:**
 
 ```python
-from cumulus_logger import CumulusLogger
+>>> from cumulus_logger import CumulusLogger
+
 ```
 
 **Instantiate the logger inside the task definition (name and level are
 optional):**
 
 ```python
-logger = CumulusLogger(event, context)
+>>> import logging
+>>> logger = CumulusLogger("event_name", logging.ERROR)
+
 ```
 
 **Use the logging methods for different levels:**
 
 ```python
-logger.trace('<your message>')
-logger.debug('<your message>')
-logger.info('<your message>')
-logger.warn('<your message>')
-logger.error('<your message>')
-logger.fatal('<your message>')
+>>> logger.trace('<your message>')
+
+>>> logger.debug('<your message>')
+
+>>> logger.info('<your message>')
+
+>>> logger.warn('<your message>')
+
+>>> logger.error('<your message>')
+
+>>> logger.fatal('<your message>')
+
 ```
 
 **It can also take additional non-keyword and keyword arguments as in Python
 Logger.**
 
 The `msg` is the message format string, the `args` and `kwargs` are the
 arguments for string formatting.
 
 If `exc_info` in `kwargs` is not `False`, the exception information in the
 `exc_info` or `sys.exc_info()` is added to the message.
 
 ```python
-logger.debug(msg, *args, **kwargs)
+>>> logger.debug(msg, *args, **kwargs)
+
 ```
 
 **Example usage:**
 
 ```python
-import os
-import sys
+>>> import os
+>>> import sys
 
-from run_cumulus_task import run_cumulus_task
-from cumulus_logger import CumulusLogger
+>>> from run_cumulus_task import run_cumulus_task
+>>> from cumulus_logger import CumulusLogger
 
 # instantiate CumulusLogger
-logger = CumulusLogger()
-
-def task(event, context):
-    logger.info('task executed')
+>>> logger = CumulusLogger()
 
-    # log error when an exception is caught
-    logger.error("task formatted message {} exc_info ", "bar", exc_info=True)
+>>> def task(event, context):
+...     logger.info('task executed')
+... 
+...     # log error when an exception is caught
+...     logger.error("task formatted message {} exc_info ", "bar", exc_info=True)
+... 
+...     # return the output of the task
+...     return { "example": "output" }
+
+>>> def handler(event, context):
+...     # make sure event & context metadata is set in the logger
+...     logger.setMetadata(event, context)
+...     return run_cumulus_task(task, event, context)
 
-    # return the output of the task
-    return { "example": "output" }
-
-def handler(event, context):
-    # make sure event & context metadata is set in the logger
-    logger.setMetadata(event, context)
-    return run_cumulus_task(task, event, context)
 ```
 
 ### Running Tests
 
 Running tests requires [localstack](https://github.com/localstack/localstack).
 
 Tests only require localstack running S3, which can be initiated with the
@@ -215,15 +225,15 @@
 ```plain
 $ SERVICES=s3 localstack start
 ```
 
 And then you can check tests pass with the following nosetests command:
 
 ```plain
-$ CUMULUS_ENV=testing nosetests -v -s --with-doctest
+$ CUMULUS_ENV=testing nose2
 ```
 
 ### Linting
 
 ```plain
 $ pylint run_cumulus_task.py
 ```
@@ -252,12 +262,10 @@
 [circleci]:
   https://circleci.com/gh/nasa/cumulus-message-adapter-python.svg?style=svg
 [pypi version]:
   https://badge.fury.io/py/cumulus-message-adapter-python.svg
 [Cumulus Documentation]:
   https://nasa.github.io/cumulus/
 [creating release packages]:
-  https://docs.aws.amazon.com/lambda/latest/dg/deployment-package-v2.html
+  https://docs.aws.amazon.com/lambda/latest/dg/gettingstarted-package.html
 [cumulus workflow documenation]:
   https://nasa.github.io/cumulus/docs/workflows/input_output
-
-
```

### Comparing `cumulus_message_adapter_python-2.1.0/LICENSE` & `cumulus_message_adapter_python-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cumulus_message_adapter_python-2.1.0/README.md` & `cumulus_message_adapter_python-2.1.1/cumulus_message_adapter_python.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: cumulus-message-adapter-python
+Version: 2.1.1
+Summary: A handler library for cumulus tasks written in python
+Home-page: https://github.com/cumulus-nasa/cumulus-message-adapter-python
+Author: Cumulus Authors
+Author-email: info@developmentseed.org
+Keywords: nasa cumulus
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # cumulus-message-adapter-python
 
 [![CircleCI]](https://circleci.com/gh/nasa/cumulus-message-adapter-python)
 [![PyPI version]](https://badge.fury.io/py/cumulus-message-adapter-python)
 
 ## What is Cumulus?
 
@@ -81,23 +97,24 @@
 
 ## Example
 
 Simple example of using this package's `run_cumulus_task` function as a wrapper
 around another function:
 
 ```python
-from run_cumulus_task import run_cumulus_task
+>>> from run_cumulus_task import run_cumulus_task
 
 # simple task that returns the event
-def task(event, context):
-    return event
+>>> def task(event, context):
+...     return event
 
 # handler that is provided to aws lambda
-def handler(event, context):
-    return run_cumulus_task(task, event, context)
+>>> def handler(event, context):
+...     return run_cumulus_task(task, event, context)
+
 ```
 
 For a full example see the [example folder](./example).
 
 ## Creating a deployment package
 
 Tasks that use this library are just standard AWS Lambda tasks. See
@@ -122,73 +139,84 @@
 Included in this package is the `cumulus_logger` which contains a logging class
 `CumulusLogger` that standardizes the log format for Cumulus. Methods are
 provided to log error, fatal, warning, debug, info, and trace.
 
 **Import the `CumulusLogger` class:**
 
 ```python
-from cumulus_logger import CumulusLogger
+>>> from cumulus_logger import CumulusLogger
+
 ```
 
 **Instantiate the logger inside the task definition (name and level are
 optional):**
 
 ```python
-logger = CumulusLogger(event, context)
+>>> import logging
+>>> logger = CumulusLogger("event_name", logging.ERROR)
+
 ```
 
 **Use the logging methods for different levels:**
 
 ```python
-logger.trace('<your message>')
-logger.debug('<your message>')
-logger.info('<your message>')
-logger.warn('<your message>')
-logger.error('<your message>')
-logger.fatal('<your message>')
+>>> logger.trace('<your message>')
+
+>>> logger.debug('<your message>')
+
+>>> logger.info('<your message>')
+
+>>> logger.warn('<your message>')
+
+>>> logger.error('<your message>')
+
+>>> logger.fatal('<your message>')
+
 ```
 
 **It can also take additional non-keyword and keyword arguments as in Python
 Logger.**
 
 The `msg` is the message format string, the `args` and `kwargs` are the
 arguments for string formatting.
 
 If `exc_info` in `kwargs` is not `False`, the exception information in the
 `exc_info` or `sys.exc_info()` is added to the message.
 
 ```python
-logger.debug(msg, *args, **kwargs)
+>>> logger.debug(msg, *args, **kwargs)
+
 ```
 
 **Example usage:**
 
 ```python
-import os
-import sys
+>>> import os
+>>> import sys
 
-from run_cumulus_task import run_cumulus_task
-from cumulus_logger import CumulusLogger
+>>> from run_cumulus_task import run_cumulus_task
+>>> from cumulus_logger import CumulusLogger
 
 # instantiate CumulusLogger
-logger = CumulusLogger()
-
-def task(event, context):
-    logger.info('task executed')
-
-    # log error when an exception is caught
-    logger.error("task formatted message {} exc_info ", "bar", exc_info=True)
+>>> logger = CumulusLogger()
 
-    # return the output of the task
-    return { "example": "output" }
+>>> def task(event, context):
+...     logger.info('task executed')
+... 
+...     # log error when an exception is caught
+...     logger.error("task formatted message {} exc_info ", "bar", exc_info=True)
+... 
+...     # return the output of the task
+...     return { "example": "output" }
+
+>>> def handler(event, context):
+...     # make sure event & context metadata is set in the logger
+...     logger.setMetadata(event, context)
+...     return run_cumulus_task(task, event, context)
 
-def handler(event, context):
-    # make sure event & context metadata is set in the logger
-    logger.setMetadata(event, context)
-    return run_cumulus_task(task, event, context)
 ```
 
 ### Running Tests
 
 Running tests requires [localstack](https://github.com/localstack/localstack).
 
 Tests only require localstack running S3, which can be initiated with the
@@ -197,15 +225,15 @@
 ```plain
 $ SERVICES=s3 localstack start
 ```
 
 And then you can check tests pass with the following nosetests command:
 
 ```plain
-$ CUMULUS_ENV=testing nosetests -v -s --with-doctest
+$ CUMULUS_ENV=testing nose2
 ```
 
 ### Linting
 
 ```plain
 $ pylint run_cumulus_task.py
 ```
@@ -234,10 +262,10 @@
 [circleci]:
   https://circleci.com/gh/nasa/cumulus-message-adapter-python.svg?style=svg
 [pypi version]:
   https://badge.fury.io/py/cumulus-message-adapter-python.svg
 [Cumulus Documentation]:
   https://nasa.github.io/cumulus/
 [creating release packages]:
-  https://docs.aws.amazon.com/lambda/latest/dg/deployment-package-v2.html
+  https://docs.aws.amazon.com/lambda/latest/dg/gettingstarted-package.html
 [cumulus workflow documenation]:
   https://nasa.github.io/cumulus/docs/workflows/input_output
```

### Comparing `cumulus_message_adapter_python-2.1.0/cumulus_logger.py` & `cumulus_message_adapter_python-2.1.1/cumulus_logger.py`

 * *Files identical despite different names*

### Comparing `cumulus_message_adapter_python-2.1.0/run_cumulus_task.py` & `cumulus_message_adapter_python-2.1.1/run_cumulus_task.py`

 * *Files identical despite different names*

### Comparing `cumulus_message_adapter_python-2.1.0/setup.py` & `cumulus_message_adapter_python-2.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `cumulus_message_adapter_python-2.1.0/PKG-INFO` & `cumulus_message_adapter_python-2.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: cumulus_message_adapter_python
-Version: 2.1.0
-Summary: A handler library for cumulus tasks written in python
-Home-page: https://github.com/cumulus-nasa/cumulus-message-adapter-python
-Author: Cumulus Authors
-Author-email: info@developmentseed.org
-License: UNKNOWN
-Keywords: nasa cumulus
-Platform: UNKNOWN
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # cumulus-message-adapter-python
 
 [![CircleCI]](https://circleci.com/gh/nasa/cumulus-message-adapter-python)
 [![PyPI version]](https://badge.fury.io/py/cumulus-message-adapter-python)
 
 ## What is Cumulus?
 
@@ -99,23 +81,24 @@
 
 ## Example
 
 Simple example of using this package's `run_cumulus_task` function as a wrapper
 around another function:
 
 ```python
-from run_cumulus_task import run_cumulus_task
+>>> from run_cumulus_task import run_cumulus_task
 
 # simple task that returns the event
-def task(event, context):
-    return event
+>>> def task(event, context):
+...     return event
 
 # handler that is provided to aws lambda
-def handler(event, context):
-    return run_cumulus_task(task, event, context)
+>>> def handler(event, context):
+...     return run_cumulus_task(task, event, context)
+
 ```
 
 For a full example see the [example folder](./example).
 
 ## Creating a deployment package
 
 Tasks that use this library are just standard AWS Lambda tasks. See
@@ -140,73 +123,84 @@
 Included in this package is the `cumulus_logger` which contains a logging class
 `CumulusLogger` that standardizes the log format for Cumulus. Methods are
 provided to log error, fatal, warning, debug, info, and trace.
 
 **Import the `CumulusLogger` class:**
 
 ```python
-from cumulus_logger import CumulusLogger
+>>> from cumulus_logger import CumulusLogger
+
 ```
 
 **Instantiate the logger inside the task definition (name and level are
 optional):**
 
 ```python
-logger = CumulusLogger(event, context)
+>>> import logging
+>>> logger = CumulusLogger("event_name", logging.ERROR)
+
 ```
 
 **Use the logging methods for different levels:**
 
 ```python
-logger.trace('<your message>')
-logger.debug('<your message>')
-logger.info('<your message>')
-logger.warn('<your message>')
-logger.error('<your message>')
-logger.fatal('<your message>')
+>>> logger.trace('<your message>')
+
+>>> logger.debug('<your message>')
+
+>>> logger.info('<your message>')
+
+>>> logger.warn('<your message>')
+
+>>> logger.error('<your message>')
+
+>>> logger.fatal('<your message>')
+
 ```
 
 **It can also take additional non-keyword and keyword arguments as in Python
 Logger.**
 
 The `msg` is the message format string, the `args` and `kwargs` are the
 arguments for string formatting.
 
 If `exc_info` in `kwargs` is not `False`, the exception information in the
 `exc_info` or `sys.exc_info()` is added to the message.
 
 ```python
-logger.debug(msg, *args, **kwargs)
+>>> logger.debug(msg, *args, **kwargs)
+
 ```
 
 **Example usage:**
 
 ```python
-import os
-import sys
+>>> import os
+>>> import sys
 
-from run_cumulus_task import run_cumulus_task
-from cumulus_logger import CumulusLogger
+>>> from run_cumulus_task import run_cumulus_task
+>>> from cumulus_logger import CumulusLogger
 
 # instantiate CumulusLogger
-logger = CumulusLogger()
-
-def task(event, context):
-    logger.info('task executed')
+>>> logger = CumulusLogger()
 
-    # log error when an exception is caught
-    logger.error("task formatted message {} exc_info ", "bar", exc_info=True)
+>>> def task(event, context):
+...     logger.info('task executed')
+... 
+...     # log error when an exception is caught
+...     logger.error("task formatted message {} exc_info ", "bar", exc_info=True)
+... 
+...     # return the output of the task
+...     return { "example": "output" }
+
+>>> def handler(event, context):
+...     # make sure event & context metadata is set in the logger
+...     logger.setMetadata(event, context)
+...     return run_cumulus_task(task, event, context)
 
-    # return the output of the task
-    return { "example": "output" }
-
-def handler(event, context):
-    # make sure event & context metadata is set in the logger
-    logger.setMetadata(event, context)
-    return run_cumulus_task(task, event, context)
 ```
 
 ### Running Tests
 
 Running tests requires [localstack](https://github.com/localstack/localstack).
 
 Tests only require localstack running S3, which can be initiated with the
@@ -215,15 +209,15 @@
 ```plain
 $ SERVICES=s3 localstack start
 ```
 
 And then you can check tests pass with the following nosetests command:
 
 ```plain
-$ CUMULUS_ENV=testing nosetests -v -s --with-doctest
+$ CUMULUS_ENV=testing nose2
 ```
 
 ### Linting
 
 ```plain
 $ pylint run_cumulus_task.py
 ```
@@ -252,12 +246,10 @@
 [circleci]:
   https://circleci.com/gh/nasa/cumulus-message-adapter-python.svg?style=svg
 [pypi version]:
   https://badge.fury.io/py/cumulus-message-adapter-python.svg
 [Cumulus Documentation]:
   https://nasa.github.io/cumulus/
 [creating release packages]:
-  https://docs.aws.amazon.com/lambda/latest/dg/deployment-package-v2.html
+  https://docs.aws.amazon.com/lambda/latest/dg/gettingstarted-package.html
 [cumulus workflow documenation]:
   https://nasa.github.io/cumulus/docs/workflows/input_output
-
-
```

