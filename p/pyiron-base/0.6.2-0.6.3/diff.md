# Comparing `tmp/pyiron_base-0.6.2.tar.gz` & `tmp/pyiron_base-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiron_base-0.6.2.tar", last modified: Wed Jul 12 13:55:34 2023, max compression
+gzip compressed data, was "pyiron_base-0.6.3.tar", last modified: Tue Jul 18 06:25:17 2023, max compression
```

## Comparing `pyiron_base-0.6.2.tar` & `pyiron_base-0.6.3.tar`

### file list

```diff
@@ -1,134 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:34.414587 pyiron_base-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-12 13:55:34.414587 pyiron_base-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:34.414587 pyiron_base-0.6.2/pyiron_base/
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-12 13:55:34.414587 pyiron_base-0.6.2/pyiron_base/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:34.402587 pyiron_base-0.6.2/pyiron_base/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/cli/control.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/cli/install.py
--rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/cli/ls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/cli/reloadfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/cli/rm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/cli/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:34.406587 pyiron_base-0.6.2/pyiron_base/database/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25072 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/database/filetable.py
--rw-r--r--   0 runner    (1001) docker     (123)    45395 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/database/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/database/jobtable.py
--rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/database/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/database/performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/database/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:34.406587 pyiron_base-0.6.2/pyiron_base/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/interfaces/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/interfaces/has_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     8855 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/interfaces/has_hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/interfaces/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/interfaces/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:34.406587 pyiron_base-0.6.2/pyiron_base/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27892 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/datamining.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/dynamic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:34.406587 pyiron_base-0.6.2/pyiron_base/jobs/job/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36920 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/job/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:34.406587 pyiron_base-0.6.2/pyiron_base/jobs/job/extension/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/job/extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/job/extension/executable.py
--rw-r--r--   0 runner    (1001) docker     (123)     9527 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/job/extension/jobstatus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:34.406587 pyiron_base-0.6.2/pyiron_base/jobs/job/extension/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/job/extension/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19894 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/job/extension/server/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    14501 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/job/extension/server/queuestatus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/job/extension/server/runmode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/job/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    57264 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/job/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    13349 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/job/interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)    13584 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/job/jobtype.py
--rw-r--r--   0 runner    (1001) docker     (123)    11822 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/job/path.py
--rw-r--r--   0 runner    (1001) docker     (123)    27025 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/job/runfunction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/job/template.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/job/toolkit.py
--rw-r--r--   0 runner    (1001) docker     (123)    14445 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/job/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/job/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:34.410587 pyiron_base-0.6.2/pyiron_base/jobs/master/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/master/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/master/flexible.py
--rw-r--r--   0 runner    (1001) docker     (123)    16909 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/master/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/master/interactivewrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/master/list.py
--rw-r--r--   0 runner    (1001) docker     (123)    32706 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/master/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)    13341 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/master/serial.py
--rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/master/submissionstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)    16462 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/script.py
--rw-r--r--   0 runner    (1001) docker     (123)    14652 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/jobs/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:34.410587 pyiron_base-0.6.2/pyiron_base/project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:34.410587 pyiron_base-0.6.2/pyiron_base/project/archiving/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/project/archiving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/project/archiving/export_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/project/archiving/import_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/project/archiving/shared.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/project/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/project/external.py
--rw-r--r--   0 runner    (1001) docker     (123)    68931 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/project/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9360 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/project/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     7230 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/project/maintenance.py
--rw-r--r--   0 runner    (1001) docker     (123)    12732 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/project/path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:34.410587 pyiron_base-0.6.2/pyiron_base/project/update/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/project/update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/project/update/pyiron_base_03x_to_04x.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:34.410587 pyiron_base-0.6.2/pyiron_base/state/
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/state/install.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/state/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/state/publications.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/state/queue_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    25086 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/state/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/state/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/state/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:34.414587 pyiron_base-0.6.2/pyiron_base/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32693 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/storage/datacontainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7321 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/storage/filedata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/storage/fileio.py
--rw-r--r--   0 runner    (1001) docker     (123)    39557 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/storage/flattenedstorage.py
--rw-r--r--   0 runner    (1001) docker     (123)    14165 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/storage/has_stored_traits.py
--rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/storage/hdfio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/storage/hdfstub.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/storage/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/storage/inputlist.py
--rw-r--r--   0 runner    (1001) docker     (123)    32625 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/storage/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:34.414587 pyiron_base-0.6.2/pyiron_base/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/utils/deprecate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/utils/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/utils/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/utils/jedi.py
--rw-r--r--   0 runner    (1001) docker     (123)    29090 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/utils/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/utils/safetar.py
--rw-r--r--   0 runner    (1001) docker     (123)    14338 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/pyiron_base/utils/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:34.402587 pyiron_base-0.6.2/pyiron_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-12 13:55:34.000000 pyiron_base-0.6.2/pyiron_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-07-12 13:55:34.000000 pyiron_base-0.6.2/pyiron_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 13:55:34.000000 pyiron_base-0.6.2/pyiron_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-12 13:55:34.000000 pyiron_base-0.6.2/pyiron_base.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-12 13:55:34.000000 pyiron_base-0.6.2/pyiron_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-12 13:55:34.000000 pyiron_base-0.6.2/pyiron_base.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-12 13:55:34.414587 pyiron_base-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-12 13:55:34.000000 pyiron_base-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:34.414587 pyiron_base-0.6.2/test_benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/test_benchmarks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:34.414587 pyiron_base-0.6.2/test_benchmarks/generic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/test_benchmarks/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/test_benchmarks/generic/test_filehdfio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:55:34.414587 pyiron_base-0.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/tests/test_testwithproject.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/tests/test_toolkit.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-12 13:55:30.000000 pyiron_base-0.6.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:25:17.923349 pyiron_base-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-18 06:25:14.000000 pyiron_base-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-18 06:25:14.000000 pyiron_base-0.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-18 06:25:17.923349 pyiron_base-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-07-18 06:25:14.000000 pyiron_base-0.6.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:25:17.923349 pyiron_base-0.6.3/pyiron_base/
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-18 06:25:17.923349 pyiron_base-0.6.3/pyiron_base/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:25:17.911348 pyiron_base-0.6.3/pyiron_base/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/cli/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/cli/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/cli/ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/cli/reloadfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/cli/rm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/cli/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:25:17.915348 pyiron_base-0.6.3/pyiron_base/database/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25072 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/database/filetable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45395 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/database/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/database/jobtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/database/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/database/performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/database/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:25:17.915348 pyiron_base-0.6.3/pyiron_base/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/interfaces/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/interfaces/has_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8855 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/interfaces/has_hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/interfaces/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/interfaces/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:25:17.915348 pyiron_base-0.6.3/pyiron_base/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27892 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/jobs/datamining.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/jobs/dynamic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:25:17.915348 pyiron_base-0.6.3/pyiron_base/jobs/job/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/jobs/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36820 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/jobs/job/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:25:17.915348 pyiron_base-0.6.3/pyiron_base/jobs/job/extension/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/jobs/job/extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/jobs/job/extension/executable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9527 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/jobs/job/extension/jobstatus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:25:17.919348 pyiron_base-0.6.3/pyiron_base/jobs/job/extension/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/jobs/job/extension/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20064 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/jobs/job/extension/server/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14501 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/jobs/job/extension/server/queuestatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/jobs/job/extension/server/runmode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/jobs/job/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57264 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/jobs/job/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13349 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/jobs/job/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13584 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/jobs/job/jobtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11822 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/jobs/job/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27024 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/jobs/job/runfunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/jobs/job/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/jobs/job/toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14445 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/jobs/job/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/jobs/job/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:25:17.919348 pyiron_base-0.6.3/pyiron_base/jobs/master/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/jobs/master/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/jobs/master/flexible.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16885 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/jobs/master/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/jobs/master/interactivewrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/jobs/master/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32706 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/jobs/master/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13295 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/jobs/master/serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/jobs/master/submissionstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16462 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/jobs/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14652 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/jobs/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:25:17.919348 pyiron_base-0.6.3/pyiron_base/project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:25:17.919348 pyiron_base-0.6.3/pyiron_base/project/archiving/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/project/archiving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/project/archiving/export_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/project/archiving/import_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/project/archiving/shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/project/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/project/external.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67485 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/project/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9360 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/project/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/project/jobloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7230 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/project/maintenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12732 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/project/path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:25:17.919348 pyiron_base-0.6.3/pyiron_base/project/update/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/project/update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/project/update/pyiron_base_03x_to_04x.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:25:17.919348 pyiron_base-0.6.3/pyiron_base/state/
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/state/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/state/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/state/publications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/state/queue_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25086 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/state/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/state/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/state/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:25:17.923349 pyiron_base-0.6.3/pyiron_base/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32693 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/storage/datacontainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7321 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/storage/filedata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/storage/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39557 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/storage/flattenedstorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14165 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/storage/has_stored_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/storage/hdfio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/storage/hdfstub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/storage/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/storage/inputlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32625 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/storage/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:25:17.923349 pyiron_base-0.6.3/pyiron_base/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/utils/deprecate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/utils/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/utils/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/utils/jedi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29090 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/utils/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/utils/safetar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14338 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/pyiron_base/utils/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:25:17.911348 pyiron_base-0.6.3/pyiron_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-18 06:25:17.000000 pyiron_base-0.6.3/pyiron_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-07-18 06:25:17.000000 pyiron_base-0.6.3/pyiron_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 06:25:17.000000 pyiron_base-0.6.3/pyiron_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-18 06:25:17.000000 pyiron_base-0.6.3/pyiron_base.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-18 06:25:17.000000 pyiron_base-0.6.3/pyiron_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-18 06:25:17.000000 pyiron_base-0.6.3/pyiron_base.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-18 06:25:17.923349 pyiron_base-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-18 06:25:17.000000 pyiron_base-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:25:17.923349 pyiron_base-0.6.3/test_benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/test_benchmarks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:25:17.923349 pyiron_base-0.6.3/test_benchmarks/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/test_benchmarks/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/test_benchmarks/generic/test_filehdfio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:25:17.923349 pyiron_base-0.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/tests/test_testwithproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/tests/test_toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-18 06:25:15.000000 pyiron_base-0.6.3/versioneer.py
```

### Comparing `pyiron_base-0.6.2/LICENSE` & `pyiron_base-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/PKG-INFO` & `pyiron_base-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron_base
-Version: 0.6.2
+Version: 0.6.3
 Summary: pyiron_base - an integrated development environment (IDE) for computational science.
 Home-page: https://github.com/pyiron/pyiron_base
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: janssen@mpie.de
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyiron_base-0.6.2/README.rst` & `pyiron_base-0.6.3/README.rst`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/__init__.py` & `pyiron_base-0.6.3/pyiron_base/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/_tests.py` & `pyiron_base-0.6.3/pyiron_base/_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,20 +154,27 @@
         super().setUpClass()
         job = cls.project.create_job(job_type=ToyJob, job_name="toy_1")
         job.run()
         job = cls.project.create_job(job_type=ToyJob, job_name="toy_2")
         job.run()
         job.status.aborted = True
 
-        with cls.project.open("sub_project") as pr_sub:
-            job = pr_sub.create_job(job_type=ToyJob, job_name="toy_1")
-            job.run()
-            job = pr_sub.create_job(job_type=ToyJob, job_name="toy_2")
-            job.run()
-            job.status.suspended = True
+        cls.pr_sub = cls.project.open("sub_project")
+        job = cls.pr_sub.create_job(job_type=ToyJob, job_name="toy_1")
+        job.run()
+        job = cls.pr_sub.create_job(job_type=ToyJob, job_name="toy_2")
+        job.run()
+        job.status.suspended = True
+        job = cls.pr_sub.create_job(job_type=ToyJob, job_name="toy_3")
+        job.run()
+
+        cls.n_jobs_filled_with = 5
+        # In a number of tests we compare the found jobs to an expected number of jobs
+        # Let's code that number once here instead of magic-numbering it throughout
+        # the tests
 
 
 _TO_SKIP = [
     PyironTestCase,
     TestWithProject,
     TestWithCleanProject,
     TestWithFilledProject,
```

### Comparing `pyiron_base-0.6.2/pyiron_base/cli/control.py` & `pyiron_base-0.6.3/pyiron_base/cli/control.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/cli/install.py` & `pyiron_base-0.6.3/pyiron_base/cli/install.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/cli/ls.py` & `pyiron_base-0.6.3/pyiron_base/cli/ls.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/cli/reloadfile.py` & `pyiron_base-0.6.3/pyiron_base/cli/reloadfile.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/cli/rm.py` & `pyiron_base-0.6.3/pyiron_base/cli/rm.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/cli/wrapper.py` & `pyiron_base-0.6.3/pyiron_base/cli/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/database/filetable.py` & `pyiron_base-0.6.3/pyiron_base/database/filetable.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/database/generic.py` & `pyiron_base-0.6.3/pyiron_base/database/generic.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/database/jobtable.py` & `pyiron_base-0.6.3/pyiron_base/database/jobtable.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/database/manager.py` & `pyiron_base-0.6.3/pyiron_base/database/manager.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/database/performance.py` & `pyiron_base-0.6.3/pyiron_base/database/performance.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/database/tables.py` & `pyiron_base-0.6.3/pyiron_base/database/tables.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/interfaces/factory.py` & `pyiron_base-0.6.3/pyiron_base/interfaces/factory.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/interfaces/has_groups.py` & `pyiron_base-0.6.3/pyiron_base/interfaces/has_groups.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/interfaces/has_hdf.py` & `pyiron_base-0.6.3/pyiron_base/interfaces/has_hdf.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/interfaces/object.py` & `pyiron_base-0.6.3/pyiron_base/interfaces/object.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/interfaces/singleton.py` & `pyiron_base-0.6.3/pyiron_base/interfaces/singleton.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/jobs/datamining.py` & `pyiron_base-0.6.3/pyiron_base/jobs/datamining.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/jobs/dynamic.py` & `pyiron_base-0.6.3/pyiron_base/jobs/dynamic.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/jobs/job/core.py` & `pyiron_base-0.6.3/pyiron_base/jobs/job/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -418,15 +418,15 @@
                     state.logger.error(
                         "Job {0} is a child of a master job and cannot be deleted!".format(
                             str(self.job_id)
                         )
                     )
                     raise ValueError("Child jobs are protected and cannot be deleted!")
             for job_id in self.child_ids:
-                job = self.project.load(job_id, convert_to_object=False)
+                job = self.project.inspect(job_id)
                 if len(job.child_ids) > 0:
                     job.remove(_protect_childs=False)
                 else:
                     self.project_hdf5.remove_job(job_id, _unprotect=True)
 
         # After all children are deleted, remove the job itself.
         self.remove_child()
@@ -543,15 +543,15 @@
 
         Args:
             job_specifier (str, int): name of the job or job ID
 
         Returns:
             JobCore: Access to the HDF5 object - not a GenericJob object - use load() instead.
         """
-        return self.project.load(job_specifier=job_specifier, convert_to_object=False)
+        return self.project.inspect(job_specifier=job_specifier)
 
     def is_master_id(self, job_id):
         """
         Check if the job ID job_id is the master ID for any child job
 
         Args:
             job_id (int): job ID of the master job
@@ -612,18 +612,15 @@
     def list_childs(self):
         """
         List child jobs as JobPath objects - not loading the full GenericJob objects for each child
 
         Returns:
             list: list of child jobs
         """
-        return [
-            self.project.load(child_id, convert_to_object=False).job_name
-            for child_id in self.child_ids
-        ]
+        return [self.project.inspect(child_id).job_name for child_id in self.child_ids]
 
     def _list_groups(self):
         return self.project_hdf5.list_groups() + self._list_ext_childs()
 
     def _list_nodes(self):
         return self.project_hdf5.list_nodes()
```

### Comparing `pyiron_base-0.6.2/pyiron_base/jobs/job/extension/executable.py` & `pyiron_base-0.6.3/pyiron_base/jobs/job/extension/executable.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/jobs/job/extension/jobstatus.py` & `pyiron_base-0.6.3/pyiron_base/jobs/job/extension/jobstatus.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/jobs/job/extension/server/generic.py` & `pyiron_base-0.6.3/pyiron_base/jobs/job/extension/server/generic.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from concurrent.futures import Executor, Future
 from collections import OrderedDict
 import numbers
 import socket
 from typing import Union
 
 from pyiron_base.state import state
+from pyiron_base.utils.instance import static_isinstance
 from pyiron_base.jobs.job.extension.server.runmode import Runmode
 
 __author__ = "Jan Janssen"
 __copyright__ = (
     "Copyright 2020, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
@@ -472,14 +473,16 @@
         Executor to execute the job object this server object is attached to in the background.
 
         Args:
             exe (concurrent.futures.Executor):
         """
         if isinstance(exe, Executor):
             self.run_mode.executor = True
+        elif static_isinstance(exe, "flux.job.executor.FluxExecutor"):
+            self.run_mode.executor = True
         elif exe is None and self.run_mode.executor:
             self.run_mode.modal = True
         elif exe is not None:
             raise TypeError(
                 "The executor has to be derived from the concurrent.futures.Executor class."
             )
         self._executor = exe
```

### Comparing `pyiron_base-0.6.2/pyiron_base/jobs/job/extension/server/queuestatus.py` & `pyiron_base-0.6.3/pyiron_base/jobs/job/extension/server/queuestatus.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/jobs/job/extension/server/runmode.py` & `pyiron_base-0.6.3/pyiron_base/jobs/job/extension/server/runmode.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/jobs/job/factory.py` & `pyiron_base-0.6.3/pyiron_base/jobs/job/factory.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/jobs/job/generic.py` & `pyiron_base-0.6.3/pyiron_base/jobs/job/generic.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/jobs/job/interactive.py` & `pyiron_base-0.6.3/pyiron_base/jobs/job/interactive.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/jobs/job/jobtype.py` & `pyiron_base-0.6.3/pyiron_base/jobs/job/jobtype.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/jobs/job/path.py` & `pyiron_base-0.6.3/pyiron_base/jobs/job/path.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/jobs/job/runfunction.py` & `pyiron_base-0.6.3/pyiron_base/jobs/job/runfunction.py`

 * *Files 1% similar despite different names*

```diff
@@ -490,19 +490,19 @@
         # This smells a bit, so if a better architecture is found in the future, use it
         # to avoid string-based specifications
     ):
         raise NotImplementedError(
             "Currently job.server.run_mode.executor does not support GenericMaster jobs."
         )
     if flux_available and isinstance(executor, flux.job.FluxExecutor):
-        return run_job_with_runmode_executor_flux(
+        run_job_with_runmode_executor_flux(
             job=job, executor=executor, gpus_per_slot=gpus_per_slot
         )
     elif isinstance(executor, ProcessPoolExecutor):
-        return run_job_with_runmode_executor_futures(job=job, executor=executor)
+        run_job_with_runmode_executor_futures(job=job, executor=executor)
     else:
         raise NotImplementedError(
             "Currently only flux.job.FluxExecutor and concurrent.futures.ProcessPoolExecutor are supported."
         )
 
 
 def run_job_with_runmode_executor_futures(job, executor):
@@ -613,15 +613,15 @@
         num_nodes=1,
         cores_per_slot=1,
         gpus_per_slot=gpus_per_slot,
         num_slots=job.server.cores,
     )
     jobspec.cwd = job.project_hdf5.working_directory
     jobspec.environment = dict(os.environ)
-    return executor.submit(jobspec)
+    job.server.future = executor.submit(jobspec)
 
 
 def run_time_decorator(func):
     def wrapper(job):
         if not state.database.database_is_disabled and job.job_id is not None:
             job.project.db.item_update({"timestart": datetime.now()}, job.job_id)
             func(job)
```

### Comparing `pyiron_base-0.6.2/pyiron_base/jobs/job/template.py` & `pyiron_base-0.6.3/pyiron_base/jobs/job/template.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/jobs/job/toolkit.py` & `pyiron_base-0.6.3/pyiron_base/jobs/job/toolkit.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/jobs/job/util.py` & `pyiron_base-0.6.3/pyiron_base/jobs/job/util.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/jobs/job/wrapper.py` & `pyiron_base-0.6.3/pyiron_base/jobs/job/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/jobs/master/flexible.py` & `pyiron_base-0.6.3/pyiron_base/jobs/master/flexible.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/jobs/master/generic.py` & `pyiron_base-0.6.3/pyiron_base/jobs/master/generic.py`

 * *Files 0% similar despite different names*

```diff
@@ -456,15 +456,15 @@
         name_lst = item.split("/")
         item_obj = name_lst[0]
         if item_obj in child_name_lst:
             child_id = child_id_lst[child_name_lst.index(item_obj)]
             if len(name_lst) > 1:
                 return self.project.inspect(child_id)["/".join(name_lst[1:])]
             else:
-                return self.project.load(child_id, convert_to_object=True)
+                return self.project.load(child_id)
         elif item_obj in self._job_name_lst:
             child = self._load_job_from_cache(job_name=item_obj)
             if len(name_lst) == 1:
                 return child
             else:
                 return child["/".join(name_lst[1:])]
         else:
```

### Comparing `pyiron_base-0.6.2/pyiron_base/jobs/master/interactivewrapper.py` & `pyiron_base-0.6.3/pyiron_base/jobs/master/interactivewrapper.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/jobs/master/list.py` & `pyiron_base-0.6.3/pyiron_base/jobs/master/list.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/jobs/master/parallel.py` & `pyiron_base-0.6.3/pyiron_base/jobs/master/parallel.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/jobs/master/serial.py` & `pyiron_base-0.6.3/pyiron_base/jobs/master/serial.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
         Returns:
             GenericJob: next job
         """
         if len(self) == 0:
             raise ValueError("No job available in job list, please append a job first.")
         if len(self._job_name_lst) > len(self.child_ids):
             return self.pop(-1)
-        ham_old = self.project.load(self.child_ids[-1], convert_to_object=True)
+        ham_old = self.project.load(self.child_ids[-1])
 
         if ham_old.status.aborted:
             ham_old.status.created = True
             return ham_old
         elif not ham_old.status.finished:
             return None
         if job_name is None:
@@ -202,15 +202,15 @@
             path (str): path inside the HDF5 files of the individual jobs like 'output/generic/volume'
 
         Returns:
             list: list of output from the child jobs
         """
         var_lst = []
         for child_id in self.child_ids:
-            ham = self.project.load(child_id, convert_to_object=False)
+            ham = self.project.inspect(child_id)
             var = ham.__getitem__(path)
             var_lst.append(var)
         return np.array(var_lst)
 
     def iter_jobs(self, convert_to_object=True):
         """
         Iterate over the jobs within the SerialMaster
```

### Comparing `pyiron_base-0.6.2/pyiron_base/jobs/master/submissionstatus.py` & `pyiron_base-0.6.3/pyiron_base/jobs/master/submissionstatus.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/jobs/script.py` & `pyiron_base-0.6.3/pyiron_base/jobs/script.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/jobs/worker.py` & `pyiron_base-0.6.3/pyiron_base/jobs/worker.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/project/archiving/export_archive.py` & `pyiron_base-0.6.3/pyiron_base/project/archiving/export_archive.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/project/archiving/import_archive.py` & `pyiron_base-0.6.3/pyiron_base/project/archiving/import_archive.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/project/data.py` & `pyiron_base-0.6.3/pyiron_base/project/data.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/project/external.py` & `pyiron_base-0.6.3/pyiron_base/project/external.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/project/generic.py` & `pyiron_base-0.6.3/pyiron_base/project/generic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 """
 The project object is the central import point of pyiron - all other objects can be created from this one
 """
 
+from __future__ import annotations
+
 import os
 import posixpath
 import shutil
 import stat
 from tqdm.auto import tqdm
 import pandas
 import pint
 import math
 import numpy as np
 
+from pyiron_base.project.jobloader import JobLoader, JobInspector
 from pyiron_base.project.maintenance import Maintenance
 from pyiron_base.project.path import ProjectPath
 from pyiron_base.database.filetable import FileTable
 from pyiron_base.state import state
 from pyiron_base.database.jobtable import (
     get_job_ids,
     get_job_id,
@@ -43,15 +46,18 @@
     update_from_remote,
     queue_enable_reservation,
     queue_check_job_is_waiting_or_running,
 )
 from pyiron_base.project.external import Notebook
 from pyiron_base.project.data import ProjectData
 from pyiron_base.project.archiving import export_archive, import_archive
-from typing import Generator, Union, Dict
+from typing import Generator, Union, Dict, TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from pyiron_base.jobs.job.generic import GenericJob
 
 __author__ = "Joerg Neugebauer, Jan Janssen"
 __copyright__ = (
     "Copyright 2020, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
@@ -118,14 +124,16 @@
 
         self.user = user
         self.sql_query = sql_query
         self._filter = ["groups", "nodes", "objects"]
         self._inspect_mode = False
         self._data = None
         self._creator = Creator(project=self)
+        self._loader = JobLoader(project=self)
+        self._inspector = JobInspector(project=self)
 
         self.job_type = JobTypeChoice()
 
         self._maintenance = None
 
     @property
     def state(self):
@@ -535,25 +543,17 @@
         Returns:
             Project: a project which is filtered by groups
         """
         new = self.copy()
         new._filter = ["groups"]
         return new
 
-    def inspect(self, job_specifier):
-        """
-        Inspect an existing pyiron object - most commonly a job - from the database
-
-        Args:
-            job_specifier (str, int): name of the job or job ID
-
-        Returns:
-            JobCore: Access to the HDF5 object - not a GenericJob object - use load() instead.
-        """
-        return self.load(job_specifier=job_specifier, convert_to_object=False)
+    @property
+    def inspect(self):
+        return self._inspector
 
     def iter_jobs(
         self,
         path: str = None,
         recursive: bool = True,
         convert_to_object: bool = True,
         progress: bool = True,
@@ -582,15 +582,15 @@
             representation of the jobs instead.
         """
         job_id_lst = self.job_table(recursive=recursive, **kwargs)["id"]
         if progress:
             job_id_lst = tqdm(job_id_lst)
         for job_id in job_id_lst:
             if path is not None:
-                yield self.load(job_id, convert_to_object=False)[path]
+                yield self.inspect(job_id)[path]
             else:  # Backwards compatibility - in future the option convert_to_object should be removed
                 yield self.load(job_id, convert_to_object=convert_to_object)
 
     def iter_output(self, recursive=True):
         """
         Iterate over the output of jobs within the current project and it is sub projects
 
@@ -818,42 +818,17 @@
         Returns:
             list: list of nodes/ jobs/ pyiron objects inside the project
         """
         if "nodes" not in self._filter:
             return []
         return self.get_jobs(recursive=recursive, columns=["job"])["job"]
 
-    def load(self, job_specifier, convert_to_object=True):
-        """
-        Load an existing pyiron object - most commonly a job - from the database
-
-        Args:
-            job_specifier (str, int): name of the job or job ID
-            convert_to_object (bool): convert the object to an pyiron object or only access the HDF5 file - default=True
-                                      accessing only the HDF5 file is about an order of magnitude faster, but only
-                                      provides limited functionality. Compare the GenericJob object to JobCore object.
-
-        Returns:
-            GenericJob, JobCore: Either the full GenericJob object or just a reduced JobCore object
-        """
-        if self.sql_query is not None:
-            state.logger.warning(
-                "SQL filter '%s' is active (may exclude job) ", self.sql_query
-            )
-        if not isinstance(job_specifier, (int, np.integer)):
-            job_specifier = _get_safe_job_name(name=job_specifier)
-        job_id = self.get_job_id(job_specifier=job_specifier)
-        if job_id is None:
-            state.logger.warning(
-                "Job '%s' does not exist and cannot be loaded", job_specifier
-            )
-            return None
-        return self.load_from_jobpath(
-            job_id=job_id, convert_to_object=convert_to_object
-        )
+    @property
+    def load(self):
+        return self._loader
 
     def load_from_jobpath(self, job_id=None, db_entry=None, convert_to_object=True):
         """
         Internal function to load an existing job either based on the job ID or based on the database entry dictionary.
 
         Args:
             job_id (int/ None): Job ID - optional, but either the job_id or the db_entry is required.
@@ -1129,17 +1104,15 @@
         """
         if isinstance(job_specifier, (list, np.ndarray)):
             for job_id in job_specifier:
                 self.remove_job(job_specifier=job_id, _unprotect=_unprotect)
         else:
             if not self.db.view_mode:
                 try:
-                    job = self.load(
-                        job_specifier=job_specifier, convert_to_object=False
-                    )
+                    job = self.inspect(job_specifier=job_specifier)
                     if job is None:
                         state.logger.warning(
                             "Job '%s' does not exist and could not be removed",
                             str(job_specifier),
                         )
                     elif _unprotect:
                         job.remove_child()
```

### Comparing `pyiron_base-0.6.2/pyiron_base/project/gui.py` & `pyiron_base-0.6.3/pyiron_base/project/gui.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/project/maintenance.py` & `pyiron_base-0.6.3/pyiron_base/project/maintenance.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/project/path.py` & `pyiron_base-0.6.3/pyiron_base/project/path.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/project/update/pyiron_base_03x_to_04x.py` & `pyiron_base-0.6.3/pyiron_base/project/update/pyiron_base_03x_to_04x.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/state/__init__.py` & `pyiron_base-0.6.3/pyiron_base/state/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/state/install.py` & `pyiron_base-0.6.3/pyiron_base/state/install.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/state/logger.py` & `pyiron_base-0.6.3/pyiron_base/state/logger.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/state/publications.py` & `pyiron_base-0.6.3/pyiron_base/state/publications.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/state/queue_adapter.py` & `pyiron_base-0.6.3/pyiron_base/state/queue_adapter.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/state/settings.py` & `pyiron_base-0.6.3/pyiron_base/state/settings.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/state/signal.py` & `pyiron_base-0.6.3/pyiron_base/state/signal.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/state/update.py` & `pyiron_base-0.6.3/pyiron_base/state/update.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/storage/datacontainer.py` & `pyiron_base-0.6.3/pyiron_base/storage/datacontainer.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/storage/filedata.py` & `pyiron_base-0.6.3/pyiron_base/storage/filedata.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/storage/fileio.py` & `pyiron_base-0.6.3/pyiron_base/storage/fileio.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/storage/flattenedstorage.py` & `pyiron_base-0.6.3/pyiron_base/storage/flattenedstorage.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/storage/has_stored_traits.py` & `pyiron_base-0.6.3/pyiron_base/storage/has_stored_traits.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/storage/hdfio.py` & `pyiron_base-0.6.3/pyiron_base/storage/hdfio.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/storage/hdfstub.py` & `pyiron_base-0.6.3/pyiron_base/storage/hdfstub.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/storage/helper_functions.py` & `pyiron_base-0.6.3/pyiron_base/storage/helper_functions.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/storage/parameters.py` & `pyiron_base-0.6.3/pyiron_base/storage/parameters.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/utils/deprecate.py` & `pyiron_base-0.6.3/pyiron_base/utils/deprecate.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/utils/error.py` & `pyiron_base-0.6.3/pyiron_base/utils/error.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/utils/instance.py` & `pyiron_base-0.6.3/pyiron_base/utils/instance.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/utils/jedi.py` & `pyiron_base-0.6.3/pyiron_base/utils/jedi.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/utils/parser.py` & `pyiron_base-0.6.3/pyiron_base/utils/parser.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/utils/safetar.py` & `pyiron_base-0.6.3/pyiron_base/utils/safetar.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base/utils/units.py` & `pyiron_base-0.6.3/pyiron_base/utils/units.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/pyiron_base.egg-info/PKG-INFO` & `pyiron_base-0.6.3/pyiron_base.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron-base
-Version: 0.6.2
+Version: 0.6.3
 Summary: pyiron_base - an integrated development environment (IDE) for computational science.
 Home-page: https://github.com/pyiron/pyiron_base
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: janssen@mpie.de
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyiron_base-0.6.2/pyiron_base.egg-info/SOURCES.txt` & `pyiron_base-0.6.3/pyiron_base.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,15 @@
 pyiron_base/jobs/master/serial.py
 pyiron_base/jobs/master/submissionstatus.py
 pyiron_base/project/__init__.py
 pyiron_base/project/data.py
 pyiron_base/project/external.py
 pyiron_base/project/generic.py
 pyiron_base/project/gui.py
+pyiron_base/project/jobloader.py
 pyiron_base/project/maintenance.py
 pyiron_base/project/path.py
 pyiron_base/project/archiving/__init__.py
 pyiron_base/project/archiving/export_archive.py
 pyiron_base/project/archiving/import_archive.py
 pyiron_base/project/archiving/shared.py
 pyiron_base/project/update/__init__.py
```

### Comparing `pyiron_base-0.6.2/setup.py` & `pyiron_base-0.6.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,25 +26,25 @@
                  'Programming Language :: Python :: 3.11'
                 ],
 
     keywords='pyiron',
     packages=find_packages(exclude=["*tests*", "*docs*", "*binder*", "*conda*", "*notebooks*", "*.ci_support*"]),
     install_requires=[
         'dill>=0.3.6',
-        'gitpython>=3.1.31',
+        'gitpython>=3.1.32',
         'h5io>=0.1.8',
         'h5py>=3.9.0',
         'jinja2>=3.1.2',
         'numpy>=1.24.3',
         'pandas>=2.0.3',
         'pint>=0.22',
         'psutil>=5.9.5',
         'pyfileindex>=0.0.11',
-        'pysqa>=0.0.25',
-        'sqlalchemy>=2.0.18',
+        'pysqa>=0.1.0',
+        'sqlalchemy>=2.0.19',
         'tables>=3.8.0',
         'tqdm>=4.65.0',
         'traitlets>=5.9.0',
     ],
     cmdclass=versioneer.get_cmdclass(),
 
     entry_points={
```

### Comparing `pyiron_base-0.6.2/test_benchmarks/generic/test_filehdfio.py` & `pyiron_base-0.6.3/test_benchmarks/generic/test_filehdfio.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/tests/test_testwithproject.py` & `pyiron_base-0.6.3/tests/test_testwithproject.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/tests/test_toolkit.py` & `pyiron_base-0.6.3/tests/test_toolkit.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.2/versioneer.py` & `pyiron_base-0.6.3/versioneer.py`

 * *Files identical despite different names*

