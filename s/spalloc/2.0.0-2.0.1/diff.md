# Comparing `tmp/spalloc-2.0.0.tar.gz` & `tmp/spalloc-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\spalloc-2.0.0.tar", last modified: Fri Aug  9 13:43:08 2019, max compression
+gzip compressed data, was "dist\spalloc-2.0.1.tar", last modified: Fri Nov 15 15:21:20 2019, max compression
```

## Comparing `spalloc-2.0.0.tar` & `spalloc-2.0.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2019-08-09 13:43:08.000000 spalloc-2.0.0/
--rw-rw-rw-   0        0        0     2333 2019-07-25 09:40:49.000000 spalloc-2.0.0/CITATION.cff
--rw-rw-rw-   0        0        0      993 2017-09-01 13:38:32.000000 spalloc-2.0.0/LICENSE.md
--rw-rw-rw-   0        0        0       63 2019-06-12 10:22:43.000000 spalloc-2.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1140 2019-08-09 13:43:08.000000 spalloc-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       18 2019-06-12 10:22:43.000000 spalloc-2.0.0/pypi_to_import
--rw-rw-rw-   0        0        0     1870 2017-03-22 10:42:32.000000 spalloc-2.0.0/README.rst
--rw-rw-rw-   0        0        0      743 2019-07-25 09:40:49.000000 spalloc-2.0.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2019-08-09 13:43:08.000000 spalloc-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0     2610 2019-08-02 07:22:50.000000 spalloc-2.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2019-08-09 13:43:08.000000 spalloc-2.0.0/spalloc/
--rw-rw-rw-   0        0        0     6968 2019-07-25 09:40:49.000000 spalloc-2.0.0/spalloc/config.py
--rw-rw-rw-   0        0        0    31597 2019-07-25 09:40:49.000000 spalloc-2.0.0/spalloc/job.py
--rw-rw-rw-   0        0        0    15215 2019-07-25 09:40:49.000000 spalloc-2.0.0/spalloc/protocol_client.py
-drwxrwxrwx   0        0        0        0 2019-08-09 13:43:08.000000 spalloc-2.0.0/spalloc/scripts/
--rw-rw-rw-   0        0        0    20823 2019-07-25 09:40:49.000000 spalloc-2.0.0/spalloc/scripts/alloc.py
--rw-rw-rw-   0        0        0    13037 2019-07-25 09:40:49.000000 spalloc-2.0.0/spalloc/scripts/job.py
--rw-rw-rw-   0        0        0    10209 2019-07-25 09:40:49.000000 spalloc-2.0.0/spalloc/scripts/machine.py
--rw-rw-rw-   0        0        0     5813 2019-07-25 09:40:49.000000 spalloc-2.0.0/spalloc/scripts/ps.py
--rw-rw-rw-   0        0        0     3827 2019-07-25 09:40:49.000000 spalloc-2.0.0/spalloc/scripts/support.py
--rw-rw-rw-   0        0        0     6596 2019-07-25 09:40:49.000000 spalloc-2.0.0/spalloc/scripts/where_is.py
--rw-rw-rw-   0        0        0      691 2019-07-25 09:40:49.000000 spalloc-2.0.0/spalloc/scripts/__init__.py
--rw-rw-rw-   0        0        0     1353 2019-07-25 09:40:49.000000 spalloc-2.0.0/spalloc/states.py
--rw-rw-rw-   0        0        0    16045 2019-07-25 09:40:49.000000 spalloc-2.0.0/spalloc/term.py
--rw-rw-rw-   0        0        0     4067 2019-07-25 09:40:49.000000 spalloc-2.0.0/spalloc/_keepalive_process.py
--rw-rw-rw-   0        0        0     1241 2019-07-25 09:40:49.000000 spalloc-2.0.0/spalloc/_utils.py
--rw-rw-rw-   0        0        0      830 2019-08-09 13:06:16.000000 spalloc-2.0.0/spalloc/_version.py
--rw-rw-rw-   0        0        0     1095 2019-07-25 09:40:49.000000 spalloc-2.0.0/spalloc/__init__.py
-drwxrwxrwx   0        0        0        0 2019-08-09 13:43:08.000000 spalloc-2.0.0/spalloc.egg-info/
--rw-rw-rw-   0        0        0        1 2019-08-09 13:43:07.000000 spalloc-2.0.0/spalloc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      228 2019-08-09 13:43:07.000000 spalloc-2.0.0/spalloc.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0     1140 2019-08-09 13:43:07.000000 spalloc-2.0.0/spalloc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       51 2019-08-09 13:43:07.000000 spalloc-2.0.0/spalloc.egg-info/requires.txt
--rw-rw-rw-   0        0        0      777 2019-08-09 13:43:08.000000 spalloc-2.0.0/spalloc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       14 2019-08-09 13:43:07.000000 spalloc-2.0.0/spalloc.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2019-08-09 13:43:08.000000 spalloc-2.0.0/tests/
--rw-rw-rw-   0        0        0     2171 2019-07-25 09:40:49.000000 spalloc-2.0.0/tests/common.py
--rw-rw-rw-   0        0        0     3270 2019-07-25 09:40:49.000000 spalloc-2.0.0/tests/conftest.py
--rw-rw-rw-   0        0        0     3039 2019-07-25 09:40:49.000000 spalloc-2.0.0/tests/test_config.py
--rw-rw-rw-   0        0        0    20204 2019-07-25 09:40:49.000000 spalloc-2.0.0/tests/test_job.py
--rw-rw-rw-   0        0        0     8011 2019-07-25 09:40:49.000000 spalloc-2.0.0/tests/test_protocol_client.py
--rw-rw-rw-   0        0        0     9845 2019-07-25 09:40:49.000000 spalloc-2.0.0/tests/test_term.py
--rw-rw-rw-   0        0        0      691 2019-07-25 09:40:49.000000 spalloc-2.0.0/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-15 15:21:20.000000 spalloc-2.0.1/
+-rw-rw-rw-   0        0        0     2333 2019-07-25 09:40:49.000000 spalloc-2.0.1/CITATION.cff
+-rw-rw-rw-   0        0        0      993 2017-09-01 13:38:32.000000 spalloc-2.0.1/LICENSE.md
+-rw-rw-rw-   0        0        0       63 2019-06-12 10:22:43.000000 spalloc-2.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1040 2019-11-15 15:21:20.000000 spalloc-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       18 2019-06-12 10:22:43.000000 spalloc-2.0.1/pypi_to_import
+-rw-rw-rw-   0        0        0     1870 2017-03-22 10:42:32.000000 spalloc-2.0.1/README.rst
+-rw-rw-rw-   0        0        0      743 2019-07-25 09:40:49.000000 spalloc-2.0.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2019-11-15 15:21:20.000000 spalloc-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     2514 2019-09-02 07:38:33.000000 spalloc-2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2019-11-15 15:21:20.000000 spalloc-2.0.1/spalloc/
+-rw-rw-rw-   0        0        0     7034 2019-10-22 12:00:46.000000 spalloc-2.0.1/spalloc/config.py
+-rw-rw-rw-   0        0        0    31525 2019-10-22 12:00:46.000000 spalloc-2.0.1/spalloc/job.py
+-rw-rw-rw-   0        0        0    15262 2019-11-13 07:58:14.000000 spalloc-2.0.1/spalloc/protocol_client.py
+drwxrwxrwx   0        0        0        0 2019-11-15 15:21:20.000000 spalloc-2.0.1/spalloc/scripts/
+-rw-rw-rw-   0        0        0    20820 2019-10-22 12:00:46.000000 spalloc-2.0.1/spalloc/scripts/alloc.py
+-rw-rw-rw-   0        0        0    13003 2019-10-22 12:00:46.000000 spalloc-2.0.1/spalloc/scripts/job.py
+-rw-rw-rw-   0        0        0    10123 2019-10-22 12:00:46.000000 spalloc-2.0.1/spalloc/scripts/machine.py
+-rw-rw-rw-   0        0        0     5813 2019-07-25 09:40:49.000000 spalloc-2.0.1/spalloc/scripts/ps.py
+-rw-rw-rw-   0        0        0     3963 2019-10-22 12:00:46.000000 spalloc-2.0.1/spalloc/scripts/support.py
+-rw-rw-rw-   0        0        0     6523 2019-10-22 12:00:46.000000 spalloc-2.0.1/spalloc/scripts/where_is.py
+-rw-rw-rw-   0        0        0      691 2019-07-25 09:40:49.000000 spalloc-2.0.1/spalloc/scripts/__init__.py
+-rw-rw-rw-   0        0        0     1353 2019-07-25 09:40:49.000000 spalloc-2.0.1/spalloc/states.py
+-rw-rw-rw-   0        0        0    15972 2019-10-22 12:00:46.000000 spalloc-2.0.1/spalloc/term.py
+-rw-rw-rw-   0        0        0     4050 2019-10-22 12:00:46.000000 spalloc-2.0.1/spalloc/_keepalive_process.py
+-rw-rw-rw-   0        0        0     1241 2019-07-25 09:40:49.000000 spalloc-2.0.1/spalloc/_utils.py
+-rw-rw-rw-   0        0        0      832 2019-11-15 15:20:36.000000 spalloc-2.0.1/spalloc/_version.py
+-rw-rw-rw-   0        0        0     1095 2019-07-25 09:40:49.000000 spalloc-2.0.1/spalloc/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-15 15:21:20.000000 spalloc-2.0.1/spalloc.egg-info/
+-rw-rw-rw-   0        0        0        1 2019-11-15 15:21:20.000000 spalloc-2.0.1/spalloc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      228 2019-11-15 15:21:20.000000 spalloc-2.0.1/spalloc.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0     1040 2019-11-15 15:21:20.000000 spalloc-2.0.1/spalloc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       51 2019-11-15 15:21:20.000000 spalloc-2.0.1/spalloc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      777 2019-11-15 15:21:20.000000 spalloc-2.0.1/spalloc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       14 2019-11-15 15:21:20.000000 spalloc-2.0.1/spalloc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2019-11-15 15:21:20.000000 spalloc-2.0.1/tests/
+-rw-rw-rw-   0        0        0     2171 2019-07-25 09:40:49.000000 spalloc-2.0.1/tests/common.py
+-rw-rw-rw-   0        0        0     3270 2019-07-25 09:40:49.000000 spalloc-2.0.1/tests/conftest.py
+-rw-rw-rw-   0        0        0     3039 2019-07-25 09:40:49.000000 spalloc-2.0.1/tests/test_config.py
+-rw-rw-rw-   0        0        0    20204 2019-07-25 09:40:49.000000 spalloc-2.0.1/tests/test_job.py
+-rw-rw-rw-   0        0        0     8011 2019-07-25 09:40:49.000000 spalloc-2.0.1/tests/test_protocol_client.py
+-rw-rw-rw-   0        0        0     9772 2019-10-22 12:00:46.000000 spalloc-2.0.1/tests/test_term.py
+-rw-rw-rw-   0        0        0      691 2019-07-25 09:40:49.000000 spalloc-2.0.1/tests/__init__.py
```

### Comparing `spalloc-2.0.0/CITATION.cff` & `spalloc-2.0.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `spalloc-2.0.0/LICENSE.md` & `spalloc-2.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `spalloc-2.0.0/PKG-INFO` & `spalloc-2.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: spalloc
-Version: 2.0.0
+Version: 2.0.1
 Summary: A client for the spalloc_server SpiNNaker machine partitioning and allocation system.
 Home-page: https://github.com/SpiNNakerManchester/spalloc
 Author: Jonathan Heathcote
 Maintainer: SpiNNakerTeam
 Maintainer-email: spinnakerusers@googlegroups.com
 License: GPLv2
 Description: UNKNOWN
@@ -14,13 +14,11 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `spalloc-2.0.0/README.rst` & `spalloc-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `spalloc-2.0.0/requirements.txt` & `spalloc-2.0.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `spalloc-2.0.0/setup.py` & `spalloc-2.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,16 +40,14 @@
 
         "Natural Language :: English",
 
         "Operating System :: POSIX :: Linux",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS",
 
-        "Programming Language :: Python :: 2",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
     ],
     keywords="spinnaker allocation packing management supercomputer",
```

### Comparing `spalloc-2.0.0/spalloc/config.py` & `spalloc-2.0.1/spalloc/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,20 +75,18 @@
     The maximum number of dead links which may be present in an allocated set
     of boards or None to allow any number of dead links. (Default: None)
 ``require_torus``
     If True, require that an allocation have wrap-around links. This typically
     requires the allocation of a whole machine. If False, wrap-around links may
     or may-not be present in allocated machines. (Default: False)
 """
-# pylint: disable=import-error
-import os
 import os.path
 import appdirs
 from six import iteritems
-from six.moves.configparser import ConfigParser, NoOptionError
+from six.moves import configparser
 
 # The application name to use in config file names
 _name = "spalloc"
 
 # Standard config file names/locations
 SYSTEM_CONFIG_FILE = appdirs.site_config_dir(_name)
 USER_CONFIG_FILE = appdirs.user_config_dir(_name)
@@ -126,15 +124,15 @@
         return None
     return parser.getint(SECTION, option)
 
 
 def _read_any_str(parser, option):
     try:
         return parser.get(SECTION, option)
-    except NoOptionError:
+    except configparser.NoOptionError:
         return None
 
 
 def _read_none_or_str(parser, option):
     if parser.get(SECTION, option) == "None":
         return None
     return parser.get(SECTION, option)
@@ -152,26 +150,27 @@
     Returns
     -------
     dict
         The configuration loaded.
     """
     if filenames is None:  # pragma: no cover
         filenames = SEARCH_PATH
-    parser = ConfigParser()
+    parser = configparser.ConfigParser()
 
     # Set default config values (NB: No read_dict in Python 2.7)
     parser.add_section(SECTION)
     for key, value in iteritems(DEFAULT_CONFIG):
         parser.set(SECTION, key, value)
 
     # Attempt to read from each possible file location in turn
     for filename in filenames:
         try:
             with open(filename, "r") as f:
-                parser.readfp(f, filename)
+                # TODO: Switch to read_file once we stop supporting 2.7
+                parser.readfp(f, filename)  # pylint: disable=deprecated-method
         except (IOError, OSError):
             # File did not exist, keep trying
             pass
 
     cfg = {
         "hostname":        _read_any_str(parser, "hostname"),
         "owner":           _read_any_str(parser, "owner"),
```

### Comparing `spalloc-2.0.0/spalloc/job.py` & `spalloc-2.0.1/spalloc/job.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,18 +11,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 """ A high-level Python interface for allocating SpiNNaker boards.
 """
-try:
-    from collections.abc import namedtuple
-except ImportError:
-    from collections import namedtuple
+from collections import namedtuple
 import logging
 import subprocess
 import time
 import sys
 from .protocol_client import ProtocolClient, ProtocolTimeoutError
 from .config import read_config, SEARCH_PATH
 from .states import JobState
```

### Comparing `spalloc-2.0.0/spalloc/protocol_client.py` & `spalloc-2.0.1/spalloc/protocol_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,18 +11,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 """ A simple blocking spalloc_server protocol implementation.
 """
-try:
-    from collections.abc import deque
-except ImportError:
-    from collections import deque
+from collections import deque
 import errno
 import json
 import socket
 import sys
 from threading import current_thread, RLock, local
 from six import raise_from
 from spalloc._utils import time_left, timed_out, make_timeout
@@ -46,14 +43,15 @@
 
 class _ProtocolThreadLocal(local):
     """ Subclass of threading.local to ensure that we get sane initialisation\
         of our state in each thread.
     """
     # See https://github.com/SpiNNakerManchester/spalloc/issues/12
     def __init__(self):
+        local.__init__(self)
         self.buffer = b""
         self.sock = None
 
 
 class ProtocolClient(object):
     """ A simple (blocking) client implementation of the `spalloc-server
     <https://github.com/project-rig/spalloc_server>`_ protocol.
@@ -87,15 +85,15 @@
 
             Does not connect to the server until :py:meth:`.connect` is called.
 
         Parameters
         ----------
         hostname : str
             The hostname of the server.
-        port : str
+        port : str or int
             The port to use (default: 22244).
         """
         self._hostname = hostname
         self._port = port
         # Mapping from threads to sockets. Kept because we need to have way to
         # shut down all sockets at once.
         self._socks = dict()
@@ -148,16 +146,16 @@
         success = False
         try:
             sock.connect((self._hostname, self._port))
             success = True
         except OSError as e:
             if e.errno != errno.EISCONN:
                 raise
-        except socket.error as e:
-            if e[0] != errno.EISCONN:
+        except socket.error as e:  # pylint: disable=duplicate-except
+            if e[0] != errno.EISCONN:  # pylint: disable=unsubscriptable-object
                 raise
         return success
 
     def _has_open_socket(self):
         return self._local.sock is not None
 
     def connect(self, timeout=None):
```

### Comparing `spalloc-2.0.0/spalloc/scripts/alloc.py` & `spalloc-2.0.1/spalloc/scripts/alloc.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,18 +107,15 @@
 
 Note that by default, jobs require a 'keepalive' message to be sent to the
 server at a regular interval. While the ``spalloc`` command is running, these
 messages are sent automatically but after exiting the commands are no longer
 sent. Adding the ``--keepalive -1`` option when creating a job disables this.
 """
 import argparse
-try:
-    from collections.abc import OrderedDict
-except ImportError:
-    from collections import OrderedDict
+from collections import OrderedDict
 import logging
 import os
 import subprocess
 import sys
 import tempfile
 from six import iteritems
 from six.moves import input, shlex_quote  # @UnresolvedImport
@@ -128,14 +125,17 @@
 from spalloc.term import Terminal, render_definitions
 # Rig is used to implement the optional '--boot' facility.
 try:
     from rig.machine_control import MachineController
 except ImportError:  # pragma: no cover
     MachineController = None
 
+arguments = None
+t = None
+
 
 def write_ips_to_csv(connections, ip_file_filename):
     """ Write the supplied IP addresses to a CSV file.
 
     The produced CSV has three columns: x, y and hostname where x and y give
     chip coordinates of Ethernet-connected chips and hostname gives the IP
     address for that chip.
@@ -162,32 +162,32 @@
         The machine the job is running on.
     connections : {(x, y): hostname, ...}
         The connections to the boards.
     width, height : int
         The width and height of the machine in chips.
     ip_file_filename : str
     """
-    t = Terminal()
+    t_stdout = Terminal()
 
     to_print = OrderedDict()
 
-    to_print["Hostname"] = t.bright(connections[(0, 0)])
+    to_print["Hostname"] = t_stdout.bright(connections[(0, 0)])
     to_print["Width"] = width
     to_print["Height"] = height
 
     if len(connections) > 1:
         to_print["Num boards"] = len(connections)
         to_print["All hostnames"] = ip_file_filename
 
     to_print["Running on"] = machine_name
 
     print(render_definitions(to_print))
 
     try:
-        input(t.dim("<Press enter when done>"))
+        input(t_stdout.dim("<Press enter when done>"))
     except (KeyboardInterrupt, EOFError):
         print("")
 
 
 def run_command(command, job_id, machine_name, connections, width, height,
                 ip_file_filename):
     """ Run a user-specified command, substituting arguments for values taken
@@ -254,15 +254,15 @@
         try:
             return p.wait()
         except KeyboardInterrupt:
             p.terminate()
 
 
 def info(msg):
-    if not args.quiet:
+    if not arguments.quiet:
         t.stream.write("{}\n".format(msg))
 
 
 def update(msg, colour, *args):
     info(t.update(colour(msg.format(*args))))
 
 
@@ -442,89 +442,90 @@
         if code != 0:
             return code
 
         # Machine is now ready
         write_ips_to_csv(job.connections, ip_file_filename)
 
         # Boot the machine if required
-        if MachineController is not None and args.boot:
+        if MachineController is not None and arguments.boot:
             update("Job {}: Booting...", t.yellow, job.id)
             mc = MachineController(job.hostname)
             mc.boot(job.width, job.height)
 
         update("Job {}: Ready!", t.green, job.id)
 
         # Either run the user's application or just print the details.
-        if not args.command:
+        if not arguments.command:
             print_info(job.machine_name, job.connections,
                        job.width, job.height, ip_file_filename)
             return 0
-        return run_command(args.command, job.id, job.machine_name,
+        return run_command(arguments.command, job.id, job.machine_name,
                            job.connections, job.width, job.height,
                            ip_file_filename)
     finally:
         # Destroy job and disconnect client
-        if args.no_destroy:
+        if arguments.no_destroy:
             job.close()
         else:
             job.destroy(reason)
 
 
+def _minzero(value):
+    return value if value >= 0.0 else None
+
+
 def main(argv=None):
-    global args, t
-    parser, args = parse_argv(argv)
+    global arguments, t
+    parser, arguments = parse_argv(argv)
     t = Terminal(stream=sys.stderr)
 
     # Fail if no owner is defined (unless resuming)
-    if not args.owner and args.resume is None:
+    if not arguments.owner and arguments.resume is None:
         parser.error(
             "--owner must be specified (typically your email address)")
 
     # Fail if server not specified
-    if args.hostname is None:
+    if arguments.hostname is None:
         parser.error("--hostname of spalloc server must be specified")
 
     # Set universal job arguments
     job_kwargs = {
-        "hostname": args.hostname,
-        "port": args.port,
-        "reconnect_delay":
-            args.reconnect_delay if args.reconnect_delay >= 0.0 else None,
-        "timeout": args.timeout if args.timeout >= 0.0 else None,
+        "hostname": arguments.hostname,
+        "port": arguments.port,
+        "reconnect_delay": _minzero(arguments.reconnect_delay),
+        "timeout": _minzero(arguments.timeout),
     }
 
-    if args.resume:
+    if arguments.resume:
         job_args = []
         job_kwargs.update({
-            "resume_job_id": args.resume,
+            "resume_job_id": arguments.resume,
         })
     else:
         # Make sure 'what' takes the right form
-        if len(args.what) not in (0, 1, 2, 3):
+        if len(arguments.what) not in (0, 1, 2, 3):
             parser.error(
                 "expected either no arguments, one argument, NUM, two "
                 "arguments, WIDTH HEIGHT, or three arguments, X Y Z")
 
         # Unpack arguments for the job and server
-        job_args = args.what
+        job_args = arguments.what
         job_kwargs.update({
-            "owner": args.owner,
-            "keepalive": args.keepalive if args.keepalive >= 0.0 else None,
-            "machine": args.machine,
-            "tags": args.tags if args.machine is None else None,
-            "min_ratio": args.min_ratio,
-            "max_dead_boards":
-                args.max_dead_boards if args.max_dead_boards >= 0.0 else None,
-            "max_dead_links":
-                args.max_dead_links if args.max_dead_links >= 0.0 else None,
-            "require_torus": args.require_torus,
+            "owner": arguments.owner,
+            "keepalive": _minzero(arguments.keepalive),
+            "machine": arguments.machine,
+            "tags": arguments.tags if arguments.machine is None else None,
+            "min_ratio": arguments.min_ratio,
+            "max_dead_boards": _minzero(arguments.max_dead_boards),
+            "max_dead_links": _minzero(arguments.max_dead_links),
+            "require_torus": arguments.require_torus,
         })
 
     # Set debug level
-    if args.debug:
+    if arguments.debug:
         logging.basicConfig(level=logging.DEBUG)
 
     # Create temporary file in which to write CSV of all board IPs
     _, ip_file_filename = tempfile.mkstemp(".csv", "spinnaker_ips_")
 
     try:
         return run_job(job_args, job_kwargs, ip_file_filename)
```

### Comparing `spalloc-2.0.0/spalloc/scripts/job.py` & `spalloc-2.0.1/spalloc/scripts/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,29 +71,30 @@
 .. warning::
 
     That this "super power" should be used carefully since the user may not be
     notified that their job was destroyed and the first sign of this will be
     their boards being powered down and re-partitioned ready for another user.
 """
 import argparse
-try:
-    from collections.abc import OrderedDict
-except ImportError:
-    from collections import OrderedDict
+from collections import OrderedDict
 import datetime
 import sys
 from pytz import utc
 from tzlocal import get_localzone
 from six import iteritems
 from spalloc import __version__, JobState
 from spalloc.term import (
     Terminal, render_definitions, render_boards, DEFAULT_BOARD_EDGES)
 from .support import Terminate, Script
 
 
+def _state_name(mapping):
+    return JobState(mapping["state"]).name  # pylint: disable=no-member
+
+
 def show_job_info(t, client, timeout, job_id):
     """ Print a human-readable overview of a Job's attributes.
 
     Parameters
     ----------
     t : :py:class:`.Terminal`
         An output styling object for stdout.
@@ -115,24 +116,24 @@
     info = OrderedDict()
     info["Job ID"] = job_id
 
     if not job:
         # Job no longer exists, just print basic info
         job = client.get_job_state(job_id, timeout=timeout)
 
-        info["State"] = JobState(job["state"]).name
+        info["State"] = _state_name(job)
         if job["reason"] is not None:
             info["Reason"] = job["reason"]
     else:
         # Job is enqueued, show all info
         machine_info = client.get_job_machine_info(job_id, timeout=timeout)
         job = job[0]
 
         info["Owner"] = job["owner"]
-        info["State"] = JobState(job["state"]).name
+        info["State"] = _state_name(job)
         if job["start_time"] is not None:
             utc_timestamp = datetime.datetime.fromtimestamp(
                 job["start_time"], utc)
             local_timestamp = utc_timestamp.astimezone(get_localzone())
             info["Start time"] = local_timestamp.strftime('%d/%m/%Y %H:%M:%S')
         info["Keepalive"] = job["keepalive"]
         if "keepalivehost" in job and job["keepalivehost"] is not None:
@@ -246,16 +247,15 @@
             except KeyboardInterrupt:
                 # If interrupted, quietly return an error state
                 raise Terminate(7)
         else:
             # In an unknown state, perhaps the job was queued etc.
             raise Terminate(8, "Error: Cannot power {} job {} in state {}",
                             "on" if power else "off",
-                            job_id,
-                            JobState(state["state"]).name)
+                            job_id, _state_name(state))
 
 
 def list_ips(client, timeout, job_id):
     """ Print a CSV of board hostnames for all boards allocated to a job.
 
     Parameters
     ----------
```

### Comparing `spalloc-2.0.0/spalloc/scripts/machine.py` & `spalloc-2.0.1/spalloc/scripts/machine.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,15 @@
 Adding the ``--detailed`` option displays additional information about jobs
 running on a machine.
 
 If the ``--watch`` option is given, the information displayed is updated in
 real-time.
 """
 import argparse
-try:
-    from collections.abc import defaultdict, OrderedDict
-except ImportError:
-    from collections import defaultdict, OrderedDict
+from collections import defaultdict, OrderedDict
 import sys
 from six import next  # pylint: disable=redefined-builtin
 from spalloc import __version__
 from spalloc.term import (
     Terminal, render_table, render_definitions, render_boards, render_cells,
     DEFAULT_BOARD_EDGES)
 from .support import Terminate, Script
```

### Comparing `spalloc-2.0.0/spalloc/scripts/ps.py` & `spalloc-2.0.1/spalloc/scripts/ps.py`

 * *Files identical despite different names*

### Comparing `spalloc-2.0.0/spalloc/scripts/support.py` & `spalloc-2.0.1/spalloc/scripts/support.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,16 +20,19 @@
 
 # The acceptable range of server version numbers
 VERSION_RANGE_START = (0, 1, 0)
 VERSION_RANGE_STOP = (2, 0, 0)
 
 
 class Terminate(Exception):
-    def __init__(self, code, message=None, *args):
+    def __init__(self, code, *args):
+        super(Terminate, self).__init__()
         self._code = code
+        args = list(args)
+        message = args.pop(0) if args else None
         if message is None:
             self._msg = None
         elif args:
             self._msg = message.format(*args)
         else:
             self._msg = message
 
@@ -49,14 +52,15 @@
 class Script(object):
     def __init__(self):
         self.client_factory = ProtocolClient
 
     def get_parser(self, cfg):
         """ Return a set-up instance of :py:class:`argparse.ArgumentParser`
         """
+        raise NotImplementedError
 
     def verify_arguments(self, args):
         """ Check the arguments for sanity and do any second-stage parsing\
             required.
         """
 
     def body(self, client, args):
```

### Comparing `spalloc-2.0.0/spalloc/scripts/where_is.py` & `spalloc-2.0.1/spalloc/scripts/where_is.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,18 +63,15 @@
 
 To query by chip coordinate of chips allocated to a job::
 
     spalloc-where-is --job-chip JOB_ID X Y
 """
 import sys
 import argparse
-try:
-    from collections.abc import OrderedDict
-except ImportError:
-    from collections import OrderedDict
+from collections import OrderedDict
 from spalloc import __version__
 from spalloc.term import render_definitions
 from .support import Terminate, Script
 
 
 class WhereIsScript(Script):
     def get_parser(self, cfg):  # @UnusedVariable
```

### Comparing `spalloc-2.0.0/spalloc/scripts/__init__.py` & `spalloc-2.0.1/spalloc/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `spalloc-2.0.0/spalloc/states.py` & `spalloc-2.0.1/spalloc/states.py`

 * *Files identical despite different names*

### Comparing `spalloc-2.0.0/spalloc/term.py` & `spalloc-2.0.1/spalloc/term.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,18 +15,15 @@
 
 """ Utilities for generating ASCII/ANSI terminal graphics.
 """
 
 import os
 import sys
 from itertools import chain
-try:
-    from collections.abc import defaultdict
-except ImportError:
-    from collections import defaultdict
+from collections import defaultdict
 from enum import IntEnum
 from functools import partial
 from six import iteritems, string_types
 
 
 class ANSIDisplayAttributes(IntEnum):
     """ Code numbers of ANSI display attributes for use with `ESC[...m`\
@@ -286,15 +283,15 @@
     return "\n".join("{:>{}s}{}{}".format(
         key, col_width, seperator, str(value).replace(
             "\n", "\n{}".format(" "*(col_width + len(seperator)))))
         for key, value in iteritems(definitions))
 
 
 def _board_to_cartesian(x, y, z):
-    """ Translate from logical board coordinates (x, y, z) into Cartesian\
+    r""" Translate from logical board coordinates (x, y, z) into Cartesian
         coordinates for printing hexagons.
 
     Example coordinates::
 
          ___     ___
         /-15\___/1 5\___
         \___/0 4\___/3 4\
```

### Comparing `spalloc-2.0.0/spalloc/_keepalive_process.py` & `spalloc-2.0.1/spalloc/_keepalive_process.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,32 +76,35 @@
                 if not stop_event.wait(reconnect_delay):
                     try:
                         client.connect(timeout)
                     except (IOError, OSError):
                         client.close()
 
 
-if __name__ == "__main__":
+def _run(argv):
     print("KEEPALIVE")
     sys.stdout.flush()
-    if len(sys.argv) != 7:
-        sys.stderr.write(
-            "wrong # args: should be '" + sys.argv[0] + " hostname port "
-            "job_id keepalive_delay comms_timeout reconnect_delay'\n")
-        sys.exit(1)
-    hostname = sys.argv[1]
-    port = int(sys.argv[2])
-    job_id = int(sys.argv[3])
-    keepalive = float(sys.argv[4])
-    timeout = float(sys.argv[5])
-    reconnect_delay = float(sys.argv[6])
+    hostname = argv[1]
+    port = int(argv[2])
+    job_id = int(argv[3])
+    keepalive = float(argv[4])
+    timeout = float(argv[5])
+    reconnect_delay = float(argv[6])
 
     # Set things up so that we can detect when to stop
     stop_event = threading.Event()
-    stdin_watcher_thread = threading.Thread(
-        target=wait_for_exit, args=(stop_event,))
-    stdin_watcher_thread.daemon = True
-    stdin_watcher_thread.start()
+    stdin_watcher = threading.Thread(target=wait_for_exit, args=(stop_event,))
+    stdin_watcher.daemon = True
+    stdin_watcher.start()
 
     # Start keeping the job alive
     keep_job_alive(hostname, port, job_id, keepalive, timeout,
                    reconnect_delay, stop_event)
+
+
+if __name__ == "__main__":
+    if len(sys.argv) != 7:
+        sys.stderr.write(
+            "wrong # args: should be '" + sys.argv[0] + " hostname port "
+            "job_id keepalive_delay comms_timeout reconnect_delay'\n")
+        sys.exit(1)
+    _run(sys.argv)
```

### Comparing `spalloc-2.0.0/spalloc/_utils.py` & `spalloc-2.0.1/spalloc/_utils.py`

 * *Files identical despite different names*

### Comparing `spalloc-2.0.0/spalloc/_version.py` & `spalloc-2.0.1/spalloc/_version.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,12 +9,12 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-__version__ = "2.0.0"
-__version_month__ = "August"
+__version__ = "2.0.1"
+__version_month__ = "November"
 __version_year__ = "2019"
-__version_day__ = "09"
+__version_day__ = "15"
 __version_name__ = "Liveware Problem"
```

### Comparing `spalloc-2.0.0/spalloc/__init__.py` & `spalloc-2.0.1/spalloc/__init__.py`

 * *Files identical despite different names*

### Comparing `spalloc-2.0.0/spalloc.egg-info/PKG-INFO` & `spalloc-2.0.1/spalloc.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: spalloc
-Version: 2.0.0
+Version: 2.0.1
 Summary: A client for the spalloc_server SpiNNaker machine partitioning and allocation system.
 Home-page: https://github.com/SpiNNakerManchester/spalloc
 Author: Jonathan Heathcote
 Maintainer: SpiNNakerTeam
 Maintainer-email: spinnakerusers@googlegroups.com
 License: GPLv2
 Description: UNKNOWN
@@ -14,13 +14,11 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `spalloc-2.0.0/spalloc.egg-info/SOURCES.txt` & `spalloc-2.0.1/spalloc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spalloc-2.0.0/tests/common.py` & `spalloc-2.0.1/tests/common.py`

 * *Files identical despite different names*

### Comparing `spalloc-2.0.0/tests/conftest.py` & `spalloc-2.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `spalloc-2.0.0/tests/test_config.py` & `spalloc-2.0.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `spalloc-2.0.0/tests/test_job.py` & `spalloc-2.0.1/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `spalloc-2.0.0/tests/test_protocol_client.py` & `spalloc-2.0.1/tests/test_protocol_client.py`

 * *Files identical despite different names*

### Comparing `spalloc-2.0.0/tests/test_term.py` & `spalloc-2.0.1/tests/test_term.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-try:
-    from collections.abc import OrderedDict
-except ImportError:
-    from collections import OrderedDict
+from collections import OrderedDict
 import pytest
 from spalloc.term import (
     Terminal, render_table, render_definitions, render_boards, render_cells,
     DEFAULT_BOARD_EDGES)
 
 
 @pytest.mark.parametrize("force", [True, False])
```

### Comparing `spalloc-2.0.0/tests/__init__.py` & `spalloc-2.0.1/tests/__init__.py`

 * *Files identical despite different names*

