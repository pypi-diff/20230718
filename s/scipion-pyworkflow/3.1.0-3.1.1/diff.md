# Comparing `tmp/scipion-pyworkflow-3.1.0.tar.gz` & `tmp/scipion-pyworkflow-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-pyworkflow-3.1.0.tar", last modified: Fri Jun 23 15:09:55 2023, max compression
+gzip compressed data, was "scipion-pyworkflow-3.1.1.tar", last modified: Tue Jul 18 13:18:01 2023, max compression
```

## Comparing `scipion-pyworkflow-3.1.0.tar` & `scipion-pyworkflow-3.1.1.tar`

### file list

```diff
@@ -1,268 +1,268 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:09:55.481531 scipion-pyworkflow-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-06-23 15:09:55.477531 scipion-pyworkflow-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:09:55.437531 scipion-pyworkflow-3.1.0/pyworkflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:09:55.441531 scipion-pyworkflow-3.1.0/pyworkflow/apps/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_protocol_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_protocol_mpirun.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_protocol_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_protocol_run.py
--rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_run_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    12456 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_schedule_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_sleep.py
--rw-r--r--   0 runner    (1001) docker     (123)    17175 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_sync_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15892 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:09:55.445531 scipion-pyworkflow-3.1.0/pyworkflow/gui/
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25926 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/browser.py
--rw-r--r--   0 runner    (1001) docker     (123)    41189 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)    34490 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)   110339 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/form.py
--rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/graph_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    19186 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/matplotlib_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/plotter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:09:55.445531 scipion-pyworkflow-3.1.0/pyworkflow/gui/project/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/project/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/project/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/project/labels.py
--rw-r--r--   0 runner    (1001) docker     (123)    18658 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/project/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/project/searchprotocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/project/searchrun.py
--rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/project/steps.py
--rw-r--r--   0 runner    (1001) docker     (123)    12008 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/project/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19471 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/project/viewdata.py
--rw-r--r--   0 runner    (1001) docker     (123)    22545 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/project/viewprojects.py
--rw-r--r--   0 runner    (1001) docker     (123)    84839 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/project/viewprotocols.py
--rw-r--r--   0 runner    (1001) docker     (123)    21331 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/project/viewprotocols_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)    28483 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     8531 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/tooltip.py
--rw-r--r--   0 runner    (1001) docker     (123)    23038 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    11157 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:09:55.445531 scipion-pyworkflow-3.1.0/pyworkflow/mapper/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/mapper/mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    60735 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/mapper/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/mapper/sqlite_db.py
--rw-r--r--   0 runner    (1001) docker     (123)    10720 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/mapper/xmlmapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    51658 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    28103 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:09:55.445531 scipion-pyworkflow-3.1.0/pyworkflow/project/
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/project/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/project/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    71104 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/project/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:09:55.449531 scipion-pyworkflow-3.1.0/pyworkflow/project/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2600 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/project/scripts/clean_projects.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2942 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/project/scripts/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/project/scripts/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/project/scripts/edit_workflow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1057 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/project/scripts/fix_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/project/scripts/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/project/scripts/refresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/project/scripts/schedule.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      941 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/project/scripts/stack2volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/project/scripts/stop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:09:55.449531 scipion-pyworkflow-3.1.0/pyworkflow/protocol/
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/protocol/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/protocol/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    16262 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/protocol/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11515 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/protocol/hosts.py
--rw-r--r--   0 runner    (1001) docker     (123)    12213 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/protocol/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/protocol/package.py
--rw-r--r--   0 runner    (1001) docker     (123)    26337 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/protocol/params.py
--rw-r--r--   0 runner    (1001) docker     (123)    95568 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/protocol/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:09:55.469531 scipion-pyworkflow-3.1.0/pyworkflow/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/backward-solid.png
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/beta.png
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/binoculares.png
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/bookmark.png
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/broom-solid.png
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/class_obj.png
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/clipboard-regular.png
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/code-branch-solid.png
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/debug.png
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-arrow-down.png
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-arrow-left.png
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-arrow-up.png
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-ban.png
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-bars.png
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-check.png
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-checked.png
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-cog.png
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-cogs.png
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-database.png
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-delete-operation.png
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-download.png
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-exclamation-triangle_alert.png
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-external-link.png
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-eye.png
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-failure.png
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-file-o.png
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-files-o.png
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-folder-open.png
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-home.png
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-info-circle_alert.png
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-install.png
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-installed.png
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-lightbulb-o.png
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-list-ul.png
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-magic.png
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-minus-square.png
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-next.png
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-pencil.png
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-play-circle-o.png
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-plus-square.png
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-previous.png
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-processing.png
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-question-circle.png
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-refresh.png
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-rocket.png
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-save.png
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-search.png
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-sign-in.png
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-sign-out.png
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-sitemap.png
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-stop-workflow.png
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-stop.png
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-tags.png
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-times-circle_alert.png
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-times.png
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-to_install.png
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-trash-o.png
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-unchecked.png
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-undo.png
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-uninstall.png
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-update.png
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-upload.png
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/file.png
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/file_folder.png
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/file_folder_link.png
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/file_generic.png
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/file_generic_link.png
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/file_image.png
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/file_image_link.png
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/file_java.png
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/file_log.png
--rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/file_md.png
--rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/file_md_link.png
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/file_python.png
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/file_sqlite.png
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/file_stack.png
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/file_stack_link.png
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/file_text.png
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/file_vol.png
--rw-r--r--   0 runner    (1001) docker     (123)    16824 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/loading.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/new.png
--rw-r--r--   0 runner    (1001) docker     (123)    29510 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/no-image.png
--rw-r--r--   0 runner    (1001) docker     (123)    13217 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/no-image128.png
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/paste-solid.png
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/power-off-solid.png
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/production.png
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/prot_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/question.png
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/rename.png
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/root.png
--rw-r--r--   0 runner    (1001) docker     (123)   113916 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/scipion_bn.png
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/scipion_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)   126140 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/scipion_icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/scipion_icon_proj.png
--rw-r--r--   0 runner    (1001) docker     (123)    13273 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/scipion_icon_projs.png
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/scipion_icon_prot.png
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/scipion_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    35151 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/scipion_logo_normal.png
--rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/scipion_logo_small.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:09:55.473531 scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/arrowDown.png
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/arrowUp.png
--rw-r--r--   0 runner    (1001) docker     (123)   284666 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/background_section.png
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/colRowModeOff.png
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/colRowModeOn.png
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/delete.png
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/doc_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/download_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/enabled_gallery.png
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/galleryViewOff.png
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/galleryViewOn.png
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/goto.png
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/menu.png
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/separator.png
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/tableViewOff.png
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/tableViewOn.png
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/ui-bg_glass_75_e6e6e6_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/ui-bg_glass_95_fef1ec_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/ui-bg_highlight-soft_75_cccccc_1x100.png
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/volumeOff.png
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/volumeOn.png
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/updated.png
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/users.png
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/wait.gif
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/workflow.png
--rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:09:55.473531 scipion-pyworkflow-3.1.0/pyworkflow/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/tests/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:09:55.473531 scipion-pyworkflow-3.1.0/pyworkflow/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14943 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/utils/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/utils/echo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/utils/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    10664 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/utils/mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)    15296 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/utils/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/utils/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/utils/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (123)    19427 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/utils/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/utils/reflection.py
--rw-r--r--   0 runner    (1001) docker     (123)    26700 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/utils/which.py
--rw-r--r--   0 runner    (1001) docker     (123)    10966 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:09:55.473531 scipion-pyworkflow-3.1.0/pyworkflow/webservices/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/webservices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/webservices/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/webservices/notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/webservices/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/wizard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:09:55.473531 scipion-pyworkflow-3.1.0/pyworkflowtests/
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflowtests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflowtests/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (123)    26247 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflowtests/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflowtests/protocols.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:09:55.477531 scipion-pyworkflow-3.1.0/pyworkflowtests/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflowtests/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflowtests/tests/test_canvas.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1624 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflowtests/tests/test_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflowtests/tests/test_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14887 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflowtests/tests/test_mappers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18094 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflowtests/tests/test_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflowtests/tests/test_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflowtests/tests/test_protocol_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflowtests/tests/test_protocol_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflowtests/tests/test_protocol_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflowtests/tests/test_streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflowtests/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:09:55.477531 scipion-pyworkflow-3.1.0/scipion_pyworkflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-06-23 15:09:55.000000 scipion-pyworkflow-3.1.0/scipion_pyworkflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8655 2023-06-23 15:09:55.000000 scipion-pyworkflow-3.1.0/scipion_pyworkflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-23 15:09:55.000000 scipion-pyworkflow-3.1.0/scipion_pyworkflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-23 15:09:55.000000 scipion-pyworkflow-3.1.0/scipion_pyworkflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-23 15:09:55.000000 scipion-pyworkflow-3.1.0/scipion_pyworkflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-23 15:09:55.000000 scipion-pyworkflow-3.1.0/scipion_pyworkflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 15:09:55.481531 scipion-pyworkflow-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:18:01.717944 scipion-pyworkflow-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-07-18 13:18:01.717944 scipion-pyworkflow-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:18:01.697944 scipion-pyworkflow-3.1.1/pyworkflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:18:01.697944 scipion-pyworkflow-3.1.1/pyworkflow/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/apps/pw_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/apps/pw_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/apps/pw_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/apps/pw_protocol_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/apps/pw_protocol_mpirun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/apps/pw_protocol_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/apps/pw_protocol_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/apps/pw_run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12456 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/apps/pw_schedule_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/apps/pw_sleep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17175 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/apps/pw_sync_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/apps/pw_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15892 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:18:01.697944 scipion-pyworkflow-3.1.1/pyworkflow/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25926 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/gui/browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41189 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/gui/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34490 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/gui/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110339 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/gui/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/gui/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/gui/graph_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19186 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/gui/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/gui/matplotlib_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/gui/plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:18:01.701944 scipion-pyworkflow-3.1.1/pyworkflow/gui/project/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/gui/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/gui/project/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/gui/project/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/gui/project/labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18658 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/gui/project/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/gui/project/searchprotocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/gui/project/searchrun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/gui/project/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12008 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/gui/project/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19471 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/gui/project/viewdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22545 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/gui/project/viewprojects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85039 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/gui/project/viewprotocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21331 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/gui/project/viewprotocols_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28483 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/gui/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8531 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/gui/tooltip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23038 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/gui/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11157 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/gui/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:18:01.701944 scipion-pyworkflow-3.1.1/pyworkflow/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/mapper/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60735 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/mapper/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/mapper/sqlite_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10720 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/mapper/xmlmapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51658 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28103 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:18:01.701944 scipion-pyworkflow-3.1.1/pyworkflow/project/
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/project/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/project/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71104 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/project/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:18:01.701944 scipion-pyworkflow-3.1.1/pyworkflow/project/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2600 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/project/scripts/clean_projects.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2942 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/project/scripts/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/project/scripts/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/project/scripts/edit_workflow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1057 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/project/scripts/fix_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/project/scripts/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/project/scripts/refresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/project/scripts/schedule.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      941 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/project/scripts/stack2volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/project/scripts/stop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:18:01.701944 scipion-pyworkflow-3.1.1/pyworkflow/protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/protocol/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/protocol/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16262 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/protocol/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11515 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/protocol/hosts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12213 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/protocol/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/protocol/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26337 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/protocol/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95568 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/protocol/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:18:01.713944 scipion-pyworkflow-3.1.1/pyworkflow/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/backward-solid.png
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/beta.png
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/binoculares.png
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/bookmark.png
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/broom-solid.png
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/class_obj.png
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/clipboard-regular.png
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/code-branch-solid.png
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/debug.png
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-arrow-down.png
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-arrow-left.png
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-arrow-up.png
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-ban.png
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-bars.png
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-check.png
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-checked.png
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-cog.png
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-cogs.png
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-database.png
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-delete-operation.png
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-download.png
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-exclamation-triangle_alert.png
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-external-link.png
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-eye.png
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-failure.png
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-file-o.png
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-files-o.png
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-folder-open.png
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-home.png
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-info-circle_alert.png
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-install.png
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-installed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-lightbulb-o.png
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-list-ul.png
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-magic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-minus-square.png
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-next.png
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-pencil.png
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-play-circle-o.png
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-plus-square.png
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-previous.png
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-processing.png
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-question-circle.png
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-refresh.png
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-rocket.png
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-save.png
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-search.png
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-sign-in.png
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-sign-out.png
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-sitemap.png
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-stop-workflow.png
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-stop.png
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-tags.png
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-times-circle_alert.png
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-times.png
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-to_install.png
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-trash-o.png
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-unchecked.png
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-undo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-uninstall.png
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-update.png
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-upload.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/file.png
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/file_folder.png
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/file_folder_link.png
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/file_generic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/file_generic_link.png
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/file_image.png
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/file_image_link.png
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/file_java.png
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/file_log.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/file_md.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/file_md_link.png
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/file_python.png
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/file_sqlite.png
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/file_stack.png
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/file_stack_link.png
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/file_text.png
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/file_vol.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16824 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/loading.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/new.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29510 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/no-image.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13217 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/no-image128.png
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/paste-solid.png
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/power-off-solid.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/production.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/prot_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/question.png
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/rename.png
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/root.png
+-rw-r--r--   0 runner    (1001) docker     (123)   113916 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/scipion_bn.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/scipion_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)   126140 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/scipion_icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/scipion_icon_proj.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13273 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/scipion_icon_projs.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/scipion_icon_prot.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/scipion_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    35151 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/scipion_logo_normal.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/scipion_logo_small.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:18:01.713944 scipion-pyworkflow-3.1.1/pyworkflow/resources/showj/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/showj/arrowDown.png
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/showj/arrowUp.png
+-rw-r--r--   0 runner    (1001) docker     (123)   284666 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/showj/background_section.png
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/showj/colRowModeOff.png
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/showj/colRowModeOn.png
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/showj/delete.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/showj/doc_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/showj/download_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/showj/enabled_gallery.png
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/showj/galleryViewOff.png
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/showj/galleryViewOn.png
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/showj/goto.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/showj/menu.png
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/showj/separator.png
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/showj/tableViewOff.png
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/showj/tableViewOn.png
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/showj/ui-bg_glass_75_e6e6e6_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/showj/ui-bg_glass_95_fef1ec_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/showj/ui-bg_highlight-soft_75_cccccc_1x100.png
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/showj/volumeOff.png
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/showj/volumeOn.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/updated.png
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/users.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/wait.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/resources/workflow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:18:01.713944 scipion-pyworkflow-3.1.1/pyworkflow/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:18:01.717944 scipion-pyworkflow-3.1.1/pyworkflow/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14943 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/utils/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/utils/echo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/utils/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10664 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/utils/mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15296 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/utils/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/utils/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/utils/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19427 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/utils/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/utils/reflection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26700 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/utils/which.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10966 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:18:01.717944 scipion-pyworkflow-3.1.1/pyworkflow/webservices/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/webservices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/webservices/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/webservices/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/webservices/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflow/wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:18:01.717944 scipion-pyworkflow-3.1.1/pyworkflowtests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflowtests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflowtests/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26247 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflowtests/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflowtests/protocols.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:18:01.717944 scipion-pyworkflow-3.1.1/pyworkflowtests/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflowtests/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflowtests/tests/test_canvas.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1624 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflowtests/tests/test_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflowtests/tests/test_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14887 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflowtests/tests/test_mappers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18094 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflowtests/tests/test_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflowtests/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflowtests/tests/test_protocol_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflowtests/tests/test_protocol_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflowtests/tests/test_protocol_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflowtests/tests/test_streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/pyworkflowtests/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:18:01.717944 scipion-pyworkflow-3.1.1/scipion_pyworkflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-07-18 13:18:01.000000 scipion-pyworkflow-3.1.1/scipion_pyworkflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8655 2023-07-18 13:18:01.000000 scipion-pyworkflow-3.1.1/scipion_pyworkflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-18 13:18:01.000000 scipion-pyworkflow-3.1.1/scipion_pyworkflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-18 13:18:01.000000 scipion-pyworkflow-3.1.1/scipion_pyworkflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-18 13:18:01.000000 scipion-pyworkflow-3.1.1/scipion_pyworkflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-18 13:18:01.000000 scipion-pyworkflow-3.1.1/scipion_pyworkflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 13:18:01.717944 scipion-pyworkflow-3.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-07-18 13:17:51.000000 scipion-pyworkflow-3.1.1/setup.py
```

### Comparing `scipion-pyworkflow-3.1.0/LICENSE.txt` & `scipion-pyworkflow-3.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/PKG-INFO` & `scipion-pyworkflow-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scipion-pyworkflow
-Version: 3.1.0
+Version: 3.1.1
 Summary: Simple workflow platform used in scientific applications, initially developed within the Scipion framework for image processing in Electron Microscopy.
 Home-page: https://github.com/scipion-em/scipion-pyworkflow
 Author: J.M. De la Rosa Trevin, Roberto Marabini, Grigory Sharov, Josue Gomez Blanco, Pablo Conesa, Yunior Fonseca Reyna
 Author-email: delarosatrevin@scilifelab.se, roberto@cnb.csic.es, gsharov@mrc-lmb.cam.ac.uk, josue.gomez-blanco@mcgill.ca, pconesa@cnb.csic.es, fonsecareyna@cnb.csic.es
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-pyworkflow/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-pyworkflow/
 Keywords: workflows science electron-microscopy cryo-em structural-biology image-processing scipion
```

### Comparing `scipion-pyworkflow-3.1.0/README.rst` & `scipion-pyworkflow-3.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/__init__.py` & `scipion-pyworkflow-3.1.1/pyworkflow/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/apps/__init__.py` & `scipion-pyworkflow-3.1.1/pyworkflow/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_manager.py` & `scipion-pyworkflow-3.1.1/pyworkflow/apps/pw_manager.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_plot.py` & `scipion-pyworkflow-3.1.1/pyworkflow/apps/pw_plot.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_project.py` & `scipion-pyworkflow-3.1.1/pyworkflow/apps/pw_project.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_protocol_list.py` & `scipion-pyworkflow-3.1.1/pyworkflow/apps/pw_protocol_list.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_protocol_mpirun.py` & `scipion-pyworkflow-3.1.1/pyworkflow/apps/pw_protocol_mpirun.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_protocol_remote.py` & `scipion-pyworkflow-3.1.1/pyworkflow/apps/pw_protocol_remote.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_protocol_run.py` & `scipion-pyworkflow-3.1.1/pyworkflow/apps/pw_protocol_run.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_run_tests.py` & `scipion-pyworkflow-3.1.1/pyworkflow/apps/pw_run_tests.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_schedule_run.py` & `scipion-pyworkflow-3.1.1/pyworkflow/apps/pw_schedule_run.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_sleep.py` & `scipion-pyworkflow-3.1.1/pyworkflow/apps/pw_sleep.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_sync_data.py` & `scipion-pyworkflow-3.1.1/pyworkflow/apps/pw_sync_data.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_viewer.py` & `scipion-pyworkflow-3.1.1/pyworkflow/apps/pw_viewer.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/config.py` & `scipion-pyworkflow-3.1.1/pyworkflow/config.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/constants.py` & `scipion-pyworkflow-3.1.1/pyworkflow/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 CORE_VERSION = '3.0.0'
 
 # Versions
 VERSION_1 = '1.0.0'
 VERSION_1_1 = '1.1.0'
 VERSION_1_2 = '1.2.0'
 VERSION_2_0 = '2.0.0'
-VERSION_3_0 = '3.1.0'
+VERSION_3_0 = '3.1.1'
 
 # For a new release, define a new constant and assign it to LAST_VERSION
 # The existing one has to be added to OLD_VERSIONS list.
 LAST_VERSION = VERSION_3_0
 OLD_VERSIONS = (VERSION_1, VERSION_1_1, VERSION_1_2, VERSION_2_0)
 
 # STATUS
```

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/gui/__init__.py` & `scipion-pyworkflow-3.1.1/pyworkflow/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/gui/browser.py` & `scipion-pyworkflow-3.1.1/pyworkflow/gui/browser.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/gui/canvas.py` & `scipion-pyworkflow-3.1.1/pyworkflow/gui/canvas.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/gui/dialog.py` & `scipion-pyworkflow-3.1.1/pyworkflow/gui/dialog.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/gui/form.py` & `scipion-pyworkflow-3.1.1/pyworkflow/gui/form.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/gui/graph.py` & `scipion-pyworkflow-3.1.1/pyworkflow/gui/graph.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/gui/graph_layout.py` & `scipion-pyworkflow-3.1.1/pyworkflow/gui/graph_layout.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/gui/gui.py` & `scipion-pyworkflow-3.1.1/pyworkflow/gui/gui.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/gui/matplotlib_image.py` & `scipion-pyworkflow-3.1.1/pyworkflow/gui/matplotlib_image.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/gui/plotter.py` & `scipion-pyworkflow-3.1.1/pyworkflow/gui/plotter.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/gui/project/__init__.py` & `scipion-pyworkflow-3.1.1/pyworkflow/gui/project/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/gui/project/base.py` & `scipion-pyworkflow-3.1.1/pyworkflow/gui/project/base.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/gui/project/constants.py` & `scipion-pyworkflow-3.1.1/pyworkflow/gui/project/constants.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/gui/project/labels.py` & `scipion-pyworkflow-3.1.1/pyworkflow/gui/project/labels.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/gui/project/project.py` & `scipion-pyworkflow-3.1.1/pyworkflow/gui/project/project.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/gui/project/searchprotocol.py` & `scipion-pyworkflow-3.1.1/pyworkflow/gui/project/searchprotocol.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/gui/project/searchrun.py` & `scipion-pyworkflow-3.1.1/pyworkflow/gui/project/searchrun.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/gui/project/steps.py` & `scipion-pyworkflow-3.1.1/pyworkflow/gui/project/steps.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/gui/project/utils.py` & `scipion-pyworkflow-3.1.1/pyworkflow/gui/project/utils.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/gui/project/viewdata.py` & `scipion-pyworkflow-3.1.1/pyworkflow/gui/project/viewdata.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/gui/project/viewprojects.py` & `scipion-pyworkflow-3.1.1/pyworkflow/gui/project/viewprojects.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/gui/project/viewprotocols.py` & `scipion-pyworkflow-3.1.1/pyworkflow/gui/project/viewprotocols.py`

 * *Files 0% similar despite different names*

```diff
@@ -1767,14 +1767,17 @@
                         project._restartWorkflow(workflowProtocolList)
                     else:
                         project._continueWorkflow(workflowProtocolList)
 
                     return [], RESULT_RUN_ALL
 
                 elif result == RESULT_RUN_SINGLE:
+                    # If mode resume, we should not reset the "current" protocol
+                    if mode==pwprot.MODE_RESUME:
+                        workflowProtocolList.pop(protocol.getObjId())
                     errorList = project.resetWorkFlow(workflowProtocolList)
                     return errorList, RESULT_RUN_SINGLE
 
                 elif result == RESULT_CANCEL:
                     return [], RESULT_CANCEL
 
             else:  # is a single protocol
```

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/gui/project/viewprotocols_extra.py` & `scipion-pyworkflow-3.1.1/pyworkflow/gui/project/viewprotocols_extra.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/gui/text.py` & `scipion-pyworkflow-3.1.1/pyworkflow/gui/text.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/gui/tooltip.py` & `scipion-pyworkflow-3.1.1/pyworkflow/gui/tooltip.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/gui/tree.py` & `scipion-pyworkflow-3.1.1/pyworkflow/gui/tree.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/gui/widgets.py` & `scipion-pyworkflow-3.1.1/pyworkflow/gui/widgets.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/mapper/__init__.py` & `scipion-pyworkflow-3.1.1/pyworkflow/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/mapper/mapper.py` & `scipion-pyworkflow-3.1.1/pyworkflow/mapper/mapper.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/mapper/sqlite.py` & `scipion-pyworkflow-3.1.1/pyworkflow/mapper/sqlite.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/mapper/sqlite_db.py` & `scipion-pyworkflow-3.1.1/pyworkflow/mapper/sqlite_db.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/mapper/xmlmapper.py` & `scipion-pyworkflow-3.1.1/pyworkflow/mapper/xmlmapper.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/object.py` & `scipion-pyworkflow-3.1.1/pyworkflow/object.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/plugin.py` & `scipion-pyworkflow-3.1.1/pyworkflow/plugin.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/project/__init__.py` & `scipion-pyworkflow-3.1.1/pyworkflow/project/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/project/config.py` & `scipion-pyworkflow-3.1.1/pyworkflow/project/config.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/project/manager.py` & `scipion-pyworkflow-3.1.1/pyworkflow/project/manager.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/project/project.py` & `scipion-pyworkflow-3.1.1/pyworkflow/project/project.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/project/scripts/clean_projects.py` & `scipion-pyworkflow-3.1.1/pyworkflow/project/scripts/clean_projects.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/project/scripts/config.py` & `scipion-pyworkflow-3.1.1/pyworkflow/project/scripts/config.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/project/scripts/create.py` & `scipion-pyworkflow-3.1.1/pyworkflow/project/scripts/create.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/project/scripts/edit_workflow.py` & `scipion-pyworkflow-3.1.1/pyworkflow/project/scripts/edit_workflow.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/project/scripts/fix_links.py` & `scipion-pyworkflow-3.1.1/pyworkflow/project/scripts/fix_links.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/project/scripts/load.py` & `scipion-pyworkflow-3.1.1/pyworkflow/project/scripts/load.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/project/scripts/refresh.py` & `scipion-pyworkflow-3.1.1/pyworkflow/project/scripts/refresh.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/project/scripts/schedule.py` & `scipion-pyworkflow-3.1.1/pyworkflow/project/scripts/schedule.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/project/scripts/stack2volume.py` & `scipion-pyworkflow-3.1.1/pyworkflow/project/scripts/stack2volume.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/project/scripts/stop.py` & `scipion-pyworkflow-3.1.1/pyworkflow/project/scripts/stop.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/protocol/__init__.py` & `scipion-pyworkflow-3.1.1/pyworkflow/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/protocol/bibtex.py` & `scipion-pyworkflow-3.1.1/pyworkflow/protocol/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/protocol/constants.py` & `scipion-pyworkflow-3.1.1/pyworkflow/protocol/constants.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/protocol/executor.py` & `scipion-pyworkflow-3.1.1/pyworkflow/protocol/executor.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/protocol/hosts.py` & `scipion-pyworkflow-3.1.1/pyworkflow/protocol/hosts.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/protocol/launch.py` & `scipion-pyworkflow-3.1.1/pyworkflow/protocol/launch.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/protocol/package.py` & `scipion-pyworkflow-3.1.1/pyworkflow/protocol/package.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/protocol/params.py` & `scipion-pyworkflow-3.1.1/pyworkflow/protocol/params.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/protocol/protocol.py` & `scipion-pyworkflow-3.1.1/pyworkflow/protocol/protocol.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/resources/beta.png` & `scipion-pyworkflow-3.1.1/pyworkflow/resources/beta.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/resources/binoculares.png` & `scipion-pyworkflow-3.1.1/pyworkflow/resources/binoculares.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/resources/bookmark.png` & `scipion-pyworkflow-3.1.1/pyworkflow/resources/bookmark.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-cog.png` & `scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-cog.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-exclamation-triangle_alert.png` & `scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-exclamation-triangle_alert.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-info-circle_alert.png` & `scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-info-circle_alert.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-tags.png` & `scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-tags.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-times-circle_alert.png` & `scipion-pyworkflow-3.1.1/pyworkflow/resources/fa-times-circle_alert.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/resources/file.png` & `scipion-pyworkflow-3.1.1/pyworkflow/resources/file.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/resources/file_folder.png` & `scipion-pyworkflow-3.1.1/pyworkflow/resources/file_folder.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/resources/file_folder_link.png` & `scipion-pyworkflow-3.1.1/pyworkflow/resources/file_folder_link.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/resources/file_image.png` & `scipion-pyworkflow-3.1.1/pyworkflow/resources/file_image.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/resources/file_image_link.png` & `scipion-pyworkflow-3.1.1/pyworkflow/resources/file_image_link.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/resources/file_java.png` & `scipion-pyworkflow-3.1.1/pyworkflow/resources/file_java.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/resources/file_log.png` & `scipion-pyworkflow-3.1.1/pyworkflow/resources/file_log.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/resources/file_md.png` & `scipion-pyworkflow-3.1.1/pyworkflow/resources/file_md.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/resources/file_md_link.png` & `scipion-pyworkflow-3.1.1/pyworkflow/resources/file_md_link.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/resources/file_python.png` & `scipion-pyworkflow-3.1.1/pyworkflow/resources/file_python.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/resources/file_sqlite.png` & `scipion-pyworkflow-3.1.1/pyworkflow/resources/file_sqlite.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/resources/file_text.png` & `scipion-pyworkflow-3.1.1/pyworkflow/resources/file_text.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/resources/file_vol.png` & `scipion-pyworkflow-3.1.1/pyworkflow/resources/file_vol.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/resources/loading.gif` & `scipion-pyworkflow-3.1.1/pyworkflow/resources/loading.gif`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/resources/new.png` & `scipion-pyworkflow-3.1.1/pyworkflow/resources/new.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/resources/no-image.png` & `scipion-pyworkflow-3.1.1/pyworkflow/resources/no-image.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/resources/no-image128.png` & `scipion-pyworkflow-3.1.1/pyworkflow/resources/no-image128.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/resources/production.png` & `scipion-pyworkflow-3.1.1/pyworkflow/resources/production.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/resources/prot_disabled.png` & `scipion-pyworkflow-3.1.1/pyworkflow/resources/prot_disabled.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/resources/question.png` & `scipion-pyworkflow-3.1.1/pyworkflow/resources/question.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/resources/scipion_bn.png` & `scipion-pyworkflow-3.1.1/pyworkflow/resources/scipion_bn.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/resources/scipion_icon.png` & `scipion-pyworkflow-3.1.1/pyworkflow/resources/scipion_icon.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/resources/scipion_icon.svg` & `scipion-pyworkflow-3.1.1/pyworkflow/resources/scipion_icon.svg`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/resources/scipion_icon_proj.png` & `scipion-pyworkflow-3.1.1/pyworkflow/resources/scipion_icon_proj.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/resources/scipion_icon_projs.png` & `scipion-pyworkflow-3.1.1/pyworkflow/resources/scipion_icon_projs.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/resources/scipion_icon_prot.png` & `scipion-pyworkflow-3.1.1/pyworkflow/resources/scipion_icon_prot.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/resources/scipion_logo.png` & `scipion-pyworkflow-3.1.1/pyworkflow/resources/scipion_logo.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/resources/scipion_logo_normal.png` & `scipion-pyworkflow-3.1.1/pyworkflow/resources/scipion_logo_normal.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/resources/scipion_logo_small.png` & `scipion-pyworkflow-3.1.1/pyworkflow/resources/scipion_logo_small.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/background_section.png` & `scipion-pyworkflow-3.1.1/pyworkflow/resources/showj/background_section.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/delete.png` & `scipion-pyworkflow-3.1.1/pyworkflow/resources/showj/delete.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/doc_icon.png` & `scipion-pyworkflow-3.1.1/pyworkflow/resources/showj/doc_icon.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/download_icon.png` & `scipion-pyworkflow-3.1.1/pyworkflow/resources/showj/download_icon.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/menu.png` & `scipion-pyworkflow-3.1.1/pyworkflow/resources/showj/menu.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/volumeOff.png` & `scipion-pyworkflow-3.1.1/pyworkflow/resources/showj/volumeOff.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/volumeOn.png` & `scipion-pyworkflow-3.1.1/pyworkflow/resources/showj/volumeOn.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/resources/updated.png` & `scipion-pyworkflow-3.1.1/pyworkflow/resources/updated.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/resources/wait.gif` & `scipion-pyworkflow-3.1.1/pyworkflow/resources/wait.gif`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/template.py` & `scipion-pyworkflow-3.1.1/pyworkflow/template.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/tests/__init__.py` & `scipion-pyworkflow-3.1.1/pyworkflow/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/tests/tests.py` & `scipion-pyworkflow-3.1.1/pyworkflow/tests/tests.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/utils/__init__.py` & `scipion-pyworkflow-3.1.1/pyworkflow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/utils/dataset.py` & `scipion-pyworkflow-3.1.1/pyworkflow/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/utils/echo.py` & `scipion-pyworkflow-3.1.1/pyworkflow/utils/echo.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/utils/graph.py` & `scipion-pyworkflow-3.1.1/pyworkflow/utils/graph.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/utils/log.py` & `scipion-pyworkflow-3.1.1/pyworkflow/utils/log.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/utils/mpi.py` & `scipion-pyworkflow-3.1.1/pyworkflow/utils/mpi.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/utils/path.py` & `scipion-pyworkflow-3.1.1/pyworkflow/utils/path.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/utils/process.py` & `scipion-pyworkflow-3.1.1/pyworkflow/utils/process.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/utils/profiler.py` & `scipion-pyworkflow-3.1.1/pyworkflow/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/utils/progressbar.py` & `scipion-pyworkflow-3.1.1/pyworkflow/utils/progressbar.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/utils/properties.py` & `scipion-pyworkflow-3.1.1/pyworkflow/utils/properties.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/utils/reflection.py` & `scipion-pyworkflow-3.1.1/pyworkflow/utils/reflection.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/utils/utils.py` & `scipion-pyworkflow-3.1.1/pyworkflow/utils/utils.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/utils/which.py` & `scipion-pyworkflow-3.1.1/pyworkflow/utils/which.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/viewer.py` & `scipion-pyworkflow-3.1.1/pyworkflow/viewer.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/webservices/config.py` & `scipion-pyworkflow-3.1.1/pyworkflow/webservices/config.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/webservices/notifier.py` & `scipion-pyworkflow-3.1.1/pyworkflow/webservices/notifier.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/webservices/repository.py` & `scipion-pyworkflow-3.1.1/pyworkflow/webservices/repository.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflow/wizard.py` & `scipion-pyworkflow-3.1.1/pyworkflow/wizard.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflowtests/__init__.py` & `scipion-pyworkflow-3.1.1/pyworkflowtests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflowtests/bibtex.py` & `scipion-pyworkflow-3.1.1/pyworkflowtests/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflowtests/objects.py` & `scipion-pyworkflow-3.1.1/pyworkflowtests/objects.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflowtests/protocols.py` & `scipion-pyworkflow-3.1.1/pyworkflowtests/protocols.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflowtests/tests/test_canvas.py` & `scipion-pyworkflow-3.1.1/pyworkflowtests/tests/test_canvas.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflowtests/tests/test_domain.py` & `scipion-pyworkflow-3.1.1/pyworkflowtests/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflowtests/tests/test_logs.py` & `scipion-pyworkflow-3.1.1/pyworkflowtests/tests/test_logs.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflowtests/tests/test_mappers.py` & `scipion-pyworkflow-3.1.1/pyworkflowtests/tests/test_mappers.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflowtests/tests/test_object.py` & `scipion-pyworkflow-3.1.1/pyworkflowtests/tests/test_object.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflowtests/tests/test_project.py` & `scipion-pyworkflow-3.1.1/pyworkflowtests/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflowtests/tests/test_protocol_execution.py` & `scipion-pyworkflow-3.1.1/pyworkflowtests/tests/test_protocol_execution.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflowtests/tests/test_protocol_export.py` & `scipion-pyworkflow-3.1.1/pyworkflowtests/tests/test_protocol_export.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflowtests/tests/test_protocol_output.py` & `scipion-pyworkflow-3.1.1/pyworkflowtests/tests/test_protocol_output.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflowtests/tests/test_streaming.py` & `scipion-pyworkflow-3.1.1/pyworkflowtests/tests/test_streaming.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/pyworkflowtests/tests/test_utils.py` & `scipion-pyworkflow-3.1.1/pyworkflowtests/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/requirements.txt` & `scipion-pyworkflow-3.1.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/scipion_pyworkflow.egg-info/PKG-INFO` & `scipion-pyworkflow-3.1.1/scipion_pyworkflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scipion-pyworkflow
-Version: 3.1.0
+Version: 3.1.1
 Summary: Simple workflow platform used in scientific applications, initially developed within the Scipion framework for image processing in Electron Microscopy.
 Home-page: https://github.com/scipion-em/scipion-pyworkflow
 Author: J.M. De la Rosa Trevin, Roberto Marabini, Grigory Sharov, Josue Gomez Blanco, Pablo Conesa, Yunior Fonseca Reyna
 Author-email: delarosatrevin@scilifelab.se, roberto@cnb.csic.es, gsharov@mrc-lmb.cam.ac.uk, josue.gomez-blanco@mcgill.ca, pconesa@cnb.csic.es, fonsecareyna@cnb.csic.es
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-pyworkflow/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-pyworkflow/
 Keywords: workflows science electron-microscopy cryo-em structural-biology image-processing scipion
```

### Comparing `scipion-pyworkflow-3.1.0/scipion_pyworkflow.egg-info/SOURCES.txt` & `scipion-pyworkflow-3.1.1/scipion_pyworkflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.1.0/setup.py` & `scipion-pyworkflow-3.1.1/setup.py`

 * *Files identical despite different names*

