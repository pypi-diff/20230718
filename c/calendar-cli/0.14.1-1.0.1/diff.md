# Comparing `tmp/calendar_cli-0.14.1.tar.gz` & `tmp/calendar_cli-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calendar_cli-0.14.1.tar", last modified: Thu Nov 24 00:18:55 2022, max compression
+gzip compressed data, was "calendar_cli-1.0.1.tar", last modified: Tue Jul 18 12:02:01 2023, max compression
```

## Comparing `calendar_cli-0.14.1.tar` & `calendar_cli-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 tobias    (7385) tobias    (7385)        0 2022-11-24 00:18:55.365459 calendar_cli-0.14.1/
--rw-r--r--   0 tobias    (7385) tobias    (7385)    35147 2019-09-10 13:09:07.000000 calendar_cli-0.14.1/LICENSE.TXT
--rw-r--r--   0 tobias    (7385) tobias    (7385)      677 2022-11-24 00:18:55.365459 calendar_cli-0.14.1/PKG-INFO
--rw-r--r--   0 tobias    (7385) tobias    (7385)    12760 2022-10-08 23:55:31.000000 calendar_cli-0.14.1/README.md
-drwxr-xr-x   0 tobias    (7385) tobias    (7385)        0 2022-11-24 00:18:55.365459 calendar_cli-0.14.1/bin/
--rw-r--r--   0 tobias    (7385) tobias    (7385)       74 2022-11-06 09:06:58.000000 calendar_cli-0.14.1/bin/calendar-cli
--rw-r--r--   0 tobias    (7385) tobias    (7385)       74 2022-11-06 09:06:58.000000 calendar_cli-0.14.1/bin/calendar-cli.py
-drwxr-xr-x   0 tobias    (7385) tobias    (7385)        0 2022-11-24 00:18:55.365459 calendar_cli-0.14.1/calendar_cli/
--rw-r--r--   0 tobias    (7385) tobias    (7385)        0 2022-11-06 08:52:39.000000 calendar_cli-0.14.1/calendar_cli/__init__.py
--rwxr-xr-x   0 tobias    (7385) tobias    (7385)    22080 2022-11-23 23:32:56.000000 calendar_cli-0.14.1/calendar_cli/cal.py
--rwxr-xr-x   0 tobias    (7385) tobias    (7385)    47653 2022-11-23 23:32:36.000000 calendar_cli-0.14.1/calendar_cli/legacy.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)      612 2022-11-24 00:18:45.000000 calendar_cli-0.14.1/calendar_cli/metadata.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)     1395 2022-10-08 23:55:31.000000 calendar_cli-0.14.1/calendar_cli/template.py
-drwxr-xr-x   0 tobias    (7385) tobias    (7385)        0 2022-11-24 00:18:55.365459 calendar_cli-0.14.1/calendar_cli.egg-info/
--rw-r--r--   0 tobias    (7385) tobias    (7385)      677 2022-11-24 00:18:55.000000 calendar_cli-0.14.1/calendar_cli.egg-info/PKG-INFO
--rw-r--r--   0 tobias    (7385) tobias    (7385)      403 2022-11-24 00:18:55.000000 calendar_cli-0.14.1/calendar_cli.egg-info/SOURCES.txt
--rw-r--r--   0 tobias    (7385) tobias    (7385)        1 2022-11-24 00:18:55.000000 calendar_cli-0.14.1/calendar_cli.egg-info/dependency_links.txt
--rw-r--r--   0 tobias    (7385) tobias    (7385)       45 2022-11-24 00:18:55.000000 calendar_cli-0.14.1/calendar_cli.egg-info/entry_points.txt
--rw-r--r--   0 tobias    (7385) tobias    (7385)       46 2022-11-24 00:18:55.000000 calendar_cli-0.14.1/calendar_cli.egg-info/requires.txt
--rw-r--r--   0 tobias    (7385) tobias    (7385)       17 2022-11-24 00:18:55.000000 calendar_cli-0.14.1/calendar_cli.egg-info/top_level.txt
--rw-r--r--   0 tobias    (7385) tobias    (7385)       38 2022-11-24 00:18:55.365459 calendar_cli-0.14.1/setup.cfg
--rw-r--r--   0 tobias    (7385) tobias    (7385)     1314 2022-11-06 09:14:10.000000 calendar_cli-0.14.1/setup.py
+drwxr-xr-x   0 tobias    (7385) tobias    (7385)        0 2023-07-18 12:02:01.752539 calendar_cli-1.0.1/
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    35147 2019-09-10 13:09:07.000000 calendar_cli-1.0.1/LICENSE.TXT
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      676 2023-07-18 12:02:01.752539 calendar_cli-1.0.1/PKG-INFO
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    11107 2023-07-17 22:21:44.000000 calendar_cli-1.0.1/README.md
+drwxr-xr-x   0 tobias    (7385) tobias    (7385)        0 2023-07-18 12:02:01.752539 calendar_cli-1.0.1/bin/
+-rwxr-xr-x   0 tobias    (7385) tobias    (7385)       74 2022-11-06 09:06:58.000000 calendar_cli-1.0.1/bin/calendar-cli
+-rwxr-xr-x   0 tobias    (7385) tobias    (7385)       74 2022-11-06 09:06:58.000000 calendar_cli-1.0.1/bin/calendar-cli.py
+drwxr-xr-x   0 tobias    (7385) tobias    (7385)        0 2023-07-18 12:02:01.752539 calendar_cli-1.0.1/calendar_cli/
+-rw-r--r--   0 tobias    (7385) tobias    (7385)        0 2022-11-06 08:52:39.000000 calendar_cli-1.0.1/calendar_cli/__init__.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     7154 2022-12-03 16:56:51.000000 calendar_cli-1.0.1/calendar_cli/config.py
+-rwxr-xr-x   0 tobias    (7385) tobias    (7385)    43494 2023-07-18 11:45:21.000000 calendar_cli-1.0.1/calendar_cli/legacy.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      611 2023-07-18 11:59:33.000000 calendar_cli-1.0.1/calendar_cli/metadata.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     1395 2022-10-08 23:55:31.000000 calendar_cli-1.0.1/calendar_cli/template.py
+drwxr-xr-x   0 tobias    (7385) tobias    (7385)        0 2023-07-18 12:02:01.752539 calendar_cli-1.0.1/calendar_cli.egg-info/
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      676 2023-07-18 12:02:01.000000 calendar_cli-1.0.1/calendar_cli.egg-info/PKG-INFO
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      385 2023-07-18 12:02:01.000000 calendar_cli-1.0.1/calendar_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 tobias    (7385) tobias    (7385)        1 2023-07-18 12:02:01.000000 calendar_cli-1.0.1/calendar_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 tobias    (7385) tobias    (7385)       51 2023-07-18 12:02:01.000000 calendar_cli-1.0.1/calendar_cli.egg-info/requires.txt
+-rw-r--r--   0 tobias    (7385) tobias    (7385)       13 2023-07-18 12:02:01.000000 calendar_cli-1.0.1/calendar_cli.egg-info/top_level.txt
+-rw-r--r--   0 tobias    (7385) tobias    (7385)       38 2023-07-18 12:02:01.752539 calendar_cli-1.0.1/setup.cfg
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     1187 2023-01-09 12:22:38.000000 calendar_cli-1.0.1/setup.py
+drwxr-xr-x   0 tobias    (7385) tobias    (7385)        0 2023-07-18 12:02:01.752539 calendar_cli-1.0.1/tests/
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     2741 2023-07-17 22:21:44.000000 calendar_cli-1.0.1/tests/test_cal.py
```

### Comparing `calendar_cli-0.14.1/LICENSE.TXT` & `calendar_cli-1.0.1/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `calendar_cli-0.14.1/PKG-INFO` & `calendar_cli-1.0.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calendar_cli
-Version: 0.14.1
+Version: 1.0.1
 Summary: Simple command-line CalDav client, for adding and browsing calendar items, todo list items, etc.
 Home-page: https://github.com/tobixen/calendar-cli
 Author: Tobias Brox
 Author-email: t-calendar-cli@tobixen.no
 Maintainer: Tobias Brox
 License: GPLv3+
 Classifier: Environment :: Web Environment
```

### Comparing `calendar_cli-0.14.1/README.md` & `calendar_cli-1.0.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,60 +1,53 @@
 calendar-cli
 ============
 
-Simple command-line CalDav client, making it possible to add calendar events, browse an agenda and doing task management towards a caldav server.
+Simple command-line CalDAV client, making it possible to add calendar events, browse an agenda and do task management using a caldav server.
+
+THIS IS THE LEGACY VERSION.  If you're already using calendar-cli and don't want to change anything, then keep using it.  If you need a production-ready mature command-line utility for accessing your calendar, then this is the right tool ... as for now.  I decided to change a bit on the user interface, rather than breaking backward compatibility I made a new command name `plann`.  I would recommend visit https://github.com/tobixen/plann for the new version.
+
+calendar-cli will be maintained primarily for backward compatibility.  Pull-requests dealing with bugfixes or minor "missing" features will be considered - but for anyone in need of a command-line interface towards a CalDAV calendar server, the recommendation is to use [plann](https://github.com/tobixen/plann) instead.
 
 Other tools
 -----------
 
 There is another project out there, "Command-line Interface for Google Calendar", previously located at pypi under the calendar-cli name.  It has now been renamed to gcalendar-cli to avoid name conflict, and is available at https://pypi.python.org/pypi/gcalendar-cli/
 
-There is a "competing" project at https://github.com/geier/khal - you may want to check it out - it's more mature but probably more complex.  It's using a "vsyncdir" backend - if I've understood it correctly, that involves building a local copy of the calendar.  The philosophy behind calendar-cli is slightly different, calendar-cli is supposed to be a simple cli-based caldav+ical client.  No synchronization, no local storage, just client-side operations.
-
-New vs old interface
---------------------
-
-DO YOU HAVE OPINIONS ON WHAT COLOR TO PAINT THE BIKE SHED WITH?  VISIT https://github.com/tobixen/calendar-cli/issues/88 NOW!
-
-calendar-cli.py is the old interface, it will hang around and be supported for some time to come.  cal.py is the new interface, but until version 1.0 is ready, there will still be functionality in calendar-cli that isn't mirrored to cal.py.
-
-I wanted a short and easy command name, since `cal(1)` is already a popular Unix command, I'm considering to install it into /usr/bin with the name `kal`, but I'm a bit uncertain (seems either like a bad typo or an attempt on localizing the command into my native language?)
+There is a "competing" project at https://github.com/geier/khal - you may want to check it out - it's more mature but probably more complex.  It's using a "vsyncdir" backend - if I've understood it correctly, that involves building a local copy of the calendar.  The philosophy behind `calendar-cli` is slightly different, `calendar-cli` is supposed to be a simple cli-based caldav+ical client.  No synchronization, no local storage, just client-side operations.
 
 Usage examples
 --------------
 
-The commands and options will be described further down, however examples often beats documentation.
+The commands and options will be described further down, however examples often beat documentation.
 
 First, check the tests folder - the file tests.sh shows some basic usage examples.  If you have radicale installed (`sudo pip install radicale`), you can try executing test_calendar-cli.sh in the test folder, it basically sets up a temporary radicale server and executes the tests.sh towards that server.  If test_calendar-cli.sh breaks then _please_ raise an issue on the github or try to reach out through other channels.
 
 In the examples folder there is a script I was using on a regular basis for task management for a while.
 
 Installation
 ------------
 
-calendar-cli depends on quite some python libraries, i.e. pytz, caldav, etc.  "sudo ./setup.py install" should take care of all those eventually.
-
-The calendar-cli executable can be executed as it is, or copied to /usr/bin.  Make sure to copy the content - as of v0.12, calendar-cli is actually a symlink to calendar_cli.py.  This mess will be fixed up in v1.0.
+`calendar-cli` depends on quite some python libraries, i.e. pytz, caldav, etc.  "sudo ./setup.py install" should take care of all those eventually, and will also make an executable under /usr/bin
 
 Support
 -------
 
 \#calendar-cli at irc.oftc.net, eventually t-calendar-cli@tobixen.no, eventually the issue tracker at https://github.com/tobixen/calendar-cli/issues
 
 Before reaching out, please make sure all the dependencies are installed and that you've installed the latest version of the caldav python library.
 
 Rationale
 ---------
 
 GUIs and Web-UIs are nice for some purposes, but I really find the command line unbeatable when it comes to:
 
-* Minor stuff that are repeated often.  Writing something like "todo add make a calendar-cli system" or "calendar add 'tomorrow 15:40+2h' doctor appointment" is (for me) faster than navigating into some web calendar interface and add an item there.
+* Minor stuff that is repeated often.  Writing something like "todo add make a calendar-cli system" or "calendar add 'tomorrow 15:40+2h' doctor appointment" is (for me) faster than navigating into some web calendar interface and add an item there.
 * Things that are outside the scope of the UI.  Here is one of many tasks I'd like to do: "go through the work calendar, find all new calendar events that are outside office hours, check up with the personal calendar if there are potential conflicts, add some information at the personal calendar if appropriate", and vice versa - it has to be handled very manually if doing it through any normal calendar application as far as I know, but if having some simple CLI or python library I could easily make some interactive script that would help me doing the operation above.
 
-When I started writing calendar-cli, all I could find was cadaver and the CalDAVClientLibrary.  Both of those seems to be a bit shortcoming; they seem to miss the iCalendar parsing/generation, and there are things that simply cannot be done through those tools.
+When I started writing `calendar-cli`, all I could find was cadaver and the CalDAVClientLibrary.  Both of those seems to be a bit shortcoming; they seem to miss the iCalendar parsing/generation, and there are things that simply cannot be done through those tools.
 
 Synopsis
 --------
 
     calendar-cli.py [global options] [command] [command options] [subcommand] [subcommand options] [subcommand arguments] ...
 
 I'm intending to make it easier by allowing calendar-cli.py to be symlinked to the various commands and also to allow the options to be placed wherever.
@@ -97,94 +90,101 @@
 
 Supported in v0.12:
 
 * anything recognized by dateutil.parser.parse()
 * An iso time stamp, followed with the duration, using either + or space as separator.  Duration is a number postfixed by s for seconds, m for minutes, h for hours, d for days, w for weeks and y for years (i.e. 2013-09-10T13:37+30d)
 * ISO dates.  For full day events, make sure to specify the duration in days.
 
-All of those would eventually be supported in future versions if it's not too difficult to achieve:
-
-* Two ISO timestamps separated by a dash (-)
-* "tomorrow" instead of an ISO date
-* weekday instead of an ISO date (this seems supported already by dateutil.parser.parse)
-* clock time without the date; event will be assumed to start within 24 hours.
-
-Alternatively, endtime or duration can be given through options (not supported as of 0.12)
-
 ### Getting out customized information through --todo-template and --event-template
 
-This is a string containing variables enclosed in curly braces, like "uid: {uid}".  Full documentation of the available variables will be given in version 1.0.
+This is a string containing variables enclosed in curly braces, like "uid: {uid}".
 
 Particularly the uid can be useful, as one may want to use the uid for things like deleting events and postponing tasks.
 
 In the examples folder there is a task management script which will use the --todo-template to create a new shell script for postponing all overdue tasks.  This shell script can then be edited interactively and run.
 
 ### Task management
 
 With the todo-command, there are quite some options available (i.e. --categories, --limit, --todo-uid, etc) to select or filter tasks.  Those are used by the commands list, edit, postpone, complete and delete.  A typical use-case scenario is to first use the "list" command, tweak the filtering options to get a list containing the tasks one wants to operate with, and then use either edit, postpone, complete or delete.
 
 The file TASK_MANAGEMENT.md contains some thoughts on how to organize tasks.
 
 Configuration file
 ------------------
 
-Configuration file is by default located in $HOME/.config/calendar.conf and should be in json syntax.  You may run `calendar-cli --interactive-config` if you don't feel comfortable with hand-crafting configuration in json syntax, though this feature is not tested regularly.
+Configuration file is by default located in $HOME/.config/calendar.conf. You may run `calendar-cli --interactive-config` if you don't feel comfortable with hand-crafting configuration in json syntax, though this feature is not tested regularly.
+
+(I considered .ini, but I was told that it's actually not a standard.  I'd like any calendar application to be able to access the file, hence calendar.conf and not calendar-cli.conf)
 
-(I considered a configuration file in .ini-format, having a "default"-section with default values for any global options, and optionally other sections for different CalDAV-servers.  Asking a bit around for recommendations on config file format as well as location, I was told that the .ini-format is not a standard, I'd be better off using a standard like yaml, json or xml.  Personally I like json a bit better than yaml - after consulting with a friend I ended up with json.  Location ... I think it's "cleaner" to keep it in ~/.config/, and I'd like any calendar application to be able to access the file, hence it got ~/.config/calendar.conf rather than ~/.calendar-cli.conf)
+### calendar-cli
 
 The file may look like this:
 
 ```json
 { "default":
   { "caldav_url": "http://foo.bar.example.com/caldav/",
     "caldav_user": "luser",
     "caldav_pass": "insecure"
   }
 }
 ```
 A configuration with multiple sections may look like this:
 
 ```json
-{ "default":
+{
+"default":
   { "caldav_url": "http://foo.bar.example.com/caldav/",
     "caldav_user": "luser",
     "caldav_pass": "insecure"
   },
-  "caldav_url": "http://foo.baz.example.com/caldav/",
+"baz":
+  { "caldav_url": "http://foo.baz.example.com/caldav/",
     "caldav_user": "luser2",
     "caldav_pass": "insecure2"
   }
 }
 ```
 
-Optionally, in addition (or even instead) of "default", other "sections" can be created and selected through the --config-section option.  The rationale is to allow configuration for multiple CalDAV-servers, or multiple calendars on the same CalDAV-server to remain in the same configuration file.  Later versions will eventually be capable of copying events, or putting events into several calendars.
+Sections may also include calendar urls or ids, and sections may inherit other sections:
 
-Remember to `chmod og-r ~/.config/calendar.conf` or `chmod 0600 ~/.config/calendar.conf`
+```json
+{
+"default":
+  { "caldav_url": "http://foo.bar.example.com/caldav/",
+    "caldav_user": "luser",
+    "caldav_pass": "insecure"
+  },
+"baz":
+  { "caldav_url": "http://foo.baz.example.com/caldav/",
+    "caldav_user": "luser2",
+    "caldav_pass": "insecure2"
+  }
+},
+"bazimportant":
+  { "inherits": "baz",
+    "calendar_url": "important"
+  }
+```
 
-### Examples
+Usage example
+-------------
 
 Add a calendar item "testevent" at 2013-10-01:
 
     ./calendar-cli.py --calendar-url=http://calendar.bekkenstenveien53c.oslo.no/caldav.php/tobias/calendar/ calendar add 2013-10-01 testevent
 
-(assumes that `caldav-url`, `calldav-pass` and `caldav-user` has been added into configuration file.  Those may also be added as command line options)
+(assumes that `caldav-url`, `caldav-pass` and `caldav-user` has been added into configuration file.  Those may also be added as command line options)
 
 Objectives
 ----------
 
 * It should be really easy and quick to add a todo-list item from the command line.
 * It should be really easy and quick to add a calendar item from the command line.
 * It should be possible to get out lists ("agenda") of calendar items and todo-items.
 * Interface for copying calendar items between calendars, even between calendars on distinct caldav servers
 
 Roadmap
 -------
-Eventually, the issues section in the github will probably be more up-to-date on the upcoming plans for enhancements and bug fixes.
-
-Possibly the next version after 0.12 will be 1.0.  One of the important things there is to refactor the calendar code, the filtering options available for tasks should also be available for the calendar.
 
-Other features that I eventually would like to add:
+calendar-cli will be maintained with bugfixes and security fixes, on requests from the community.  The maintainer is no longer using calendar-cli.
 
-* Allow pulling out an agenda for several calendars at once (though, with the current design it's so much easier to do it through a bash loop rather than in the python code, so this is postponed for a while)
-* Allow specification of event duration and/or event end time through options
-* Fix easy-to-use symlinks (or alternatively wrapper scripts)
-* Make some nosetests
+A new project https://github.com/tobixen/plann with a new interface has been forked off.
```

### Comparing `calendar_cli-0.14.1/calendar_cli/legacy.py` & `calendar_cli-1.0.1/calendar_cli/legacy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 #!/usr/bin/env python
 
 """
 https://github.com/tobixen/calendar-cli/ - high-level cli against caldav servers.
 
-This is the legacy calendar-cli.  A new interface is being built in cal.py - aka kal
-Feedback/wishes/discussions on the new cli can be held at
-https://github.com/tobixen/calendar-cli/issues/88
+This is the "legacy" interface - or, if you prefer,, the "long term support" interface.
 
-Copyright (C) 2013-2022 Tobias Brox and other contributors.
+Due to user feedback the new interface has been split out in a separate project.
+
+See https://plann.no
+
+Copyright (C) 2013-2023 Tobias Brox and other contributors.
 
 See https://www.gnu.org/licenses/gpl-3.0.en.html for license information.
 """
-
 import argparse
 import tzlocal
 ## we still need to use pytz, see https://github.com/collective/icalendar/issues/333
 #try:
 #    import zoneinfo
 #except:
 #    from backports import zoneinfo
 import pytz
 import time
 from datetime import datetime, timedelta, date
 from datetime import time as time_
 import dateutil.parser
 from dateutil.rrule import rrulestr
 from icalendar import Calendar,Event,Todo,Journal,Alarm
+from calendar_cli.config import interactive_config, config_section, read_config
 import vobject
 import caldav
 import uuid
 import json
 import os
 import logging
 import sys
@@ -258,105 +260,14 @@
         uid = x['UID'].to_ical()
         uids[uid] = uids.get(uid, []) + [x]
 
     for uid in uids:
         c.subcomponents = timezones + uids[uid]
         _calendar_addics(caldav_conn, c.to_ical(), uid, args)
 
-def interactive_config(args, config, remaining_argv):
-    import readline
-
-    new_config = False
-    section = 'default'
-    backup = {}
-    modified = False
-
-    print("Welcome to the interactive calendar configuration mode")
-    print("Warning - untested code ahead, raise issues at t-calendar-cli@tobixen.no or the github issue tracker")
-    print("It might be a good idea to read the documentation in parallel if running this for your first time")
-    if not config or not hasattr(config, 'keys'):
-        config = {}
-        print("No valid existing configuration found")
-        new_config = True
-    if config:
-        print("The following sections have been found: ")
-        print("\n".join(config.keys()))
-        if args.config_section and args.config_section != 'default':
-            section = args.config_section
-        else:
-            ## TODO: tab completion
-            section = raw_input("Chose one of those, or a new name / no name for a new configuration section: ")
-        if section in config:
-            backup = config[section].copy()
-        print("Using section " + section)
-    else:
-        section = 'default'
-
-    if not section in config:
-        config[section] = {}
-
-    for config_key in ('caldav_url', 'calendar_url', 'caldav_user', 'caldav_pass', 'caldav_proxy', 'ssl_verify_cert', 'language', 'timezone', 'inherits'):
-
-        if config_key == 'caldav_pass':
-            print("Config option caldav_pass - old value: **HIDDEN**")
-            value = getpass(prompt="Enter new value (or just enter to keep the old): ")
-        else:
-            print("Config option %s - old value: %s" % (config_key, config[section].get(config_key, '(None)')))
-            value = raw_input("Enter new value (or just enter to keep the old): ")
-
-        if value:
-            config[section][config_key] = value
-            modified = True
-
-    if not modified:
-        print("No configuration changes have been done")
-    else:
-        state = 'start'
-        while state == 'start':
-            options = []
-            if section:
-                options.append(('save', 'save configuration into section %s' % section))
-            if backup or not section:
-                options.append(('save_other', 'add this new configuration into a new section in the configuration file'))
-            if remaining_argv:
-                options.append(('use', 'use this configuration without saving'))
-            options.append(('abort', 'abort without saving'))
-            print("CONFIGURATION DONE ...")
-            for o in options:
-                print("Type %s if you want to %s" % o)
-            cmd = raw_input("Enter a command: ")
-            if cmd in ('use', 'abort'):
-                state = 'done'
-            if cmd in ('save', 'save_other'):
-                if cmd == 'save_other':
-                    new_section = raw_input("New config section name: ")
-                    config[new_section] = config[section]
-                    if backup:
-                        config[section] = backup
-                    else:
-                        del config[section]
-                    section = new_section
-                try:
-                    if os.path.isfile(args.config_file):
-                        os.rename(args.config_file, "%s.%s.bak" % (args.config_file, int(time.time())))
-                    with open(args.config_file, 'w') as outfile:
-                        json.dump(config, outfile, indent=4)
-                except Exception as e:
-                    print(e)
-                else:
-                    print("Saved config")
-                    state = 'done'
-
-
-
-
-    if args.config_section == 'default' and section != 'default':
-        config['default'] = config[section]
-    return config
-
 def create_alarm(message, relative_timedelta):
     alarm = Alarm()
     alarm.add('ACTION', 'DISPLAY')
     alarm.add('DESCRIPTION', message)
     alarm.add('TRIGGER', relative_timedelta, parameters={'VALUE':'DURATION'})
     return alarm
 
@@ -719,17 +630,23 @@
             t['due'] = task.instance.vtodo.due.value if hasattr(task.instance.vtodo,'due') else date.today()+timedelta(args.default_due)
             t['due_passed_mark'] = '!' if _force_datetime(t['due'], args) < _now() else ' '
             for timeattr in ('dtstart', 'due'):
                 t[timeattr] = t[timeattr].strftime(args.timestamp_format)
             for summary_attr in ('summary', 'location', 'description', 'url', 'uid'):
                 if hasattr(task.instance.vtodo, summary_attr):
                     t['summary'] = getattr(task.instance.vtodo, summary_attr).value
+                    t['summary'] = to_normal_str(t['summary'])
                     break
+            for attr in ('location', 'description', 'url'):
+                if hasattr(task.instance.vtodo, attr):
+                    t[attr] = getattr(task.instance.vtodo, attr).value
+                else:
+                    t[attr] = ""
+                t[attr] = to_normal_str(t[attr])
             t['uid'] = task.instance.vtodo.uid.value
-            t['summary'] = to_normal_str(t['summary'])
             print(args.todo_template.format(**t))
 
 def todo_complete(caldav_conn, args):
     if args.nocaldav:
         raise ValueError("No caldav connection, aborting")
     tasks = todo_select(caldav_conn, args)
     for task in tasks:
@@ -773,29 +690,20 @@
 def todo_delete(caldav_conn, args):
     if args.nocaldav:
         raise ValueError("No caldav connection, aborting")
     tasks = todo_select(caldav_conn, args)
     for task in tasks:
         task.delete()
 
-def config_section(config, section='default'):
-    if section in config and 'inherits' in config[section]:
-        ret = config_section(config, config[section]['inherits'])
-    else:
-        ret = {}
-    if section in config:
-        ret.update(config[section])
-    return ret
-
 def main():
     """
     the main function does (almost) nothing but parsing command line parameters
     """
 #    sys.stderr.write("""
-#The calendar-cli command is slowly being deprecated in favor of kal
+#The calendar-cli command is slowly being deprecated in favor of plann
 #Check https://github.com/tobixen/calendar-cli/issues/88
 #""")
             
     ## This boilerplate pattern is from
     ## http://stackoverflow.com/questions/3609852
     ## We want defaults for the command line options to be fetched from the config file
 
@@ -815,27 +723,15 @@
     conf_parser.add_argument("--config-section",
                              help="Specify config section; allows several caldav servers to be configured in the same config file",  default='default')
     conf_parser.add_argument("--interactive-config",
                              help="Interactively ask for configuration", action="store_true")
     args, remaining_argv = conf_parser.parse_known_args()
     conf_parser.add_argument("--version", action='version', version='%%(prog)s %s' % metadata["version"])
 
-    config = {}
-
-    try:
-        with open(args.config_file) as config_file:
-            config = json.load(config_file)
-    except IOError:
-        ## File not found
-        logging.info("no config file found")
-    except ValueError:
-        if args.interactive_config:
-            logging.error("error in config file.  Be aware that the current config file will be ignored and overwritten", exc_info=True)
-        else:
-            logging.error("error in config file.  You may want to run --interactive-config or fix the config file", exc_info=True)
+    config = read_config(args.config_file)
 
     if args.interactive_config:
         defaults = interactive_config(args, config, remaining_argv)
         if not remaining_argv:
             return
     else:
         defaults = config_section(config, args.config_section)
```

### Comparing `calendar_cli-0.14.1/calendar_cli/template.py` & `calendar_cli-1.0.1/calendar_cli/template.py`

 * *Files identical despite different names*

### Comparing `calendar_cli-0.14.1/calendar_cli.egg-info/PKG-INFO` & `calendar_cli-1.0.1/calendar_cli.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calendar-cli
-Version: 0.14.1
+Version: 1.0.1
 Summary: Simple command-line CalDav client, for adding and browsing calendar items, todo list items, etc.
 Home-page: https://github.com/tobixen/calendar-cli
 Author: Tobias Brox
 Author-email: t-calendar-cli@tobixen.no
 Maintainer: Tobias Brox
 License: GPLv3+
 Classifier: Environment :: Web Environment
```

### Comparing `calendar_cli-0.14.1/setup.py` & `calendar_cli-1.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,24 +23,18 @@
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Operating System :: POSIX",
         "Programming Language :: Python",
         "Topic :: Internet :: WWW/HTTP",
         "Topic :: Internet :: WWW/HTTP :: Dynamic Content :: CGI Tools/Libraries",
     ],
     scripts=['bin/calendar-cli.py', 'bin/calendar-cli'],
-    py_modules=['cal'],
     install_requires=[
         'icalendar',
-        'caldav>=0.10',
+        'caldav>=0.12-dev0',
 #        'isodate',
         'pytz', ## pytz is supposed to be obsoleted, but see https://github.com/collective/icalendar/issues/333 
         'tzlocal',
         'Click',
         'six'
     ],
-    entry_points={
-        'console_scripts': [
-            'kal = calendar_cli.cal:cli',
-        ],
-    },
    **metadata_
 )
```

