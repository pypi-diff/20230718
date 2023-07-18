# Comparing `tmp/gocept.logging-0.8.1.tar.gz` & `tmp/gocept.logging-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gocept.logging-0.8.1.tar", last modified: Mon Jan  9 14:40:25 2017, max compression
+gzip compressed data, was "gocept.logging-1.0.tar", last modified: Tue Jul 18 05:43:26 2023, max compression
```

## Comparing `gocept.logging-0.8.1.tar` & `gocept.logging-1.0.tar`

### file list

```diff
@@ -1,38 +1,34 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2017-01-09 14:40:25.000000 gocept.logging-0.8.1/
--rw-r--r--   0 mac        (501) staff       (20)      184 2017-01-09 14:40:25.000000 gocept.logging-0.8.1/.coveragerc
--rw-r--r--   0 mac        (501) staff       (20)      108 2017-01-09 14:40:25.000000 gocept.logging-0.8.1/.hgignore
--rw-r--r--   0 mac        (501) staff       (20)      360 2017-01-09 14:40:25.000000 gocept.logging-0.8.1/.hgtags
--rw-r--r--   0 mac        (501) staff       (20)     1087 2017-01-09 14:40:25.000000 gocept.logging-0.8.1/CHANGES.rst
--rw-r--r--   0 mac        (501) staff       (20)      448 2017-01-09 14:40:25.000000 gocept.logging-0.8.1/COPYRIGHT.rst
--rw-r--r--   0 mac        (501) staff       (20)      408 2017-01-09 14:40:25.000000 gocept.logging-0.8.1/HACKING.rst
--rw-r--r--   0 mac        (501) staff       (20)     2071 2017-01-09 14:40:25.000000 gocept.logging-0.8.1/LICENSE.rst
--rw-r--r--   0 mac        (501) staff       (20)    11809 2017-01-09 14:40:25.000000 gocept.logging-0.8.1/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)        0 2017-01-09 14:40:25.000000 gocept.logging-0.8.1/pytest.ini
--rw-r--r--   0 mac        (501) staff       (20)     6927 2017-01-09 14:40:25.000000 gocept.logging-0.8.1/README.rst
--rw-r--r--   0 mac        (501) staff       (20)       59 2017-01-09 14:40:25.000000 gocept.logging-0.8.1/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)     1566 2017-01-09 14:40:25.000000 gocept.logging-0.8.1/setup.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2017-01-09 14:40:25.000000 gocept.logging-0.8.1/src/
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2017-01-09 14:40:25.000000 gocept.logging-0.8.1/src/gocept/
--rw-r--r--   0 mac        (501) staff       (20)       56 2017-01-09 14:40:25.000000 gocept.logging-0.8.1/src/gocept/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2017-01-09 14:40:25.000000 gocept.logging-0.8.1/src/gocept/logging/
--rw-r--r--   0 mac        (501) staff       (20)      211 2017-01-09 14:40:25.000000 gocept.logging-0.8.1/src/gocept/logging/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      327 2017-01-09 14:40:25.000000 gocept.logging-0.8.1/src/gocept/logging/adapter.py
--rw-r--r--   0 mac        (501) staff       (20)     1168 2017-01-09 14:40:25.000000 gocept.logging-0.8.1/src/gocept/logging/argumentparser.py
--rw-r--r--   0 mac        (501) staff       (20)     1372 2017-01-09 14:40:25.000000 gocept.logging-0.8.1/src/gocept/logging/formatter.py
--rw-r--r--   0 mac        (501) staff       (20)      653 2017-01-09 14:40:25.000000 gocept.logging-0.8.1/src/gocept/logging/testing.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2017-01-09 14:40:25.000000 gocept.logging-0.8.1/src/gocept/logging/tests/
--rw-r--r--   0 mac        (501) staff       (20)        0 2017-01-09 14:40:25.000000 gocept.logging-0.8.1/src/gocept/logging/tests/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     1102 2017-01-09 14:40:25.000000 gocept.logging-0.8.1/src/gocept/logging/tests/test_adapter.py
--rw-r--r--   0 mac        (501) staff       (20)     3397 2017-01-09 14:40:25.000000 gocept.logging-0.8.1/src/gocept/logging/tests/test_argumentparser.py
--rw-r--r--   0 mac        (501) staff       (20)     1897 2017-01-09 14:40:25.000000 gocept.logging-0.8.1/src/gocept/logging/tests/test_formatter.py
--rw-r--r--   0 mac        (501) staff       (20)      641 2017-01-09 14:40:25.000000 gocept.logging-0.8.1/src/gocept/logging/tests/test_testing.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2017-01-09 14:40:25.000000 gocept.logging-0.8.1/src/gocept.logging.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)        1 2017-01-09 14:40:25.000000 gocept.logging-0.8.1/src/gocept.logging.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       20 2017-01-09 14:40:25.000000 gocept.logging-0.8.1/src/gocept.logging.egg-info/entry_points.txt
--rw-r--r--   0 mac        (501) staff       (20)        7 2017-01-09 14:40:25.000000 gocept.logging-0.8.1/src/gocept.logging.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2017-01-09 14:40:25.000000 gocept.logging-0.8.1/src/gocept.logging.egg-info/not-zip-safe
--rw-r--r--   0 mac        (501) staff       (20)    11809 2017-01-09 14:40:25.000000 gocept.logging-0.8.1/src/gocept.logging.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)       24 2017-01-09 14:40:25.000000 gocept.logging-0.8.1/src/gocept.logging.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)      857 2017-01-09 14:40:25.000000 gocept.logging-0.8.1/src/gocept.logging.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        7 2017-01-09 14:40:25.000000 gocept.logging-0.8.1/src/gocept.logging.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)      358 2017-01-09 14:40:25.000000 gocept.logging-0.8.1/tox.ini
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-07-18 05:43:26.309630 gocept.logging-1.0/
+-rw-r--r--   0 mac        (513) staff       (20)      184 2023-07-18 05:43:25.000000 gocept.logging-1.0/.coveragerc
+-rw-r--r--   0 mac        (513) staff       (20)     1039 2023-07-18 05:43:25.000000 gocept.logging-1.0/.pre-commit-config.yaml
+-rw-r--r--   0 mac        (513) staff       (20)     2070 2023-07-18 05:43:25.000000 gocept.logging-1.0/LICENSE.txt
+-rw-r--r--   0 mac        (513) staff       (20)       70 2023-07-18 05:43:25.000000 gocept.logging-1.0/MANIFEST.in
+-rw-r--r--   0 mac        (513) staff       (20)     9809 2023-07-18 05:43:26.309766 gocept.logging-1.0/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)     7231 2023-07-18 05:43:25.000000 gocept.logging-1.0/README.rst
+-rw-r--r--   0 mac        (513) staff       (20)       69 2023-07-18 05:43:25.000000 gocept.logging-1.0/pytest.ini
+-rw-r--r--   0 mac        (513) staff       (20)      213 2023-07-18 05:43:26.310269 gocept.logging-1.0/setup.cfg
+-rw-r--r--   0 mac        (513) staff       (20)     1651 2023-07-18 05:43:25.000000 gocept.logging-1.0/setup.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-07-18 05:43:26.300342 gocept.logging-1.0/src/
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-07-18 05:43:26.304183 gocept.logging-1.0/src/gocept/
+-rw-r--r--   0 mac        (513) staff       (20)       76 2023-07-18 05:43:25.000000 gocept.logging-1.0/src/gocept/__init__.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-07-18 05:43:26.307895 gocept.logging-1.0/src/gocept/logging/
+-rw-r--r--   0 mac        (513) staff       (20)      339 2023-07-18 05:43:25.000000 gocept.logging-1.0/src/gocept/logging/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)      369 2023-07-18 05:43:25.000000 gocept.logging-1.0/src/gocept/logging/adapter.py
+-rw-r--r--   0 mac        (513) staff       (20)     1128 2023-07-18 05:43:25.000000 gocept.logging-1.0/src/gocept/logging/argumentparser.py
+-rw-r--r--   0 mac        (513) staff       (20)     1299 2023-07-18 05:43:25.000000 gocept.logging-1.0/src/gocept/logging/formatter.py
+-rw-r--r--   0 mac        (513) staff       (20)      633 2023-07-18 05:43:25.000000 gocept.logging-1.0/src/gocept/logging/testing.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-07-18 05:43:26.309351 gocept.logging-1.0/src/gocept/logging/tests/
+-rw-r--r--   0 mac        (513) staff       (20)        0 2023-07-18 05:43:25.000000 gocept.logging-1.0/src/gocept/logging/tests/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)     1319 2023-07-18 05:43:25.000000 gocept.logging-1.0/src/gocept/logging/tests/test_adapter.py
+-rw-r--r--   0 mac        (513) staff       (20)     3411 2023-07-18 05:43:25.000000 gocept.logging-1.0/src/gocept/logging/tests/test_argumentparser.py
+-rw-r--r--   0 mac        (513) staff       (20)     1818 2023-07-18 05:43:25.000000 gocept.logging-1.0/src/gocept/logging/tests/test_formatter.py
+-rw-r--r--   0 mac        (513) staff       (20)      641 2023-07-18 05:43:25.000000 gocept.logging-1.0/src/gocept/logging/tests/test_testing.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-07-18 05:43:26.306354 gocept.logging-1.0/src/gocept.logging.egg-info/
+-rw-r--r--   0 mac        (513) staff       (20)     9809 2023-07-18 05:43:26.000000 gocept.logging-1.0/src/gocept.logging.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)      802 2023-07-18 05:43:26.000000 gocept.logging-1.0/src/gocept.logging.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-07-18 05:43:26.000000 gocept.logging-1.0/src/gocept.logging.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (513) staff       (20)        7 2023-07-18 05:43:26.000000 gocept.logging-1.0/src/gocept.logging.egg-info/namespace_packages.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-07-18 05:43:26.000000 gocept.logging-1.0/src/gocept.logging.egg-info/not-zip-safe
+-rw-r--r--   0 mac        (513) staff       (20)       24 2023-07-18 05:43:26.000000 gocept.logging-1.0/src/gocept.logging.egg-info/requires.txt
+-rw-r--r--   0 mac        (513) staff       (20)        7 2023-07-18 05:43:26.000000 gocept.logging-1.0/src/gocept.logging.egg-info/top_level.txt
+-rw-r--r--   0 mac        (513) staff       (20)      494 2023-07-18 05:43:25.000000 gocept.logging-1.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `gocept.logging-0.8.1/LICENSE.rst` & `gocept.logging-1.0/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -37,8 +37,7 @@
 EVENT SHALL THE COPYRIGHT HOLDERS BE LIABLE FOR ANY DIRECT, INDIRECT,
 INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
 LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR
 PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
```

### Comparing `gocept.logging-0.8.1/PKG-INFO` & `gocept.logging-1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,340 +1,357 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: gocept.logging
-Version: 0.8.1
+Version: 1.0
 Summary: Infrastructure for semi-structured log messages.
-Home-page: https://bitbucket.org/gocept/gocept.logging/
+Home-page: https://github.com/gocept/gocept.logging
 Author: gocept <mail@gocept.com>
 Author-email: mail@gocept.com
 License: ZPL 2.1
-Description: ==============
-        gocept.logging
-        ==============
-        
-        .. contents::
-           :depth: 2
-        
-        This package provides infrastructure for semi-structured log messages.
-        
-        This means appending easily parseable information after the free-text log
-        message to facilitate analysis of the logs later on. The ``logging`` module of
-        the Python standard library already has support for this, via the ``extra``
-        parameter. gocept.logging provides a ``Formatter`` that extracts these
-        ``extra`` values, formats them as ``key=value`` pairs and appends them to the
-        message::
-        
-            >>> import gocept.logging
-            >>> import logging
-            >>> import sys
-        
-            >>> handler = logging.StreamHandler(sys.stdout)
-            >>> handler.setFormatter(gocept.logging.SyslogKeyValueFormatter())
-            >>> log = logging.getLogger('example')
-            >>> log.addHandler(handler)
-            >>> log.warning('Hello, world!', extra={'foo': 'bar'})
-            Aug 24 12:10:08 localhost example: Hello, world! foo=bar
-        
-        This package is tested to be compatible with Python version 2.7 and 3.3.
-        
-        
-        Advanced usage
-        ==============
-        
-        If you have ``extra`` values that you always want to pass to your log messages
-        (e.g things like the current user, session id, ...) you can wrap your logger
-        with an `LoggerAdapter`_ that prefills these values. gocept.logging provides
-        one that allows both stacking adapters and overriding the prefilled values::
-        
-            >>> from gocept.logging.adapter import StaticDefaults
-            >>> import logging
-        
-            >>> log = logging.getLogger('advanced')
-            >>> log = StaticDefaults(log, {'foo': 'bar', 'qux': 'baz'})
-            >>> log = StaticDefaults(log, {'blam': 'splat'})
-            >>> log.warning('Hello, world!', extra={'foo': 'override'})
-                # yields {'foo': 'override', 'qux': 'baz', 'blam': 'splat'}
-        
-        .. _`LoggerAdapter`: http://docs.python.org/2/library/logging.html#loggeradapter-objects
-        
-        
-        Testing support
-        ---------------
-        
-        To help inspecting the ``extra`` values, gocept.logging comes with a
-        specialized handler for testing::
-        
-            >>> import gocept.logging
-            >>> import logging
-        
-            >>> log = logging.getLogger('testing')
-            >>> handler = gocept.logging.TestingHandler()
-            >>> log.addHandler(handler)
-            >>> log.warning('Hello, world!', extra={'foo': 'bar'})
-            >>> handler.messages[0].extra['foo']
-            'bar'
-        
-        The TestingHandler records each log message as a namedtuple of type
-        ``gocept.logging.testing.LogMessage`` so you an easily access all parts of the
-        message.
-        
-        
-        Example configuration
-        =====================
-        
-        Creating semi-structured log messages is the first half of the issue, while
-        analysing them is the second half. We use `logstash`_ for that purpose.
-        
-        The recommended setup is::
-        
-            application -> syslogd on localhost -> logstash on central host (via UDP syslog input)
-        
-        For development you might want to leave out the middle man and configure the
-        application to send log messags via syslog protocol directly to logstash.
-        
-        
-        .. _`logstash`: http://logstash.net/
-        
-        
-        Setup with ini file
-        -------------------
-        
-        If you have a paste.ini for your application, you might use something like
-        this::
-        
-            [loggers]
-            keys = root
-        
-            [handlers]
-            keys = console, syslog
-        
-            [formatters]
-            keys = generic, keyvalue
-        
-            [logger_root]
-            level = INFO
-            handlers = console, syslog
-        
-            [handler_console]
-            class = StreamHandler
-            args = (sys.stderr,)
-            level = NOTSET
-            formatter = generic
-        
-            [formatter_generic]
-            format = %(asctime)s %(levelname)-5.5s %(name)s: %(message)s
-        
-            [handler_syslog]
-            class = logging.handlers.SysLogHandler
-            args = ()
-            formatter = keyvalue
-        
-            [formatter_keyvalue]
-            class = gocept.logging.SyslogKeyValueFormatter
-        
-        
-        Setup with ZConfig
-        ------------------
-        
-        If you have a Zope application, you might use something like this::
-        
-            <eventlog>
-              <logfile>
-                formatter zope.exceptions.log.Formatter
-                format %(asctime)s %(levelname)-5.5s %(name)s: %(message)s
-                path STDOUT
-              </logfile>
-              <syslog>
-                formatter gocept.logging.SyslogKeyValueFormatter
-              </syslog>
-            </eventlog>
-        
-        
-        syslogd configuration
-        ---------------------
-        
-        rsyslog::
-        
-            $EscapeControlCharactersOnReceive off
-            $MaxMessageSize 64k
-            user.* @localhost:5140
-        
-        The first two lines are to support tracebacks, which are multiline and might
-        take up some space. The last line tells rsyslogd to forward all messages of the
-        ``user`` facility (which is what stdlib ``logging`` uses by default) via syslog
-        UDP protocol to localhost port 5140 (where logstash might be listening).
-        
-        
-        logstash configuration
-        ----------------------
-        
-        ::
-        
-            input {
-                    tcp {
-                            host => "localhost"
-                            port => 5140
-                            type => syslog
-                    }
-                    udp {
-                            host => "localhost"
-                            port => 5140
-                            type => syslog
-                    }
-            }
-        
-            filter {
-                    grok {
-                            type => "syslog"
-                            pattern => [ "(?m)<%{POSINT:syslog_pri}>%{SYSLOGTIMESTAMP:syslog_timestamp} %{SYSLOGHOST:syslog_hostname} %{DATA:syslog_program}(?:\[%{POSINT:syslog_pid}\])?: %{GREEDYDATA:syslog_message}" ]
-                    }
-                    syslog_pri {
-                            type => "syslog"
-                    }
-                    date {
-                            type => "syslog"
-                            match => [ "syslog_timestamp", "MMM  d HH:mm:ss", "MMM dd HH:mm:ss" ]
-                    }
-                    mutate {
-                            type => "syslog"
-                            exclude_tags => "_grokparsefailure"
-                            replace => [ "@source_host", "%{syslog_hostname}" ]
-                            replace => [ "@message", "%{syslog_program}: %{syslog_message}" ]
-                    }
-                    mutate {
-                            type => "syslog"
-                            remove => [ "syslog_hostname", "syslog_timestamp" ]
-                    }
-                    kv {
-                            exclude_tags => "_grokparsefailure"
-                            type => "syslog"
-                    }
-            }
-        
-            output {
-                    elasticsearch { embedded => true }
-            }
-        
-        
-        Additional features
-        ===================
-        
-        ArgumentParser
-        --------------
-        
-        The provided ``gocept.logging.ArgumentParser`` provides you with the ability to
-        set a ``logging`` level in you runscripts.::
-        
-            from gocept.logging import ArgumentParser
-            parser = ArgumentParser()
-            # Optionally set a custom log format, defaults to ``logging.BASIC_FORMAT``
-            parser.LOG_FORMAT = 'LOG:%(message)s'
-            # add your arguments with parser.add_argument() here
-            options = parser.parse_args()
-        
-        Use ``your_run_script --help`` to see a help message about the arguments you
-        can pass to set logging level.
-        
-        
-        Known bugs
-        ==========
-        
-        If you log messages as unicode, e.g. ``log.info(u'foo')``, the SyslogHandler
-        will (incorrectly) prepend a byte-order mark, which confuses the logstash
-        parser, resulting in "_grokparsefailure". This is a `known bug`_ in the Python
-        standard library that has been fixed in Python-2.7.4.
-        
-        .. _`known bug`: http://bugs.python.org/issue14452
-        
-        
-        =========================
-        Developing gocept.logging
-        =========================
-        
-        :Author:
-            `gocept <http://gocept.com/>`_ <mail@gocept.com>
-        
-        :PyPI page:
-            http://pypi.python.org/pypi/gocept.logging/
-        
-        :Issues:
-            `report by e-mail <mail@gocept.com>`_
-        
-        :Source code:
-            https://bitbucket.org/gocept/gocept.logging/
-        
-        :Current change log:
-            https://bitbucket.org/gocept/gocept.logging/raw/tip/CHANGES.txt
-        
-        
-        =============================
-        Change log for gocept.logging
-        =============================
-        
-        0.8.1 (2017-01-09)
-        ==================
-        
-        - Fix `setup.py` to use relative paths.
-        
-        
-        0.8 (2016-03-17)
-        ================
-        
-        - Declare compatibility with PyPy and PyPy3.
-        
-        
-        0.7 (2015-09-29)
-        ================
-        
-        - Declare Python 3.5 compatibility.
-        
-        
-        0.6 (2015-09-17)
-        ================
-        
-        - Declare Python 3.4 compatibility.
-        
-        - ``ArgumentParser.parse_args()`` now stores the computed log level on the
-          ``log_level`` attribute of the return value.
-        
-        0.5 (2014-02-07)
-        ================
-        
-        - Allow to change log format for the ``ArgumentParser``
-        
-        
-        0.4 (2013-09-24)
-        ================
-        
-        - Handle non-string log messages properly.
-        
-        
-        0.3 (2013-09-04)
-        ================
-        
-        - Added sepcialized ``argparse.ArgumentParser`` which enables user to set the
-          ``logging`` level by default..
-        
-        
-        0.2 (2013-08-24)
-        ================
-        
-        - Add timestamp and hostname to syslog messages,
-          this allows plugging SyslogKeyValueFormatter directly into logstash
-          without an intermediary syslogd.
-        
-        
-        0.1 (2013-08-16)
-        ================
-        
-        - initial release
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.7
+Provides-Extra: test
+License-File: LICENSE.txt
+
+==============
+gocept.logging
+==============
+
+.. image:: https://github.com/gocept/gocept.logging/workflows/tests/badge.svg
+    :target: https://github.com/gocept/gocept.logging/actions?query=workflow%3Atests
+.. image:: https://coveralls.io/repos/github/gocept/gocept.logging/badge.svg
+    :target: https://coveralls.io/github/gocept/gocept.logging
+
+.. contents::
+   :depth: 2
+
+This package provides infrastructure for semi-structured log messages.
+
+This means appending easily parseable information after the free-text log
+message to facilitate analysis of the logs later on. The ``logging`` module of
+the Python standard library already has support for this, via the ``extra``
+parameter. gocept.logging provides a ``Formatter`` that extracts these
+``extra`` values, formats them as ``key=value`` pairs and appends them to the
+message::
+
+    >>> import gocept.logging
+    >>> import logging
+    >>> import sys
+
+    >>> handler = logging.StreamHandler(sys.stdout)
+    >>> handler.setFormatter(gocept.logging.SyslogKeyValueFormatter())
+    >>> log = logging.getLogger('example')
+    >>> log.addHandler(handler)
+    >>> log.warning('Hello, world!', extra={'foo': 'bar'})
+    Aug 24 12:10:08 localhost example: Hello, world! foo=bar
+
+This package is tested to be compatible with Python version 2.7 and 3.3.
+
+
+Advanced usage
+==============
+
+If you have ``extra`` values that you always want to pass to your log messages
+(e.g things like the current user, session id, ...) you can wrap your logger
+with an `LoggerAdapter`_ that prefills these values. gocept.logging provides
+one that allows both stacking adapters and overriding the prefilled values::
+
+    >>> from gocept.logging.adapter import StaticDefaults
+    >>> import logging
+
+    >>> log = logging.getLogger('advanced')
+    >>> log = StaticDefaults(log, {'foo': 'bar', 'qux': 'baz'})
+    >>> log = StaticDefaults(log, {'blam': 'splat'})
+    >>> log.warning('Hello, world!', extra={'foo': 'override'})
+        # yields {'foo': 'override', 'qux': 'baz', 'blam': 'splat'}
+
+.. _`LoggerAdapter`: http://docs.python.org/2/library/logging.html#loggeradapter-objects
+
+
+Testing support
+---------------
+
+To help inspecting the ``extra`` values, gocept.logging comes with a
+specialized handler for testing::
+
+    >>> import gocept.logging
+    >>> import logging
+
+    >>> log = logging.getLogger('testing')
+    >>> handler = gocept.logging.TestingHandler()
+    >>> log.addHandler(handler)
+    >>> log.warning('Hello, world!', extra={'foo': 'bar'})
+    >>> handler.messages[0].extra['foo']
+    'bar'
+
+The TestingHandler records each log message as a namedtuple of type
+``gocept.logging.testing.LogMessage`` so you an easily access all parts of the
+message.
+
+
+Example configuration
+=====================
+
+Creating semi-structured log messages is the first half of the issue, while
+analysing them is the second half. We use `logstash`_ for that purpose.
+
+The recommended setup is::
+
+    application -> syslogd on localhost -> logstash on central host (via UDP syslog input)
+
+For development you might want to leave out the middle man and configure the
+application to send log messags via syslog protocol directly to logstash.
+
+
+.. _`logstash`: http://logstash.net/
+
+
+Setup with ini file
+-------------------
+
+If you have a paste.ini for your application, you might use something like
+this::
+
+    [loggers]
+    keys = root
+
+    [handlers]
+    keys = console, syslog
+
+    [formatters]
+    keys = generic, keyvalue
+
+    [logger_root]
+    level = INFO
+    handlers = console, syslog
+
+    [handler_console]
+    class = StreamHandler
+    args = (sys.stderr,)
+    level = NOTSET
+    formatter = generic
+
+    [formatter_generic]
+    format = %(asctime)s %(levelname)-5.5s %(name)s: %(message)s
+
+    [handler_syslog]
+    class = logging.handlers.SysLogHandler
+    args = ()
+    formatter = keyvalue
+
+    [formatter_keyvalue]
+    class = gocept.logging.SyslogKeyValueFormatter
+
+
+Setup with ZConfig
+------------------
+
+If you have a Zope application, you might use something like this::
+
+    <eventlog>
+      <logfile>
+        formatter zope.exceptions.log.Formatter
+        format %(asctime)s %(levelname)-5.5s %(name)s: %(message)s
+        path STDOUT
+      </logfile>
+      <syslog>
+        formatter gocept.logging.SyslogKeyValueFormatter
+      </syslog>
+    </eventlog>
+
+
+syslogd configuration
+---------------------
+
+rsyslog::
+
+    $EscapeControlCharactersOnReceive off
+    $MaxMessageSize 64k
+    user.* @localhost:5140
+
+The first two lines are to support tracebacks, which are multiline and might
+take up some space. The last line tells rsyslogd to forward all messages of the
+``user`` facility (which is what stdlib ``logging`` uses by default) via syslog
+UDP protocol to localhost port 5140 (where logstash might be listening).
+
+
+logstash configuration
+----------------------
+
+::
+
+    input {
+            tcp {
+                    host => "localhost"
+                    port => 5140
+                    type => syslog
+            }
+            udp {
+                    host => "localhost"
+                    port => 5140
+                    type => syslog
+            }
+    }
+
+    filter {
+            grok {
+                    type => "syslog"
+                    pattern => [ "(?m)<%{POSINT:syslog_pri}>%{SYSLOGTIMESTAMP:syslog_timestamp} %{SYSLOGHOST:syslog_hostname} %{DATA:syslog_program}(?:\[%{POSINT:syslog_pid}\])?: %{GREEDYDATA:syslog_message}" ]
+            }
+            syslog_pri {
+                    type => "syslog"
+            }
+            date {
+                    type => "syslog"
+                    match => [ "syslog_timestamp", "MMM  d HH:mm:ss", "MMM dd HH:mm:ss" ]
+            }
+            mutate {
+                    type => "syslog"
+                    exclude_tags => "_grokparsefailure"
+                    replace => [ "@source_host", "%{syslog_hostname}" ]
+                    replace => [ "@message", "%{syslog_program}: %{syslog_message}" ]
+            }
+            mutate {
+                    type => "syslog"
+                    remove => [ "syslog_hostname", "syslog_timestamp" ]
+            }
+            kv {
+                    exclude_tags => "_grokparsefailure"
+                    type => "syslog"
+            }
+    }
+
+    output {
+            elasticsearch { embedded => true }
+    }
+
+
+Additional features
+===================
+
+ArgumentParser
+--------------
+
+The provided ``gocept.logging.ArgumentParser`` provides you with the ability to
+set a ``logging`` level in you runscripts.::
+
+    from gocept.logging import ArgumentParser
+    parser = ArgumentParser()
+    # Optionally set a custom log format, defaults to ``logging.BASIC_FORMAT``
+    parser.LOG_FORMAT = 'LOG:%(message)s'
+    # add your arguments with parser.add_argument() here
+    options = parser.parse_args()
+
+Use ``your_run_script --help`` to see a help message about the arguments you
+can pass to set logging level.
+
+
+Known bugs
+==========
+
+If you log messages as unicode, e.g. ``log.info(u'foo')``, the SyslogHandler
+will (incorrectly) prepend a byte-order mark, which confuses the logstash
+parser, resulting in "_grokparsefailure". This is a `known bug`_ in the Python
+standard library that has been fixed in Python-2.7.4.
+
+.. _`known bug`: http://bugs.python.org/issue14452
+
+
+=========================
+Developing gocept.logging
+=========================
+
+:Author:
+    `gocept <http://gocept.com/>`_ <mail@gocept.com>
+
+:PyPI page:
+    http://pypi.python.org/pypi/gocept.logging/
+
+:Issues:
+    `report by e-mail <mail@gocept.com>`_
+
+:Source code:
+    https://github.com/gocept/gocept.logging
+
+:Current change log:
+    https://raw.githubusercontent.com/gocept/gocept.logging/master/CHANGES.rst
+
+
+=============================
+Change log for gocept.logging
+=============================
+
+1.0 (2023-07-18)
+================
+
+- Drop support for Python 2.7, 3.3, 3.4, 3.5, 3.6.
+
+- Add support for Python 3.7, 3.8 3.9, 3.10, 3.11.
+
+- Add an alias ``.warn`` for ``.warning`` for ``StaticDefaults``. (#1)
+
+
+0.8.1 (2017-01-09)
+==================
+
+- Fix `setup.py` to use relative paths.
+
+
+0.8 (2016-03-17)
+================
+
+- Declare compatibility with PyPy and PyPy3.
+
+
+0.7 (2015-09-29)
+================
+
+- Declare Python 3.5 compatibility.
+
+
+0.6 (2015-09-17)
+================
+
+- Declare Python 3.4 compatibility.
+
+- ``ArgumentParser.parse_args()`` now stores the computed log level on the
+  ``log_level`` attribute of the return value.
+
+0.5 (2014-02-07)
+================
+
+- Allow to change log format for the ``ArgumentParser``
+
+
+0.4 (2013-09-24)
+================
+
+- Handle non-string log messages properly.
+
+
+0.3 (2013-09-04)
+================
+
+- Added sepcialized ``argparse.ArgumentParser`` which enables user to set the
+  ``logging`` level by default..
+
+
+0.2 (2013-08-24)
+================
+
+- Add timestamp and hostname to syslog messages,
+  this allows plugging SyslogKeyValueFormatter directly into logstash
+  without an intermediary syslogd.
+
+
+0.1 (2013-08-16)
+================
+
+- initial release
```

### Comparing `gocept.logging-0.8.1/README.rst` & `gocept.logging-1.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 ==============
 gocept.logging
 ==============
 
+.. image:: https://github.com/gocept/gocept.logging/workflows/tests/badge.svg
+    :target: https://github.com/gocept/gocept.logging/actions?query=workflow%3Atests
+.. image:: https://coveralls.io/repos/github/gocept/gocept.logging/badge.svg
+    :target: https://coveralls.io/github/gocept/gocept.logging
+
 .. contents::
    :depth: 2
 
 This package provides infrastructure for semi-structured log messages.
 
 This means appending easily parseable information after the free-text log
 message to facilitate analysis of the logs later on. The ``logging`` module of
```

### Comparing `gocept.logging-0.8.1/setup.py` & `gocept.logging-1.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # This should be only one line. If it must be multi-line, indent the second
 # line onwards to keep the PKG-INFO file format intact.
 """Infrastructure for semi-structured log messages.
 """
 
-from setuptools import setup, find_packages
-import glob
+from setuptools import find_packages
+from setuptools import setup
 
 
 setup(
     name='gocept.logging',
-    version='0.8.1',
-
+    version='1.0',
+    python_requires='>=3.7',
     install_requires=[
         'setuptools',
     ],
 
     extras_require={
         'test': [
             'mock',
@@ -26,36 +26,35 @@
             # 'binary-name = gocept.logging.module:function'
         ],
     },
 
     author='gocept <mail@gocept.com>',
     author_email='mail@gocept.com',
     license='ZPL 2.1',
-    url='https://bitbucket.org/gocept/gocept.logging/',
+    url='https://github.com/gocept/gocept.logging',
 
     keywords='',
-    classifiers="""\
-License :: OSI Approved :: Zope Public License
-Programming Language :: Python
-Programming Language :: Python :: 2
-Programming Language :: Python :: 2.7
-Programming Language :: Python :: 3
-Programming Language :: Python :: 3.3
-Programming Language :: Python :: 3.4
-Programming Language :: Python :: 3.5
-Programming Language :: Python :: Implementation :: CPython
-Programming Language :: Python :: Implementation :: PyPy
-"""[:-1].split('\n'),
+    classifiers=[
+        'License :: OSI Approved :: Zope Public License',
+        'Programming Language :: Python',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: Implementation :: CPython',
+        'Programming Language :: Python :: Implementation :: PyPy',
+    ],
     description=__doc__.strip(),
     long_description='\n\n'.join(open(name).read() for name in (
         'README.rst',
         'HACKING.rst',
         'CHANGES.rst',
     )),
 
     namespace_packages=['gocept'],
     packages=find_packages('src'),
     package_dir={'': 'src'},
     include_package_data=True,
-    data_files=[('', glob.glob('*.rst'))],
     zip_safe=False,
 )
```

### Comparing `gocept.logging-0.8.1/src/gocept/logging/argumentparser.py` & `gocept.logging-1.0/src/gocept/logging/argumentparser.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 
 
 class ArgumentParser(argparse.ArgumentParser):
 
     LOG_FORMAT = logging.BASIC_FORMAT
 
     def __init__(self, *args, **kw):
-        super(ArgumentParser, self).__init__(*args, **kw)
+        super().__init__(*args, **kw)
         self.add_argument('-q', '--quiet', action='count', default=0,
                           help='Log less info. (may be used up to twice.)')
         self.add_argument('-v', '--verbose', action='count', default=0,
                           help='Log more info. (may be used up to twice.)')
 
     def parse_args(self, *args, **kw):
-        options = super(ArgumentParser, self).parse_args(*args, **kw)
+        options = super().parse_args(*args, **kw)
 
         verbosity = options.verbose - options.quiet
         if verbosity <= -2:
             log_level = 'CRITICAL'
         elif verbosity == -1:
             log_level = 'ERROR'
         elif verbosity == 0:
```

### Comparing `gocept.logging-0.8.1/src/gocept/logging/formatter.py` & `gocept.logging-1.0/src/gocept/logging/formatter.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,38 +9,38 @@
 PREDEFINED_KEYS.add('asctime')
 PREDEFINED_KEYS.add('hostname')  # SyslogKeyValueFormatter
 
 
 class KeyValueFormatter(logging.Formatter):
 
     def format(self, record):
-        record.msg = '%s %s' % (record.msg, self.format_extra(record))
-        return super(KeyValueFormatter, self).format(record)
+        record.msg = '{} {}'.format(record.msg, self.format_extra(record))
+        return super().format(record)
 
     def format_extra(self, record):
         result = []
         for key, value in record.__dict__.items():
             if key in PREDEFINED_KEYS:
                 continue
-            result.append('%s=%s' % (key, self.quote(value)))
+            result.append('{}={}'.format(key, self.quote(value)))
         return ' '.join(result)
 
     SIMPLE_WORD = re.compile(r'^[a-zA-Z0-9_.+-]+$')
 
     def quote(self, value):
         value = str(value)
         if self.SIMPLE_WORD.match(value):
             return value
         return repr(value)
 
 
 class SyslogKeyValueFormatter(KeyValueFormatter):
 
     def __init__(self, fmt=None, datefmt=None):
-        super(SyslogKeyValueFormatter, self).__init__(
+        super().__init__(
             '%(asctime)s %(hostname)s %(name)s: %(message)s',
             '%b %-2d %H:%M:%S')
         self.hostname = socket.gethostname()
 
     def format(self, record):
         record.hostname = self.hostname
-        return super(SyslogKeyValueFormatter, self).format(record)
+        return super().format(record)
```

### Comparing `gocept.logging-0.8.1/src/gocept/logging/testing.py` & `gocept.logging-1.0/src/gocept/logging/testing.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 LogMessage = collections.namedtuple(
     'LogMessage', ['name', 'levelname', 'message', 'extra'])
 
 
 class TestingHandler(logging.Handler):
 
     def __init__(self, *args, **kw):
-        super(TestingHandler, self).__init__(*args, **kw)
+        super().__init__(*args, **kw)
         self.messages = []
 
     def emit(self, record):
         extra = {}
         for key, value in record.__dict__.items():
             if key in gocept.logging.formatter.PREDEFINED_KEYS:
                 continue
```

### Comparing `gocept.logging-0.8.1/src/gocept/logging/tests/test_adapter.py` & `gocept.logging-1.0/src/gocept/logging/tests/test_adapter.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,7 +27,12 @@
         self.assertEqual(
             {'foo': 'bar', 'qux': 'baz'}, self.handler.messages[0].extra)
 
     def test_logger_overrides_values(self):
         log = StaticDefaults(self.log, {'foo': 'bar'})
         log.warning('', extra={'foo': 'over'})
         self.assertEqual({'foo': 'over'}, self.handler.messages[0].extra)
+
+    def test_logger_uses_warn_alias(self):
+        log = StaticDefaults(self.log, {'foo': 'bar'})
+        log.warn('', extra={'foo': 'over'})
+        self.assertEqual({'foo': 'over'}, self.handler.messages[0].extra)
```

### Comparing `gocept.logging-0.8.1/src/gocept/logging/tests/test_argumentparser.py` & `gocept.logging-1.0/src/gocept/logging/tests/test_argumentparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+from unittest import mock
 import unittest
-import mock
 
 
 class ArgumentParserTests(unittest.TestCase):
     """Testing ..argumentparser.ArgumentParser."""
 
     def test_adds_quiet_and_verbose_arguments_per_default(self):
         from gocept.logging import ArgumentParser
```

### Comparing `gocept.logging-0.8.1/src/gocept/logging/tests/test_formatter.py` & `gocept.logging-1.0/src/gocept/logging/tests/test_formatter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-try:
-    from StringIO import StringIO
-except ImportError:
-    from io import StringIO
+from io import StringIO
 import gocept.logging
 import logging
 import unittest
 
 
 class KeyValueFormatter(unittest.TestCase):
 
@@ -45,12 +42,12 @@
 
     def test_single_quotes_are_quoted_with_double(self):
         self.log.warning('', extra={'foo': "bar'baz"})
         self.assertIn('foo="bar\'baz"', self.output)
 
     def test_objects_in_extra_are_serialized_to_string(self):
         self.log.warning('', extra={'foo': object()})
-        self.assertRegexpMatches(self.output, "foo='<object object at 0x.*>'")
+        self.assertRegex(self.output, "foo='<object object at 0x.*>'")
 
     def test_objects_in_message_are_serialized_to_string(self):
         self.log.warning(object())
-        self.assertRegexpMatches(self.output, "<object object at 0x.*>")
+        self.assertRegex(self.output, "<object object at 0x.*>")
```

### Comparing `gocept.logging-0.8.1/src/gocept/logging/tests/test_testing.py` & `gocept.logging-1.0/src/gocept/logging/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `gocept.logging-0.8.1/src/gocept.logging.egg-info/PKG-INFO` & `gocept.logging-1.0/src/gocept.logging.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,340 +1,357 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: gocept.logging
-Version: 0.8.1
+Version: 1.0
 Summary: Infrastructure for semi-structured log messages.
-Home-page: https://bitbucket.org/gocept/gocept.logging/
+Home-page: https://github.com/gocept/gocept.logging
 Author: gocept <mail@gocept.com>
 Author-email: mail@gocept.com
 License: ZPL 2.1
-Description: ==============
-        gocept.logging
-        ==============
-        
-        .. contents::
-           :depth: 2
-        
-        This package provides infrastructure for semi-structured log messages.
-        
-        This means appending easily parseable information after the free-text log
-        message to facilitate analysis of the logs later on. The ``logging`` module of
-        the Python standard library already has support for this, via the ``extra``
-        parameter. gocept.logging provides a ``Formatter`` that extracts these
-        ``extra`` values, formats them as ``key=value`` pairs and appends them to the
-        message::
-        
-            >>> import gocept.logging
-            >>> import logging
-            >>> import sys
-        
-            >>> handler = logging.StreamHandler(sys.stdout)
-            >>> handler.setFormatter(gocept.logging.SyslogKeyValueFormatter())
-            >>> log = logging.getLogger('example')
-            >>> log.addHandler(handler)
-            >>> log.warning('Hello, world!', extra={'foo': 'bar'})
-            Aug 24 12:10:08 localhost example: Hello, world! foo=bar
-        
-        This package is tested to be compatible with Python version 2.7 and 3.3.
-        
-        
-        Advanced usage
-        ==============
-        
-        If you have ``extra`` values that you always want to pass to your log messages
-        (e.g things like the current user, session id, ...) you can wrap your logger
-        with an `LoggerAdapter`_ that prefills these values. gocept.logging provides
-        one that allows both stacking adapters and overriding the prefilled values::
-        
-            >>> from gocept.logging.adapter import StaticDefaults
-            >>> import logging
-        
-            >>> log = logging.getLogger('advanced')
-            >>> log = StaticDefaults(log, {'foo': 'bar', 'qux': 'baz'})
-            >>> log = StaticDefaults(log, {'blam': 'splat'})
-            >>> log.warning('Hello, world!', extra={'foo': 'override'})
-                # yields {'foo': 'override', 'qux': 'baz', 'blam': 'splat'}
-        
-        .. _`LoggerAdapter`: http://docs.python.org/2/library/logging.html#loggeradapter-objects
-        
-        
-        Testing support
-        ---------------
-        
-        To help inspecting the ``extra`` values, gocept.logging comes with a
-        specialized handler for testing::
-        
-            >>> import gocept.logging
-            >>> import logging
-        
-            >>> log = logging.getLogger('testing')
-            >>> handler = gocept.logging.TestingHandler()
-            >>> log.addHandler(handler)
-            >>> log.warning('Hello, world!', extra={'foo': 'bar'})
-            >>> handler.messages[0].extra['foo']
-            'bar'
-        
-        The TestingHandler records each log message as a namedtuple of type
-        ``gocept.logging.testing.LogMessage`` so you an easily access all parts of the
-        message.
-        
-        
-        Example configuration
-        =====================
-        
-        Creating semi-structured log messages is the first half of the issue, while
-        analysing them is the second half. We use `logstash`_ for that purpose.
-        
-        The recommended setup is::
-        
-            application -> syslogd on localhost -> logstash on central host (via UDP syslog input)
-        
-        For development you might want to leave out the middle man and configure the
-        application to send log messags via syslog protocol directly to logstash.
-        
-        
-        .. _`logstash`: http://logstash.net/
-        
-        
-        Setup with ini file
-        -------------------
-        
-        If you have a paste.ini for your application, you might use something like
-        this::
-        
-            [loggers]
-            keys = root
-        
-            [handlers]
-            keys = console, syslog
-        
-            [formatters]
-            keys = generic, keyvalue
-        
-            [logger_root]
-            level = INFO
-            handlers = console, syslog
-        
-            [handler_console]
-            class = StreamHandler
-            args = (sys.stderr,)
-            level = NOTSET
-            formatter = generic
-        
-            [formatter_generic]
-            format = %(asctime)s %(levelname)-5.5s %(name)s: %(message)s
-        
-            [handler_syslog]
-            class = logging.handlers.SysLogHandler
-            args = ()
-            formatter = keyvalue
-        
-            [formatter_keyvalue]
-            class = gocept.logging.SyslogKeyValueFormatter
-        
-        
-        Setup with ZConfig
-        ------------------
-        
-        If you have a Zope application, you might use something like this::
-        
-            <eventlog>
-              <logfile>
-                formatter zope.exceptions.log.Formatter
-                format %(asctime)s %(levelname)-5.5s %(name)s: %(message)s
-                path STDOUT
-              </logfile>
-              <syslog>
-                formatter gocept.logging.SyslogKeyValueFormatter
-              </syslog>
-            </eventlog>
-        
-        
-        syslogd configuration
-        ---------------------
-        
-        rsyslog::
-        
-            $EscapeControlCharactersOnReceive off
-            $MaxMessageSize 64k
-            user.* @localhost:5140
-        
-        The first two lines are to support tracebacks, which are multiline and might
-        take up some space. The last line tells rsyslogd to forward all messages of the
-        ``user`` facility (which is what stdlib ``logging`` uses by default) via syslog
-        UDP protocol to localhost port 5140 (where logstash might be listening).
-        
-        
-        logstash configuration
-        ----------------------
-        
-        ::
-        
-            input {
-                    tcp {
-                            host => "localhost"
-                            port => 5140
-                            type => syslog
-                    }
-                    udp {
-                            host => "localhost"
-                            port => 5140
-                            type => syslog
-                    }
-            }
-        
-            filter {
-                    grok {
-                            type => "syslog"
-                            pattern => [ "(?m)<%{POSINT:syslog_pri}>%{SYSLOGTIMESTAMP:syslog_timestamp} %{SYSLOGHOST:syslog_hostname} %{DATA:syslog_program}(?:\[%{POSINT:syslog_pid}\])?: %{GREEDYDATA:syslog_message}" ]
-                    }
-                    syslog_pri {
-                            type => "syslog"
-                    }
-                    date {
-                            type => "syslog"
-                            match => [ "syslog_timestamp", "MMM  d HH:mm:ss", "MMM dd HH:mm:ss" ]
-                    }
-                    mutate {
-                            type => "syslog"
-                            exclude_tags => "_grokparsefailure"
-                            replace => [ "@source_host", "%{syslog_hostname}" ]
-                            replace => [ "@message", "%{syslog_program}: %{syslog_message}" ]
-                    }
-                    mutate {
-                            type => "syslog"
-                            remove => [ "syslog_hostname", "syslog_timestamp" ]
-                    }
-                    kv {
-                            exclude_tags => "_grokparsefailure"
-                            type => "syslog"
-                    }
-            }
-        
-            output {
-                    elasticsearch { embedded => true }
-            }
-        
-        
-        Additional features
-        ===================
-        
-        ArgumentParser
-        --------------
-        
-        The provided ``gocept.logging.ArgumentParser`` provides you with the ability to
-        set a ``logging`` level in you runscripts.::
-        
-            from gocept.logging import ArgumentParser
-            parser = ArgumentParser()
-            # Optionally set a custom log format, defaults to ``logging.BASIC_FORMAT``
-            parser.LOG_FORMAT = 'LOG:%(message)s'
-            # add your arguments with parser.add_argument() here
-            options = parser.parse_args()
-        
-        Use ``your_run_script --help`` to see a help message about the arguments you
-        can pass to set logging level.
-        
-        
-        Known bugs
-        ==========
-        
-        If you log messages as unicode, e.g. ``log.info(u'foo')``, the SyslogHandler
-        will (incorrectly) prepend a byte-order mark, which confuses the logstash
-        parser, resulting in "_grokparsefailure". This is a `known bug`_ in the Python
-        standard library that has been fixed in Python-2.7.4.
-        
-        .. _`known bug`: http://bugs.python.org/issue14452
-        
-        
-        =========================
-        Developing gocept.logging
-        =========================
-        
-        :Author:
-            `gocept <http://gocept.com/>`_ <mail@gocept.com>
-        
-        :PyPI page:
-            http://pypi.python.org/pypi/gocept.logging/
-        
-        :Issues:
-            `report by e-mail <mail@gocept.com>`_
-        
-        :Source code:
-            https://bitbucket.org/gocept/gocept.logging/
-        
-        :Current change log:
-            https://bitbucket.org/gocept/gocept.logging/raw/tip/CHANGES.txt
-        
-        
-        =============================
-        Change log for gocept.logging
-        =============================
-        
-        0.8.1 (2017-01-09)
-        ==================
-        
-        - Fix `setup.py` to use relative paths.
-        
-        
-        0.8 (2016-03-17)
-        ================
-        
-        - Declare compatibility with PyPy and PyPy3.
-        
-        
-        0.7 (2015-09-29)
-        ================
-        
-        - Declare Python 3.5 compatibility.
-        
-        
-        0.6 (2015-09-17)
-        ================
-        
-        - Declare Python 3.4 compatibility.
-        
-        - ``ArgumentParser.parse_args()`` now stores the computed log level on the
-          ``log_level`` attribute of the return value.
-        
-        0.5 (2014-02-07)
-        ================
-        
-        - Allow to change log format for the ``ArgumentParser``
-        
-        
-        0.4 (2013-09-24)
-        ================
-        
-        - Handle non-string log messages properly.
-        
-        
-        0.3 (2013-09-04)
-        ================
-        
-        - Added sepcialized ``argparse.ArgumentParser`` which enables user to set the
-          ``logging`` level by default..
-        
-        
-        0.2 (2013-08-24)
-        ================
-        
-        - Add timestamp and hostname to syslog messages,
-          this allows plugging SyslogKeyValueFormatter directly into logstash
-          without an intermediary syslogd.
-        
-        
-        0.1 (2013-08-16)
-        ================
-        
-        - initial release
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.7
+Provides-Extra: test
+License-File: LICENSE.txt
+
+==============
+gocept.logging
+==============
+
+.. image:: https://github.com/gocept/gocept.logging/workflows/tests/badge.svg
+    :target: https://github.com/gocept/gocept.logging/actions?query=workflow%3Atests
+.. image:: https://coveralls.io/repos/github/gocept/gocept.logging/badge.svg
+    :target: https://coveralls.io/github/gocept/gocept.logging
+
+.. contents::
+   :depth: 2
+
+This package provides infrastructure for semi-structured log messages.
+
+This means appending easily parseable information after the free-text log
+message to facilitate analysis of the logs later on. The ``logging`` module of
+the Python standard library already has support for this, via the ``extra``
+parameter. gocept.logging provides a ``Formatter`` that extracts these
+``extra`` values, formats them as ``key=value`` pairs and appends them to the
+message::
+
+    >>> import gocept.logging
+    >>> import logging
+    >>> import sys
+
+    >>> handler = logging.StreamHandler(sys.stdout)
+    >>> handler.setFormatter(gocept.logging.SyslogKeyValueFormatter())
+    >>> log = logging.getLogger('example')
+    >>> log.addHandler(handler)
+    >>> log.warning('Hello, world!', extra={'foo': 'bar'})
+    Aug 24 12:10:08 localhost example: Hello, world! foo=bar
+
+This package is tested to be compatible with Python version 2.7 and 3.3.
+
+
+Advanced usage
+==============
+
+If you have ``extra`` values that you always want to pass to your log messages
+(e.g things like the current user, session id, ...) you can wrap your logger
+with an `LoggerAdapter`_ that prefills these values. gocept.logging provides
+one that allows both stacking adapters and overriding the prefilled values::
+
+    >>> from gocept.logging.adapter import StaticDefaults
+    >>> import logging
+
+    >>> log = logging.getLogger('advanced')
+    >>> log = StaticDefaults(log, {'foo': 'bar', 'qux': 'baz'})
+    >>> log = StaticDefaults(log, {'blam': 'splat'})
+    >>> log.warning('Hello, world!', extra={'foo': 'override'})
+        # yields {'foo': 'override', 'qux': 'baz', 'blam': 'splat'}
+
+.. _`LoggerAdapter`: http://docs.python.org/2/library/logging.html#loggeradapter-objects
+
+
+Testing support
+---------------
+
+To help inspecting the ``extra`` values, gocept.logging comes with a
+specialized handler for testing::
+
+    >>> import gocept.logging
+    >>> import logging
+
+    >>> log = logging.getLogger('testing')
+    >>> handler = gocept.logging.TestingHandler()
+    >>> log.addHandler(handler)
+    >>> log.warning('Hello, world!', extra={'foo': 'bar'})
+    >>> handler.messages[0].extra['foo']
+    'bar'
+
+The TestingHandler records each log message as a namedtuple of type
+``gocept.logging.testing.LogMessage`` so you an easily access all parts of the
+message.
+
+
+Example configuration
+=====================
+
+Creating semi-structured log messages is the first half of the issue, while
+analysing them is the second half. We use `logstash`_ for that purpose.
+
+The recommended setup is::
+
+    application -> syslogd on localhost -> logstash on central host (via UDP syslog input)
+
+For development you might want to leave out the middle man and configure the
+application to send log messags via syslog protocol directly to logstash.
+
+
+.. _`logstash`: http://logstash.net/
+
+
+Setup with ini file
+-------------------
+
+If you have a paste.ini for your application, you might use something like
+this::
+
+    [loggers]
+    keys = root
+
+    [handlers]
+    keys = console, syslog
+
+    [formatters]
+    keys = generic, keyvalue
+
+    [logger_root]
+    level = INFO
+    handlers = console, syslog
+
+    [handler_console]
+    class = StreamHandler
+    args = (sys.stderr,)
+    level = NOTSET
+    formatter = generic
+
+    [formatter_generic]
+    format = %(asctime)s %(levelname)-5.5s %(name)s: %(message)s
+
+    [handler_syslog]
+    class = logging.handlers.SysLogHandler
+    args = ()
+    formatter = keyvalue
+
+    [formatter_keyvalue]
+    class = gocept.logging.SyslogKeyValueFormatter
+
+
+Setup with ZConfig
+------------------
+
+If you have a Zope application, you might use something like this::
+
+    <eventlog>
+      <logfile>
+        formatter zope.exceptions.log.Formatter
+        format %(asctime)s %(levelname)-5.5s %(name)s: %(message)s
+        path STDOUT
+      </logfile>
+      <syslog>
+        formatter gocept.logging.SyslogKeyValueFormatter
+      </syslog>
+    </eventlog>
+
+
+syslogd configuration
+---------------------
+
+rsyslog::
+
+    $EscapeControlCharactersOnReceive off
+    $MaxMessageSize 64k
+    user.* @localhost:5140
+
+The first two lines are to support tracebacks, which are multiline and might
+take up some space. The last line tells rsyslogd to forward all messages of the
+``user`` facility (which is what stdlib ``logging`` uses by default) via syslog
+UDP protocol to localhost port 5140 (where logstash might be listening).
+
+
+logstash configuration
+----------------------
+
+::
+
+    input {
+            tcp {
+                    host => "localhost"
+                    port => 5140
+                    type => syslog
+            }
+            udp {
+                    host => "localhost"
+                    port => 5140
+                    type => syslog
+            }
+    }
+
+    filter {
+            grok {
+                    type => "syslog"
+                    pattern => [ "(?m)<%{POSINT:syslog_pri}>%{SYSLOGTIMESTAMP:syslog_timestamp} %{SYSLOGHOST:syslog_hostname} %{DATA:syslog_program}(?:\[%{POSINT:syslog_pid}\])?: %{GREEDYDATA:syslog_message}" ]
+            }
+            syslog_pri {
+                    type => "syslog"
+            }
+            date {
+                    type => "syslog"
+                    match => [ "syslog_timestamp", "MMM  d HH:mm:ss", "MMM dd HH:mm:ss" ]
+            }
+            mutate {
+                    type => "syslog"
+                    exclude_tags => "_grokparsefailure"
+                    replace => [ "@source_host", "%{syslog_hostname}" ]
+                    replace => [ "@message", "%{syslog_program}: %{syslog_message}" ]
+            }
+            mutate {
+                    type => "syslog"
+                    remove => [ "syslog_hostname", "syslog_timestamp" ]
+            }
+            kv {
+                    exclude_tags => "_grokparsefailure"
+                    type => "syslog"
+            }
+    }
+
+    output {
+            elasticsearch { embedded => true }
+    }
+
+
+Additional features
+===================
+
+ArgumentParser
+--------------
+
+The provided ``gocept.logging.ArgumentParser`` provides you with the ability to
+set a ``logging`` level in you runscripts.::
+
+    from gocept.logging import ArgumentParser
+    parser = ArgumentParser()
+    # Optionally set a custom log format, defaults to ``logging.BASIC_FORMAT``
+    parser.LOG_FORMAT = 'LOG:%(message)s'
+    # add your arguments with parser.add_argument() here
+    options = parser.parse_args()
+
+Use ``your_run_script --help`` to see a help message about the arguments you
+can pass to set logging level.
+
+
+Known bugs
+==========
+
+If you log messages as unicode, e.g. ``log.info(u'foo')``, the SyslogHandler
+will (incorrectly) prepend a byte-order mark, which confuses the logstash
+parser, resulting in "_grokparsefailure". This is a `known bug`_ in the Python
+standard library that has been fixed in Python-2.7.4.
+
+.. _`known bug`: http://bugs.python.org/issue14452
+
+
+=========================
+Developing gocept.logging
+=========================
+
+:Author:
+    `gocept <http://gocept.com/>`_ <mail@gocept.com>
+
+:PyPI page:
+    http://pypi.python.org/pypi/gocept.logging/
+
+:Issues:
+    `report by e-mail <mail@gocept.com>`_
+
+:Source code:
+    https://github.com/gocept/gocept.logging
+
+:Current change log:
+    https://raw.githubusercontent.com/gocept/gocept.logging/master/CHANGES.rst
+
+
+=============================
+Change log for gocept.logging
+=============================
+
+1.0 (2023-07-18)
+================
+
+- Drop support for Python 2.7, 3.3, 3.4, 3.5, 3.6.
+
+- Add support for Python 3.7, 3.8 3.9, 3.10, 3.11.
+
+- Add an alias ``.warn`` for ``.warning`` for ``StaticDefaults``. (#1)
+
+
+0.8.1 (2017-01-09)
+==================
+
+- Fix `setup.py` to use relative paths.
+
+
+0.8 (2016-03-17)
+================
+
+- Declare compatibility with PyPy and PyPy3.
+
+
+0.7 (2015-09-29)
+================
+
+- Declare Python 3.5 compatibility.
+
+
+0.6 (2015-09-17)
+================
+
+- Declare Python 3.4 compatibility.
+
+- ``ArgumentParser.parse_args()`` now stores the computed log level on the
+  ``log_level`` attribute of the return value.
+
+0.5 (2014-02-07)
+================
+
+- Allow to change log format for the ``ArgumentParser``
+
+
+0.4 (2013-09-24)
+================
+
+- Handle non-string log messages properly.
+
+
+0.3 (2013-09-04)
+================
+
+- Added sepcialized ``argparse.ArgumentParser`` which enables user to set the
+  ``logging`` level by default..
+
+
+0.2 (2013-08-24)
+================
+
+- Add timestamp and hostname to syslog messages,
+  this allows plugging SyslogKeyValueFormatter directly into logstash
+  without an intermediary syslogd.
+
+
+0.1 (2013-08-16)
+================
+
+- initial release
```

### Comparing `gocept.logging-0.8.1/src/gocept.logging.egg-info/SOURCES.txt` & `gocept.logging-1.0/src/gocept.logging.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 .coveragerc
-.hgignore
-.hgtags
-CHANGES.rst
-COPYRIGHT.rst
-HACKING.rst
-LICENSE.rst
+.pre-commit-config.yaml
+LICENSE.txt
+MANIFEST.in
 README.rst
 pytest.ini
+setup.cfg
 setup.py
 tox.ini
 src/gocept/__init__.py
 src/gocept.logging.egg-info/PKG-INFO
 src/gocept.logging.egg-info/SOURCES.txt
 src/gocept.logging.egg-info/dependency_links.txt
-src/gocept.logging.egg-info/entry_points.txt
 src/gocept.logging.egg-info/namespace_packages.txt
 src/gocept.logging.egg-info/not-zip-safe
 src/gocept.logging.egg-info/requires.txt
 src/gocept.logging.egg-info/top_level.txt
 src/gocept/logging/__init__.py
 src/gocept/logging/adapter.py
 src/gocept/logging/argumentparser.py
```

